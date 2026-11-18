---
name: voice-and-music
description: Voice casting, AI or human voice-over, pronunciation of Korean terms, theme song, background music, and sound effects for the kids ITF Taekwondo anime, with licensing and loudness rules. Use when recording or generating dialogue, choosing or composing music, building the sound library, or mixing audio.
---

# Voice and music

Output goes to `episodes/EP###/audio/`: `dialogue/SC02_KAI_01.wav`, `music/`, `sfx/`, and a `mix.wav` stem set (dialogue, music, effects) for the editor.

## Voices

| Character | Voice brief |
|-----------|-------------|
| Kai | Bright, energetic 8-year-old boy, fast when excited, cracks when nervous |
| Bori | Small, squeaky, dramatic; tries to sound big and fails |
| Hana | Clear, precise 9-year-old girl, slightly faster when explaining facts |
| Leo | Younger, softer, rising "uh-oh" intonation, great comic timing |
| Sabum Han | Warm, low, calm adult male; slight Korean accent only if voiced by a Korean speaker; never a caricature |
| Mrs. Park | Gentle grandmother storyteller; legends read in a slower "once upon a time" cadence |
| The Gloom | Breathy whisper, soft, more sneaky than scary |

Options, in order of preference as budget allows:
1. **Human voice actors** (union or freelance) for main cast, recorded remotely. Best quality and best for brand trust.
2. **AI voices from a licensed provider** with commercial rights and consenting voice talent. Never clone a real person's voice without written consent. Never clone a child's voice.
3. Mixed: human for Sabum Han and Kai, AI for minor characters.

Record the chosen voice IDs/actors and their licences in `brand/voices.md` so every episode uses the same voices.

## Pronunciation

Every script has a `## PRONUNCIATION` block. Feed phonetic spellings (or SSML phonemes where supported) to TTS. Have a Korean speaker check Korean terms at least once per season; log corrections in `references/itf/terminology.md`.

## Music

- **Theme song** (15 s intro, 30 s full version, instrumental end-card version): energetic, taiko-and-gayageum-inspired drums with modern synths, a catchy chant of the tenets. Must be original and owned or exclusively licensed.
- **Background cues:** a library of 10-15 cues per season: dojang (warm), adventure (driving), legend (traditional Korean instruments, e.g. gayageum, daegeum, janggu), Gloom (mysterious, not scary), victory, comedy, safety lesson (calm, upbeat).
- **Sources:** commission a composer, use AI music generators whose terms grant commercial rights, or use royalty-free libraries whose licence covers YouTube monetisation. Avoid anything that triggers Content ID claims on our own channel; register owned music carefully (claiming our own music can block others' fair use and cause disputes; get advice first).
- Never use popular songs or trending TikTok sounds in the YouTube episodes. On TikTok/Instagram, platform-licensed sounds are fine only inside those apps and only if appropriate for kids.

Log every track with source, licence, and proof in `brand/music-licences.md`.

## Sound effects

Build a reusable `brand/sfx/` library: belt snap, dobok swish, kihap ("ki-YAP"), door gong, Bori's squeak-roar, Gloom whoosh, Clock tick. Use licensed SFX libraries or generate with a tool that grants commercial rights.

## Mix

- Dialogue always clearly above music (music around -18 to -24 dB under speech).
- Final loudness ~-14 LUFS integrated, true peak under -1 dBTP.
- Kihaps and impacts punchy but not startling; no sudden loud noises (kids often watch with headphones).
