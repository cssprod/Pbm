---
name: video-generation
description: Turn an approved storyboard into consistent, high-quality anime video clips with AI image and video generators - tool selection, keyframe-first workflow, character consistency, motion prompting, lip-sync, retries, cost control, and file naming. Use when generating, regenerating, or upscaling any visual asset for an episode.
---

# Video generation

Input: `storyboard.md`, `brand/prompt-blocks.md`, canonical character images in `brand/characters/`.
Output: clips in `episodes/EP###/assets/` named `SC02-SH03_v1.mp4` (and keyframes `SC02-SH03_kf_v1.png`).

## Tool choice

The AI video market changes monthly. At the start of each season (and when a tool fails you), re-evaluate and record the choice and date in `brand/toolstack.md`. Evaluate on:

1. **Commercial use rights** for generated output (must allow monetised YouTube use; see `rights-and-licensing`).
2. **Character consistency** (reference-image or character features, or custom fine-tunes/LoRAs).
3. **Image-to-video quality** for anime style and martial-arts motion.
4. **Clip length and resolution** (aim for 5-10 s clips at 1080p+).
5. **API access** for automation (see `ai-automation`), and price per second of output.
6. **Content policy** compatibility with depictions of children and martial arts.

Typical stack categories: an image model for keyframes, an image-to-video model for motion, a lip-sync tool for dialogue shots, an upscaler/frame interpolator, and optionally a 3D or pose tool for complex pattern choreography. Run a 10-shot bake-off with the same storyboard before committing; save the results in `brand/bakeoffs/`.

## Workflow: keyframes first

1. **Generate keyframes** (still images) for every shot from the prompt template in `art-direction`, always attaching the canonical character reference(s). Generate 2-4 options per shot.
2. **Pick and fix**: choose the best, inpaint fixes (hands, belt knot, dobok details). Check against the model sheet.
3. **Approve keyframes in a contact sheet** (`assets/contact_SC##.png`) before spending on video. This is the cheapest place to catch problems.
4. **Animate** each approved keyframe with image-to-video using the shot's motion prompt. Use start and end frames when the tool supports it, for controlled moves.
5. **Lip-sync** dialogue close-ups after audio is recorded (see `voice-and-music`); medium/wide shots can rely on simple mouth flaps or cut-aways.
6. **Upscale / interpolate** only the selected takes to final resolution.

## Martial-arts motion

Generators often get technique wrong. For pattern demos and safety lessons:
- Use reference video of the real movement (filmed by an instructor or from a licensed source) as motion guidance where the tool supports video-to-video or pose control.
- Otherwise, break each move into separate short shots (chamber pose, then completed pose) and cut between them.
- Every pattern and safety shot must be checked by someone who knows ITF technique (see `content-qa`).

## Consistency checklist (per shot)

- Face, hair, eye colour match the sheet.
- Belt colour and knot correct for the character's current rank (check `episodes/continuity.md`).
- Dobok correct, no random logos or text.
- Correct number of fingers and toes; bare feet on the dojang floor.
- Lighting matches neighbouring shots in the scene.

## Retries and cost control

- Max 4 video generations per shot. After that, simplify the shot (fewer characters, less motion) or flag it in status.yaml.
- Keep a per-episode generation budget in `status.yaml` (default: set by the owner in `brand/brand.md`). Stop and ask before exceeding it.
- Log every paid job to `finance/ledger.csv` (tool, shot, seconds, cost).
- Reuse: establishing shots, the Great Clock door sequence, title sting, and Bori's Fact frame are generated once and reused all season.

## Safety and policy

- Never generate realistic depictions of real children, and never use photos of the owner's son or any real child as input.
- No real people's likeness except historical figures depicted respectfully in stylised form.
- Enable and keep the platform's AI-content metadata (e.g. C2PA) where provided; disclose AI-generated content when publishing (see `social-media-management`).
