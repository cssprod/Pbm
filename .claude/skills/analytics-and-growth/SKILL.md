---
name: analytics-and-growth
description: Measure what kids and parents actually watch and use it to steer the show - YouTube Analytics retention and traffic, TikTok/Instagram insights, a weekly report, experiments, and feeding learnings back into story, format, and calendar decisions. Use for weekly reviews, after each release, when choosing the next topics, or when growth stalls.
---

# Analytics and growth

Output: `analytics/weekly/YYYY-MM-DD.md`, `analytics/experiments.md`, and updates to `episodes/backlog.md`.

## Metrics that matter (in order)

1. **Audience retention** (YouTube): average percentage viewed, and the retention curve. Dips tell you exactly which scene lost them.
2. **Returning viewers and playlist/autoplay views:** are kids coming back for the next door?
3. **Views from Browse/Suggested vs Search:** shows whether YouTube is recommending us.
4. **CTR on impressions:** thumbnail/title effectiveness (compare within our channel; kids' CTR norms differ).
5. **Shorts:** viewed vs swiped-away rate; percent who watched to the end and looped.
6. **TikTok/Instagram:** saves and shares (parents saving a safety lesson is our best signal), follows, profile-to-YouTube clicks where measurable.
7. **The test viewer:** the owner's son's reactions (from content-qa section F). Weight this heavily early on.

Note that MFK videos have limited data (no comments, restricted personalised features); rely on retention and traffic sources.

## Weekly report template

```markdown
# Week of <date>
Headline: <one sentence>
Top video: <title> - <views>, <avg % viewed>
Retention dips: <video, timestamp, what happened on screen, hypothesis>
Best short per platform:
Shares/saves on parent platforms:
Test viewer notes:
Spend this week (from finance/ledger.csv): $
Next week: <3 concrete changes>
```

## Turning data into decisions

- A scene type that repeatedly causes a dip (e.g. long legend narration) -> update `storytelling` beat timings.
- A safety lesson short outperforming -> make more safety shorts; consider a "Safety Lessons" spin-off playlist.
- A belt or pattern question appearing in parent comments -> add it to the backlog.
- Thumbnail tests -> record the winning patterns in `thumbnails-and-seo` notes.

## Experiments

Run one experiment at a time per platform for 2-3 weeks. Log in `analytics/experiments.md`: hypothesis, change, metric, result, decision. Examples: episode length 4 vs 6 min; cold open with Bori vs action; post time morning vs after school.

## Data access

Use the YouTube Analytics API and platform insights exports (see `ai-automation` for credentials). If no API access is configured, ask the owner for a CSV export each week and store it in `analytics/raw/` (exclude it from the repo if it contains anything private).
