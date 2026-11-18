---
name: production-pipeline
description: Master workflow for producing one episode of the kids ITF Taekwondo anime series from idea to approved upload package. Use whenever starting, resuming, or checking the status of an episode, or when deciding which skill to use next.
---

# Production pipeline

This is the spine of the operation. Every episode moves through the same stages, and every stage writes its output into the episode folder so any session (or a human) can pick up where the last one stopped.

## Episode folder layout

```
episodes/EP###-short-slug/
  status.yaml          # stage, owner, blockers, approvals (source of truth)
  brief.md             # stage 1 output
  outline.md           # stage 2
  script.md            # stage 3 (includes the self-defense segment)
  storyboard.md        # stage 4 (shot list with prompts)
  assets/              # generated images, clips, audio (gitignored if large)
  audio/               # voice lines, music, sfx
  edit/                # project files, renders
  deliverables/        # final masters per platform
  metadata/            # titles, descriptions, tags, thumbnails per platform
  qa-report.md         # stage 9
  approval.md          # stage 10, signed off by the parent/owner
```

`status.yaml` template:

```yaml
episode: EP001
title_working: "The White Belt Seed"
pattern_or_theme: "White belt meaning + Chon-Ji intro"
tenet: courtesy
self_defense_topic: "Strong voice and safe distance"
stage: brief            # brief|outline|script|storyboard|generate|audio|edit|package|qa|approval|scheduled|published
blockers: []
approvals:
  script: null          # name + date when approved
  final_cut: null
  publish: null
costs_usd: 0
updated: 2026-11-18
```

## Stages and the skill that owns each

| # | Stage | Skill | Output |
|---|-------|-------|--------|
| 1 | Brief | `storytelling`, `itf-lore`, `analytics-and-growth` | brief.md: lesson, tenet, belt/pattern, self-defense topic, hook |
| 2 | Outline | `storytelling`, `series-bible` | beat sheet that fits the chosen format |
| 3 | Script | `script-writing`, `self-defense-lessons` | script.md with timings |
| 4 | Storyboard | `art-direction` | shot list + image/video prompts |
| 5 | Generate visuals | `video-generation` | clips in assets/ |
| 6 | Voice, music, SFX | `voice-and-music` | audio stems |
| 7 | Edit and captions | `video-editing` | masters for 16:9 and 9:16 |
| 8 | Package | `thumbnails-and-seo`, `brand-management` | metadata/ per platform |
| 9 | QA | `content-qa`, `child-safety-compliance`, `rights-and-licensing` | qa-report.md (pass/fail) |
| 10 | Human approval | (the owner) | approval.md signed |
| 11 | Schedule and publish | `social-media-management` | scheduled posts, links in status.yaml |
| 12 | Review | `analytics-and-growth`, `accounting` | learnings + costs logged |

## Rules

1. **Never skip QA, never skip human approval.** Nothing goes public until `approvals.publish` is filled in by the owner (Randy). The agent may prepare and schedule drafts as private/unlisted, but flipping to public is a human step.
2. **Lore before story.** Read the matching file in `references/itf/` before writing the brief. If a fact is not in the references, mark it `[VERIFY]` and do not present it as fact on screen.
3. **Every episode ends with a self-defense lesson** (see `self-defense-lessons`). Shorts may make the lesson the whole short.
4. **Log every paid generation** to `finance/ledger.csv` (see `accounting`) as it happens.
5. **Update status.yaml at the end of every stage**, including blockers. If a stage fails twice, stop and record the blocker instead of looping.
6. **Batch where possible.** Write 3-4 scripts in one sitting, then generate visuals for all of them, so characters stay consistent and costs stay predictable.

## Cadence (starting target, adjust with analytics)

- 1 main episode (3-6 min, 16:9) every 2 weeks.
- 3 shorts (30-60 s, 9:16) per week, cut from the episode or standalone lessons.
- Season = one belt colour. Season 1 = White to Yellow (Chon-Ji, Dan-Gun), and so on up the belt ladder, so the show grows with the viewer.

## Starting a new episode

1. Pick the next item from `episodes/backlog.md` (create it if missing; seed it from `itf-lore` season map).
2. Create the folder and `status.yaml` from the template.
3. Run stage 1. Continue stage by stage until you reach a human gate or a blocker.
4. At a human gate, write a short summary for the owner: what was made, what it cost, what needs a decision.
