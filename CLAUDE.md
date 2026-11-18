# Tiger Belt: The 24 Doors (working title)

Anime-style animated series teaching boys aged 6-10 the stories and values of ITF Taekwon-Do (General Choi Hong Hi's teachings: belt meanings, the 24 patterns, the five tenets), with a self-defense lesson at the end of every episode. Published on YouTube (Made for Kids), with TikTok and Instagram aimed at parents.

## Where things live
- `.claude/agents/episode-producer.md`: the autonomous showrunner agent
- `.claude/skills/`: one skill per job (start with `production-pipeline`)
- `references/itf/`: ITF lore source of truth (patterns, belts, tenets, General Choi, self-defense lesson library)
- `brand/brand.md`: brand file (owner, budgets, reviewer, fonts, colours)
- `episodes/`: one folder per episode, each with `status.yaml`; plus `backlog.md`, `continuity.md`
- `finance/ledger.csv`: every expense and income line
- `analytics/`, `business/`, `social/`, `logs/`, `tools/`

## Rules for every session
1. Nothing is published publicly without the owner's (Randy's) written approval.
2. Follow `child-safety-compliance` and `content-qa`; all YouTube uploads are Made for Kids.
3. Lore facts come only from `references/itf/`; unknowns are marked `[VERIFY]`.
4. Never use images, voices, or details of real children, including the owner's son.
5. Never spend money or change accounts without approval; log all costs.
6. API keys live in environment variables only.
7. If a `PAUSE` file exists at the repo root, do nothing and report it.
