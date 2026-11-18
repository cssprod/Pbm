---
name: script-writing
description: Write production-ready scripts for the kids ITF Taekwondo anime - dialogue, action lines, timings, on-screen text, pronunciation, and the closing self-defense segment - in a format the storyboard, voice, and edit stages can consume directly. Use after a brief or outline is approved and whenever revising a script.
---

# Script writing

Input: `brief.md` and `outline.md`, plus `series-bible`, `episodes/continuity.md`, and the relevant `references/itf/` files.
Output: `script.md` in the episode folder.

## Format

Use this exact structure so later stages can parse it (each scene has an ID used by storyboard, audio, and edit):

```markdown
# EP001 "The White Belt Seed" (target 4:30)
Tenet: Courtesy | Pattern: Chon-Ji | Safety lesson: SD-01

## SC01 COLD OPEN (0:00-0:08)
[VISUAL] Night. A giant clock glows in the sky. One door creaks open.
[SFX] Deep gong. Wind.
BORI (V.O., whisper): Psst... wanna see something AWESOME?
[TEXT] none

## SC02 KAI'S BEDROOM - MORNING (0:08-0:40)
[VISUAL] Kai leaps out of bed, already in dobok, belt in a knot like a pretzel.
KAI (excited): Today I become a NINJA!
MRS. PARK (O.S., amused): Taekwon-Do, Kai. And first, breakfast.
...
## SC09 SABUM HAN'S SAFETY LESSON (3:50-4:40)
(see self-defense-lessons skill for the required structure)

## PRONUNCIATION
Chon-Ji = CHUN-jee | Sabum-nim = SAH-bum-neem | Dobok = DOH-bok
```

Line types: `[VISUAL]` (what we see, one shot idea per line), `[SFX]`, `[MUSIC]`, `[TEXT]` (on-screen words), and `CHARACTER (direction): line`.

## Dialogue rules for 6-10 year olds

- Sentences of 12 words or fewer. Most lines 3-8 words.
- One idea per line. Kids should never need to rewind to follow.
- Every character sounds different (see bible): Kai = loud, short bursts; Hana = precise facts; Leo = worried questions then jokes; Sabum Han = calm, few words; Bori = boastful then squeaky.
- Use the tenet's name out loud at least once, in context, not as a lecture.
- Korean terms: introduce with meaning the first time ("Chon-Ji, that means Heaven and Earth"), then use freely.
- Names and facts must match `references/itf/` exactly.
- No insults beyond "silly" level. No "stupid", "shut up", "hate".
- Show adults and kids saying please, thank you, and bowing; it's courtesy modelled, not preached.

## Timing

- Spoken English ≈ 2.5 words per second for kids' content (slower than adult). Budget each scene with that.
- Write the target duration in every scene header; total must be within ±10% of target.
- Action-only stretches count too: give them explicit durations.

## Martial arts on screen

- Use correct ITF terms for techniques that appear (e.g. walking stance = gunnun sogi, front kick = ap chagi). If unsure, check `references/itf/terminology.md` or mark `[VERIFY]`.
- Pattern demonstrations show the real opening movements; the animator needs them listed move by move in `[VISUAL]`.
- Any move a child could copy at home is shown safely (space around them, no hitting people, no objects).

## Revision loop

1. Write draft 1.
2. Self-check against the storytelling checklist and the `content-qa` script checklist.
3. Read it aloud at kid pace (count words). Trim anything over time.
4. Set `stage: script` and request script approval from the owner if the episode introduces a new character, a sensitive legend, or a new self-defense topic. Otherwise continue.

## Shorts

Shorts scripts follow the same format but are 75-150 words, one scene or three micro-scenes, with the hook in the first line and on-screen text throughout (many viewers watch muted).
