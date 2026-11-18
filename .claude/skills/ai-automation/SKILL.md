---
name: ai-automation
description: Wire the production pipeline into an autonomous system - scheduled runs, tool and API integrations (generation, voice, upload, analytics), secrets handling, job state and retries, cost guards, logging, and where humans must stay in the loop. Use when automating any step, adding a new tool or API, setting up schedules, or debugging an automated run.
---

# AI automation

The goal is an agent that can carry an episode from backlog to "ready for approval" with no hand-holding, and publish after a human approves.

## Architecture

```
Scheduler (cron / Claude Code scheduled task / GitHub Actions)
   -> episode-producer agent (.claude/agents/episode-producer.md)
        reads status.yaml -> runs the next stage's skill -> writes outputs -> updates status.yaml
        calls tools via scripts in tools/ (one script per external API)
   -> stops at human gates; posts a summary for the owner
```

State lives in files (`episodes/*/status.yaml`), so runs are resumable and auditable through git history. Each run should do one stage of one episode (or one batch step), commit, and exit.

## Tool adapters (`tools/`)

Write a small script per external service with a consistent CLI, e.g.:

```
tools/gen_image.py   --prompt-file p.txt --ref brand/characters/kai/ref.png --out assets/SC02-SH03_kf_v1.png
tools/gen_video.py   --image kf.png --motion-file m.txt --seconds 5 --out assets/SC02-SH03_v1.mp4
tools/tts.py         --voice kai --text-file line.txt --out audio/dialogue/SC02_KAI_01.wav
tools/upload_youtube.py --video ... --metadata metadata/youtube.md --privacy private
tools/yt_analytics.py --since 7d --out analytics/raw/
```

Each adapter must: read keys from environment variables, print the cost of the call, append a row to `finance/ledger.csv`, retry transient errors up to 3 times with backoff, and exit non-zero on failure with a clear message. Swap vendors by swapping the adapter, not the skills.

## Secrets

- API keys only in environment variables / the environment's secret store (or GitHub Actions secrets). Never commit keys; add `.env` to `.gitignore`.
- OAuth tokens for YouTube/TikTok/Instagram upload belong to the owner's accounts and use the narrowest scopes (upload only, not delete or account management).

## Schedules (defaults)

| Job | When | What |
|-----|------|------|
| Producer run | daily | Advance the next episode one stage |
| Shorts packager | twice weekly | Cut and package verticals from finished episodes |
| Analytics | Monday | Pull stats, write weekly report |
| Accounting close | 1st of month | Monthly close |
| Compliance refresh | quarterly | Re-check platform rules, update compliance log |

## Guardrails (hard-coded, not optional)

1. **Human approval before public publishing** (see `social-media-management`). Uploads default to private/draft.
2. **Budget guard:** adapters refuse to run if the episode's spend exceeds its budget in `brand/brand.md`.
3. **QA guard:** the upload adapter refuses unless `qa-report.md` says `RESULT: PASS` and `approvals.publish` is set.
4. **No real-child data:** adapters refuse image or voice inputs outside `brand/` and `episodes/*/assets/`.
5. **Loop guard:** a stage that fails twice sets a blocker and stops.
6. **Kill switch:** if `PAUSE` file exists at repo root, every job exits immediately.

## Logging

Each run appends to `logs/runs.md`: timestamp, episode, stage, result, cost, next step. Keep it short; git history holds detail.

## Building it in steps

1. Manual: run skills by hand for the pilot episode to learn the real costs and failure points.
2. Semi-automatic: adapters for generation and TTS; human does edit and upload.
3. Automatic to approval: producer agent on a daily schedule; owner reviews and publishes.
4. Automatic publish after approval: upload adapter schedules approved posts.

Do not jump to step 4 before at least 3 episodes have gone through step 3 cleanly.
