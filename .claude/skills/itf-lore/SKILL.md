---
name: itf-lore
description: How to use ITF Taekwondo history, belt meanings, the tenets, the student oath, and the 24 pattern legends (Chon-Ji to Tong-Il) as accurate, kid-appropriate story material. Use whenever an episode touches a pattern, belt, tenet, General Choi Hong Hi, or Korean history.
---

# ITF lore

The show's plot is the meaning behind the belts and patterns. Fighting is secondary. Accuracy matters because parents and instructors will watch too.

## Source of truth

All facts come from `references/itf/` in this repo:

- `references/itf/README.md`: index and how the files fit together
- `references/itf/patterns.md`: the 24 patterns, movement counts, namesakes, meanings
- `references/itf/belts.md`: belt colours, meanings, gup/dan ranks
- `references/itf/tenets-and-oath.md`: the five tenets and the student oath
- `references/itf/general-choi.md`: General Choi Hong Hi, founder of ITF Taekwondo
- `references/itf/sources.md`: where every fact came from
- `references/itf/terminology.md`: Korean terms with pronunciation
- `references/itf/self-defense-lessons.md`: the numbered lesson library (SD-01 onward), see `self-defense-lessons`
- `references/itf/patterns.json`: machine-readable pattern data (name, korean, moves, belt, namesake, era, moral, tenet, diagram). Prefer this when generating backlogs, on-screen facts, or metadata.

Read the relevant file before writing. If something is not in the references, mark it `[VERIFY]` in the script and leave it off screen until confirmed. Do not invent "ancient legends" and present them as real history. Invented adventures for our characters are fine; they must be clearly our story, inspired by the real meaning.

## Core facts (quick reference, confirm against the references folder)

**Founder:** General Choi Hong Hi (1918-2002), who named Taekwondo in 1955 and founded the International Taekwon-Do Federation (ITF) in 1966. (The name is often misspelled; on screen always write "General Choi Hong Hi".)

**The five tenets:** Courtesy (Ye Ui), Integrity (Yom Chi), Perseverance (In Nae), Self-Control (Guk Gi), Indomitable Spirit (Baekjul Boolgool).

**Belt meanings (ITF):**
- White: innocence, a beginner with no previous knowledge
- Yellow: the earth, from which a plant sprouts and takes root as the foundation is laid
- Green: the plant's growth as skill begins to develop
- Blue: the heaven, towards which the plant matures into a towering tree as training progresses
- Red: danger, cautioning the student to exercise control and warning the opponent to stay away
- Black: the opposite of white, maturity and proficiency, and imperviousness to darkness and fear

This seed-to-tree arc is the backbone of the whole series. Use it.

**The 24 patterns** represent the 24 hours of a day, or one's whole life. Colour belt patterns in order: Chon-Ji, Dan-Gun, Do-San, Won-Hyo, Yul-Gok, Joong-Gun, Toi-Gye, Hwa-Rang, Choong-Moo. Black belt patterns follow (Kwang-Gae, Po-Eun, Ge-Baek, Eui-Am, Choong-Jang, Ko-Dang/Juche, Sam-Il, Yoo-Sin, Choi-Yong, Yon-Gae, Ul-Ji, Moon-Moo, So-San, Se-Jong, Tong-Il). Each is named after a person, event, or idea; the namesake story is the episode's "legend" thread.

## Season map (default)

| Season | Belt journey | Patterns | Big idea |
|--------|--------------|----------|----------|
| 1 | White to Yellow | Chon-Ji, Dan-Gun | Heaven and earth; where a story starts |
| 2 | Yellow to Green | Do-San, Won-Hyo | Patriots and teachers; learning to care for others |
| 3 | Green to Blue | Yul-Gok, Joong-Gun | Wisdom and courage |
| 4 | Blue to Red | Toi-Gye, Hwa-Rang | Scholars and the young warrior-knights |
| 5 | Red to Black | Choong-Moo | Admiral Yi and the turtle ship; never giving up |

## Handling sensitive history (required)

The audience is 6-10. Keep it hopeful and apolitical.

- **War and violence in namesake stories** (e.g. Joong-Gun, Choong-Moo, Kwang-Gae): tell the value (bravery, love of home, never giving up), not the killing. No depictions of assassination, executions, or graphic battle. "He stood up for his people even when it was very hard" is the right register.
- **Japanese occupation and Korean history:** present respectfully without villainising any modern nation or people.
- **Politics around General Choi and the ITF** (North/South Korea, federation splits, Ko-Dang vs Juche): do not include. Present General Choi as the founder who wanted Taekwondo to build good people.
- **Religion and myth** (Dan-Gun and the bear/tiger legend): tell as "an old Korean legend says...", which it is.
- **Federation names and marks:** say "ITF-style Taekwon-Do" in metadata; do not imply endorsement by any federation (see `rights-and-licensing`).

## Turning lore into story

For each pattern or belt episode, pull these from the references and write them into the brief:

1. **The one-sentence meaning** a 7-year-old can repeat.
2. **The namesake story** reduced to one scene with a clear choice and a value.
3. **A number hook** (e.g. "Chon-Ji has 19 movements") for a fun on-screen fact.
4. **The tenet** that the story best demonstrates.
5. **The bridge** to our hero's own problem this episode (the lore mirrors what the kid is going through).

Pronunciation: provide a phonetic guide in the script for every Korean term, for the voice actor/TTS (e.g. Chon-Ji: "chun-jee").
