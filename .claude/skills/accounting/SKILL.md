---
name: accounting
description: Bookkeeping for the channel - logging every expense and income line in finance/ledger.csv, tracking AI tool and subscription costs per episode, budgets and alerts, monthly close, and preparing tidy records for tax time. Use whenever money is spent or received, when a budget check is needed, at month end, or when the owner asks what things cost.
---

# Accounting

Not tax advice. The agent keeps clean records; the owner (or their accountant) files taxes.

## The ledger

`finance/ledger.csv` is the single source of truth. Append one row per transaction, immediately when it happens. Never edit or delete past rows; correct with a new reversing row.

```csv
date,type,category,vendor,description,episode,amount_usd,payment_method,receipt,notes
2026-11-18,expense,ai_video,<vendor>,SC02 image-to-video 8s x3,EP001,-4.20,card-1234,receipts/2026-11/xyz.pdf,
2026-11-18,expense,subscription,<vendor>,monthly plan,ALL,-30.00,card-1234,receipts/2026-11/abc.pdf,
2026-12-30,income,ad_revenue,YouTube,December AdSense,ALL,12.34,bank,receipts/2026-12/yt.pdf,
```

Categories (keep to this list so reports work): `ai_image`, `ai_video`, `ai_voice`, `ai_music`, `ai_text`, `subscription`, `voice_talent`, `music_license`, `sfx_license`, `font_license`, `reviewer_fee`, `contractor`, `software`, `hardware`, `ads_promo`, `legal`, `bank_fees`, `other_expense`; income: `ad_revenue`, `partner_fee`, `sponsorship`, `merch_sales`, `printables`, `licensing`, `grant`, `other_income`.

Expenses are negative, income positive. `episode` is `EP###` or `ALL` for shared costs.

Receipts: save to `finance/receipts/YYYY-MM/` (keep this folder out of git if receipts contain personal data; store them in the owner's cloud drive and record the path).

## Budgets and alerts

- Per-episode and monthly budgets come from `brand/brand.md`.
- Before each paid generation batch, sum the episode's spend; if it would pass 80% of budget, note it in `status.yaml`; at 100%, stop and ask the owner.
- Subscriptions: keep `finance/subscriptions.md` (tool, plan, monthly cost, renewal date, what it's used for). Flag tools unused for 30 days for cancellation.

## Monthly close (first working day of each month)

Write `finance/monthly/YYYY-MM.md`:

```markdown
# <Month YYYY>
Income: $ (by category)
Expenses: $ (by category)
Net: $
Cost per main episode this month: $   | per short: $
Over/under budget: 
Subscriptions renewing next month:
Notes / anomalies:
```

A quick summary can be computed with:

```bash
python3 - <<'EOF'
import csv, collections
t = collections.defaultdict(float)
for r in csv.DictReader(open('finance/ledger.csv')):
    if r['date'].startswith('2026-11'):
        t[(r['type'], r['category'])] += float(r['amount_usd'])
for k, v in sorted(t.items()): print(k, round(v, 2))
EOF
```

## Tax-time pack (yearly)

Produce `finance/tax/YYYY.md` with totals by category, list of contractors paid (for any required information returns), list of income sources, and the receipts index. Hand it to the owner/accountant. Note: platform payouts (e.g. AdSense) may require tax forms set up in their dashboards; remind the owner.

## Rules

- Never make purchases, sign up for paid plans, or change billing without the owner's explicit approval.
- No card numbers or bank details in the repo; last 4 digits only.
