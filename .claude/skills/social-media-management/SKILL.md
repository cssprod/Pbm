---
name: social-media-management
description: Plan, schedule, publish, and manage the show's YouTube, TikTok, and Instagram accounts - content calendar, upload settings (Made for Kids, AI disclosure), the human approval gate before anything goes public, community moderation, and cross-promotion. Use when scheduling or publishing posts, setting up accounts, planning the calendar, or handling comments and messages.
---

# Social media management

## The approval gate (required)

The agent **prepares** posts; a human **publishes**. Concretely:

1. Upload as **private** (YouTube) or save as **draft** (TikTok/Instagram) with all metadata filled in.
2. Write `episodes/EP###/approval.md` with: links to the private/draft posts, the QA report summary, the costs, and a checklist for the owner.
3. Wait for the owner to write `APPROVED <name> <date>` in `approval.md` (or approve in chat). Record it in `status.yaml` under `approvals.publish`.
4. Only then schedule or make public. If the owner has explicitly enabled scheduled publishing for a given post, the agent may set the scheduled time; otherwise the owner presses publish.

Never change an account's settings, delete content, reply to messages as the brand, or post anything not in an approved package without the owner's go-ahead.

## Upload settings checklist

**YouTube**
- Audience: **Yes, it's made for kids** (channel default too).
- Altered/synthetic content: set per `child-safety-compliance` (disclose in description regardless).
- Paid promotion: tick if any sponsor.
- Category: Education (or Film & Animation; keep consistent).
- Language and caption language: set; upload the .srt.
- Playlist: the season playlist plus a topic playlist.
- Thumbnail, title, description, chapters, tags from `metadata/youtube.md`.
- License: Standard YouTube.

**TikTok** (account 13+, run by the owner, aimed at parents)
- Caption from `metadata/tiktok.md`, AI-generated content label on, branded content toggle if sponsored.
- Comments filtered; duets/stitches limited if kids appear to engage.

**Instagram Reels** (same as TikTok)
- Caption, cover, AI label where applicable, share to feed on, location off.

## Content calendar

Keep `social/calendar.md` (a table: date, platform, asset, status, link). Default weekly rhythm (adjust per `analytics-and-growth`):

| Day | YouTube | TikTok | Instagram |
|-----|---------|--------|-----------|
| Mon | | Safety lesson clip | Safety lesson clip |
| Wed | Short: legend in 45 | Legend clip | Carousel: belt meaning |
| Fri (every 2 weeks) | Main episode | Trailer for episode | Reel trailer |
| Sat | Short: Bori's Fact | Bori's Fact | Story: behind the scenes |

Post times: weekend mornings and after-school hours in the main audience's time zone; test and refine.

## Community management

- **YouTube:** comments are disabled on MFK content; nothing to moderate there. Don't try to re-enable them.
- **TikTok/Instagram:** check comments daily. Reply only to parents/adults with friendly, short answers drafted for approval until the owner allows routine replies. Hide spam, mean, or inappropriate comments. Never reply to or engage with accounts that appear to belong to children beyond hiding inappropriate content. Escalate any safety concern per `child-safety-compliance` section 8.
- Save useful parent feedback to `analytics/feedback.md`.

## Cross-promotion

- Every short ends with a soft "Full adventure on YouTube" card (no clickable kid-targeted links).
- Instagram/TikTok bios: link to the YouTube channel only.
- Partner with Taekwon-Do schools (see `business-strategy`) by giving them shareable clips; they post on their own accounts.

## Account security

- 2FA on every account; owner holds the recovery codes.
- API tokens for automation live in environment secrets, never in the repo (see `ai-automation`).
