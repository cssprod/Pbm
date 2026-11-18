# ITF Taekwon-Do Lore References

Reference library for a kids' (ages 6-10) animated series built on **ITF Taekwon-Do**, the martial art founded by **General Choi Hong Hi**. The focus is the **myth, history and philosophy** behind the belts and the 24 patterns, not fighting. Each episode ends with an age-appropriate **self-defense lesson**.

The production skills (script writing, storytelling, video generation and so on) read these files as their source of truth.

## Files

| File | What's in it | Use it for |
|---|---|---|
| [general-choi.md](general-choi.md) | Kid-friendly founder bio, philosophy, **topics to avoid** | Origin episode, brand-safety rules |
| [tenets-and-oath.md](tenets-and-oath.md) | The 5 tenets (Korean + kid meaning + story hooks), Student Oath | One tenet per episode, opening/closing chant |
| [belts.md](belts.md) | Belt colour meanings (seed → tree), kup/dan ranks, pattern per belt | Season arcs, visual motifs |
| [patterns.md](patterns.md) | All 24 patterns: official meaning, movement and diagram symbolism, history check, **kid retelling**, episode hooks, what to avoid | The main plot source for every episode |
| [patterns.json](patterns.json) | Machine-readable summary of patterns.md (moves, belt, tenet, moral, sensitivity, paired lesson) | Automation and episode planning |
| [terminology.md](terminology.md) | Korean terms, commands, counting, stances, techniques, pronunciation | Dialogue, on-screen captions, voice direction |
| [self-defense-lessons.md](self-defense-lessons.md) | 25 kid-safe lessons (SD-01…SD-25), ground rules, pairing table | End-of-episode segment |
| [sources.md](sources.md) | All citations, plus what still needs verifying | Fact-checking |

## Rules of thumb for writers

1. **Pattern = plot, tenet = moral, belt = character growth, SD lesson = ending.**
2. Quote the **official ITF meaning** for the pattern. Tell the **kid retelling** for the story.
3. Follow every **Avoid** note. No killing, executions or war gore on screen. Present history without villainising present-day nations.
4. Use **Ko-Dang**, not Juche, for the 2nd Dan slot (see `general-choi.md`).
5. Spell the founder's name **Choi Hong Hi**.
6. Don't reproduce any ITF organization's logo or crest. Design an original series emblem.
7. Treat items under "Not yet verified" in `sources.md` as unconfirmed until someone checks them.

## Suggested series structure

- **Season 1 (colour belts):** 9 pattern episodes (Chon-Ji → Choong-Moo) plus a General Choi origin episode and a Student Oath episode. The hero grows from white belt to red/black belt, matching the belt story of the seed growing into a tree.
- **Season 2 (black belt legends):** 15 dan patterns as "legend" episodes told by the instructor (Dragon King's flute, Ul-Ji's poem, Admiral Yi's 13 ships, King Sejong's letters, and so on).
- **Finale:** Tong-Il, "two halves become one", mirroring Chon-Ji in the pilot.
