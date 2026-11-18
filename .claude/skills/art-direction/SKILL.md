---
name: art-direction
description: Visual style guide and storyboarding for the kids ITF Taekwondo anime - the high-quality realistic anime look, character model sheets, colour scripts tied to belt colours, shot language, accurate Korean and Taekwon-Do details, and how to write consistent image/video generation prompts. Use when designing characters or locations, storyboarding, writing generation prompts, or reviewing visuals.
---

# Art direction

## The look

**High-quality, realistic anime:** cinematic lighting, detailed backgrounds, expressive but grounded faces, believable martial arts motion. Reference qualities (describe qualities, never name living artists or studios in prompts): painterly skies, soft volumetric light, clean line art, rich colour, film-like depth of field.

Kid-friendly guardrails: big readable expressions, bright palette in the real world, slightly more mysterious (never horror) palette in the legend world. The Gloom is a soft purple-grey fog with glowing eyes: spooky-cute, not frightening.

## Colour script

The belt colours drive colour mood (and align with the ITF meanings in `itf-lore`):

| World / moment | Palette |
|----------------|---------|
| Dojang (real world) | Warm wood, cream walls, morning gold |
| Great Clock | Deep indigo night, gold door glow |
| White belt episodes | Pale dawn, snow, seed motif |
| Yellow | Earth tones, wheat, sunrise |
| Green | Spring forest, new leaves |
| Blue | Open sky, mountains, clouds |
| Red | Sunset, red blossoms, caution |
| Black | Night sky with stars: strong, calm, unafraid |
| The Gloom | Desaturated purple-grey; colour returns as it shrinks |

## Character model sheets

Each main character needs `brand/characters/<name>/` containing: turnaround (front, 3/4, side, back), expression sheet (8 expressions), dobok and belt details, colour swatches with hex, height chart against other cast, and **one canonical reference image** used in every generation prompt. Lock these before Season 1 production; changing a design mid-season breaks consistency.

Taekwon-Do accuracy:
- ITF dobok: white, V-neck jacket with black trim on black belt uniforms only, ITF-style back logo only if licensed (otherwise a plain back or our own show emblem; see `rights-and-licensing`).
- Belt tied in the correct ITF knot, ends equal length.
- Bare feet on the dojang floor; bow when entering and leaving.
- Stances must look like real ITF stances (walking stance length ~1.5 shoulder widths). Use reference footage of real patterns for motion.

Korean culture accuracy: hanbok, architecture (hanok, palace roofs), historical armour, and the turtle ship should be researched from museum references for the right era; record references in `brand/visual-references.md`.

## Shot language

- Establishing wide, then mediums, then close-ups for emotion. Kids follow geography easily if every new location starts wide.
- Action: clear silhouettes, one move per shot, hold the final pose 0.5 s (kids need to see the move to learn it).
- Pattern demos: full-body, front or 45°, locked camera, no fast cuts.
- Safety lesson: Sabum Han full-body front, then side; arrows/graphics overlaid.
- Shot duration: 2-5 s average in action, 4-8 s in talk.

## Storyboard format (`storyboard.md`)

```markdown
## SC02-SH03 (3.0 s) MEDIUM, eye level, slight push-in
Action: Kai tugs his pretzel-knotted belt; Bori pops out of the knot.
Characters: kai_v1, bori_v1 | Location: kai_bedroom_v1 | Time: morning
Image prompt: <see template>
Motion prompt: belt wiggles, small tiger cub springs up, Kai's eyes widen, slight camera push
Audio cue: SFX pop, Bori "Ta-daaa!"
```

## Prompt template

```
[STYLE BLOCK - identical every time]
high-quality cinematic anime illustration, clean line art, soft volumetric lighting,
detailed painted background, vibrant but natural colours, child-friendly, 16:9

[CHARACTER BLOCK - from the character's sheet, identical every time]
Kai: 8-year-old boy, spiky black hair, warm brown eyes, white ITF-style dobok,
white belt tied in a slightly messy knot, energetic expression

[SHOT BLOCK]
medium shot, eye level, Kai in his bedroom at morning, tugging his belt,
a tiny glowing orange tiger cub spirit popping out of the knot

[NEGATIVE / AVOID]
no text, no logos, no weapons, no blood, no scary faces, no extra fingers, no realistic gore
```

Keep the style and character blocks in `brand/prompt-blocks.md` and paste them verbatim. Use the generator's character/style reference features with the canonical images on every shot.
