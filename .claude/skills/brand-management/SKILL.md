---
name: brand-management
description: Keep the show's brand consistent and trustworthy - name, voice, logo and colour system, typography, character usage rules, channel art across YouTube/TikTok/Instagram, and the brand file every other skill reads. Use when creating channel art, writing anything public in the show's voice, approving merch or partner use, or checking whether something is on-brand.
---

# Brand management

The single source of brand truth is `brand/brand.md`. Create it from the template below if it doesn't exist, and keep it current. Other skills read from it (budgets, reviewer names, fonts).

## brand/brand.md template

```markdown
# Brand
Show name: Tiger Belt: The 24 Doors (working title; trademark check pending)
Channel handle(s): @<tbd> (same on YouTube, TikTok, Instagram)
Owner and final approver: Randy
Instructor reviewer (safety lessons, technique): <name, rank, school>
Promise: Exciting anime adventures that teach kids the heart of Taekwon-Do.
Values: the five tenets; kindness over strength; honesty about AI use.
Audience: kids 6-10 (YouTube); their parents (TikTok, Instagram)
Budget per main episode (USD): <set by owner>
Budget per short (USD): <set by owner>
Fonts: Display <bold rounded font with licence>, Body <readable sans>
Colours: Tiger Orange #F28C28, Dojang Cream #FFF4DF, Clock Indigo #1E2357, Door Gold #F5C542, Belt colours per art-direction
Logo files: brand/logo/
```

## Voice

- **To kids (on screen, YouTube titles):** excited, warm, simple. "Let's open the next door!"
- **To parents (descriptions, TikTok, Instagram):** friendly, knowledgeable, reassuring. Mention the values and safety. Never preachy.
- **Never:** sarcastic, fear-based, pushy ("SMASH that subscribe"), or claims of being "official ITF".

## Visual identity

- Logo: a tiger-face badge inside a clock door, with the show name; versions for light and dark, square avatar, and watermark.
- Fonts: licensed for commercial video and print. Record licences in `brand/licences.md`.
- Colour system: brand colours above plus the belt colours (white, yellow, green, blue, red, black) used as the season accent.
- Channel art kit per platform in `brand/channel-art/` (YouTube banner, avatar, watermark; TikTok/Instagram avatar and highlight covers). Same avatar everywhere for recognisability.

## Character usage rules

- Characters always behave per the series bible. Kai never mocks anyone; Sabum Han never loses his temper; Bori may brag but is never mean.
- No character endorses a product directly to kids.
- Merch and partner use require the owner's approval and must keep the model sheets accurate.

## Consistency checks (run in content-qa)

- Correct logo version and placement (watermark bottom-right, small).
- Fonts and colours from the brand file only.
- Title format matches `thumbnails-and-seo`.
- Sign-off line and bow present.

## Reputation

- Respond to parent questions politely within 48 hours on TikTok/Instagram; YouTube MFK comments are off.
- Corrections policy: if a lore fact or technique is wrong, pin a correction (where possible), fix in the next upload's description, and log it in `brand/corrections.md`. Accuracy is the brand.
- Keep the ITF and Korean-heritage community on side: credit General Choi Hong Hi's teachings, invite instructors to review, never claim official status.
