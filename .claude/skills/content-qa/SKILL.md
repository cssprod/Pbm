---
name: content-qa
description: Quality and safety gate for every script and finished video - lore accuracy, technique accuracy, child safety, brand consistency, technical specs, accessibility, and a "would a 7-year-old love this?" check including the owner's son as test viewer. Use after the script stage and before any human approval or publishing, and whenever reviewing existing content.
---

# Content QA

Output: `episodes/EP###/qa-report.md`. The episode advances only with `RESULT: PASS`. Any red-line item is an automatic FAIL.

## qa-report.md template

```markdown
# QA EP### <title>  | Reviewer: <agent/human> | Date:
RESULT: PASS | FAIL | PASS WITH NOTES

## A. Script (run after stage 3)
- [ ] Lore facts match references/itf/ (list each fact + file it came from)
- [ ] No [VERIFY] tags left on screen
- [ ] Tenet shown through a choice, not a lecture
- [ ] Self-defense segment follows self-defense-lessons structure; lesson ID: SD-__
- [ ] Sensitive history handled per itf-lore
- [ ] Dialogue ≤12 words per sentence, kid-appropriate words
- [ ] Runtime within ±10% of target

## B. Picture
- [ ] Characters on model (face, hair, belt rank per continuity.md)
- [ ] ITF technique and stances correct in pattern and safety shots (reviewed by: ___)
- [ ] Korean cultural details accurate and respectful
- [ ] No artefacts (hands, faces, text glitches, logos)
- [ ] No flashing > 3 per second; no jump scares

## C. Sound
- [ ] Dialogue intelligible over music
- [ ] Loudness ~-14 LUFS, true peak < -1 dBTP
- [ ] Korean pronunciation correct
- [ ] All music/SFX licensed (listed in brand/licences.md)

## D. Safety and compliance (child-safety-compliance)
- [ ] No red-line content (section 6)
- [ ] Safety lesson instructor sign-off: name, rank, date
- [ ] Disclaimer present on end card and in description
- [ ] MFK setting planned; no data collection; no off-platform calls to action for kids
- [ ] AI disclosure line in description

## E. Brand and packaging
- [ ] Logo, fonts, colours correct
- [ ] Title/thumbnail honest and on-format
- [ ] Captions accurate and synced (.srt + burned-in for vertical)
- [ ] Specs per episode-formats for every deliverable

## F. Kid test
- [ ] Shown to the test viewer (owner's son) by the owner; reactions noted below
- Where did he laugh? Where did he look away? Could he say the lesson afterwards? Did he try the safety move?

## Notes / fixes required
```

## How to run

1. Run section A immediately after the script is drafted, before any money is spent on generation.
2. Run B-E on the rough cut and again on the final.
3. Section F is done by the owner. The agent prepares a private link and three questions, and records the answers the owner shares. The agent never directly interacts with or records the child.
4. On FAIL: list fixes with owner skill, set `blockers` in status.yaml, loop back to the right stage. Two FAILs on the same issue: escalate to the owner.

## Lessons log

After each episode, add any recurring issue to `episodes/qa-lessons.md` and update the relevant skill if a rule was missing.
