# Tiger Belt: The 24 Doors (working title)

An AI-assisted production system for an anime-style kids' series about ITF Taekwon-Do: the myths and meanings behind the belts and patterns, the five tenets, and a self-defense lesson at the end of every episode.

## How it works
The `episode-producer` agent (`.claude/agents/episode-producer.md`) advances episodes through the pipeline in `.claude/skills/production-pipeline/SKILL.md`, using one skill per job:

| Area | Skills |
|------|--------|
| Story and lore | itf-lore, series-bible, storytelling, script-writing, self-defense-lessons |
| Production | art-direction, video-generation, voice-and-music, video-editing, episode-formats |
| Release | thumbnails-and-seo, social-media-management, brand-management |
| Safety and rights | child-safety-compliance, rights-and-licensing, content-qa |
| Business | analytics-and-growth, business-strategy, accounting |
| System | production-pipeline, ai-automation |

Human gates: script approval for sensitive topics, instructor sign-off on safety lessons, the kid test, and final publish approval. Uploads stay private until the owner approves.

## Getting started
1. Fill in `brand/brand.md` (budgets, instructor reviewer, handles).
2. Make sure `references/itf/` is populated.
3. In Claude Code, run the `episode-producer` agent: "Start the pilot episode."
