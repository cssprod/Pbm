---
name: video-editing
description: Assemble generated clips, voice, music, and graphics into finished masters for YouTube (16:9) and vertical platforms (9:16), including captions, on-screen text, the recurring segment graphics, end screens, and scripted ffmpeg renders. Use when editing, re-cutting, captioning, or rendering an episode or short.
---

# Video editing and assembly

Input: approved clips in `assets/`, stems in `audio/`, `script.md` (scene IDs and timings).
Output: `deliverables/EP###_youtube_16x9.mp4`, `EP###_short_<n>_9x16.mp4`, captions `.srt`, and `edit/edl.md`.

## Edit order

1. **Radio cut:** lay dialogue and narration first, to the script timings.
2. **Picture:** drop clips per scene/shot ID. Trim to action; hold key martial-arts poses 0.5 s.
3. **Recurring graphics** (from `brand/graphics/`): title sting, Great Clock door transition, Bori's Fact card, Safety Lesson title, safety reminder card, sign-off bow, end screen.
4. **Music and SFX:** music under, SFX on actions.
5. **On-screen text:** facts, Korean terms with meaning, lesson chant. Big, short, on screen ≥ 2 s per 5 words.
6. **Captions:** generate from the script (not ASR) and align. Export `.srt`.
7. **Colour pass:** match shots within a scene.
8. **Render** masters, then verticals (see `episode-formats`).

## Automated assembly (ffmpeg)

For automation, keep an `edit/edl.md` (or `edl.json`) listing each shot's file, in/out points, and audio. A simple assembly:

```bash
# concat list: file 'SC01-SH01_v2.mp4' etc. (all same codec/fps/resolution)
ffmpeg -f concat -safe 0 -i edit/concat.txt -i audio/mix.wav \
  -map 0:v -map 1:a -c:v libx264 -preset slow -crf 18 -pix_fmt yuv420p \
  -r 24 -c:a aac -b:a 192k -movflags +faststart deliverables/EP001_youtube_16x9.mp4

# loudness normalise to -14 LUFS
ffmpeg -i in.mp4 -af loudnorm=I=-14:TP=-1:LRA=11 -c:v copy out.mp4

# burn captions for vertical
ffmpeg -i short.mp4 -vf "subtitles=short.srt:force_style='FontName=<BrandFont>,FontSize=18,Outline=2,Alignment=2,MarginV=320'" -c:a copy short_captioned.mp4
```

Normalise all clips first (`-r 24`, same resolution, `yuv420p`) so concat works. For complex edits (titles, keyframed graphics), use a project in an NLE (DaVinci Resolve, Premiere, CapCut desktop) or a code-driven editor (e.g. Remotion, MoviePy) and save the project in `edit/`.

## Pacing guide (6-10 year olds)

- Average shot 2-5 s in action, up to 8 s in calm talk.
- New visual idea at least every 10 s.
- No flashing or strobing (no more than 3 flashes per second, avoid saturated red flashes) to protect photosensitive viewers.
- Avoid sudden loud stings.

## End screen (YouTube)

Videos set to Made for Kids cannot use YouTube cards or end screens (confirm against current YouTube help). So build the "what's next" into the video itself: a 5-8 s in-video teaser of the next door opening ("Next time: the Yellow Door!"), with no clickable elements and no "subscribe" pressure aimed at kids. Organise episodes into season playlists so autoplay does the work.

## Hand-off

When renders are done, update `status.yaml` to `stage: package` and list deliverable paths. Keep the final masters and project files; delete unused generations only after the episode is published and approved (they cost money to regenerate).
