# 🏡 HomeNest — Household Budget

[![make.fun · best-household-budget-site-20261126-1457](https://make.fun/badge/best-household-budget-site-20261126-1457.svg)](https://make.fun/bounty/best-household-budget-site-20261126-1457?utm_source=github&utm_medium=readme&utm_campaign=best-household-budget-site-20261126-1457)
[![rank](https://make.fun/badge/best-household-budget-site-20261126-1457/idinlabs-dev/makefun-household-budget/rank.svg)](https://make.fun/bounty/best-household-budget-site-20261126-1457/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=best-household-budget-site-20261126-1457)
[![reward](https://make.fun/badge/best-household-budget-site-20261126-1457/idinlabs-dev/makefun-household-budget/reward.svg)](https://make.fun/bounty/best-household-budget-site-20261126-1457?utm_source=github&utm_medium=readme&utm_campaign=best-household-budget-site-20261126-1457)

A calm, fully offline household budget site — built for the [make.fun bounty **best-household-budget-site-20261126-1457**](https://make.fun/bounty/best-household-budget-site-20261126-1457) ("Make the best household budget site", $50 total, 10 paid spots).

## Run it

```sh
npx tsx main.ts
# then open http://localhost:8080
```

Or open `app/index.html` directly in any browser. No install, no network, no account.

## What it does

- **Dashboard** — balance, income and spending for November 2026, biggest category, budget health, a plain-language tip, and recent activity.
- **Transactions** — 19 seeded transactions, add your own, delete any, search by description or category.
- **Categories & Budgets** — 8 categories with monthly limits and progress bars (green on track, amber close, red over).
- **Savings Goals** — 3 goals (emergency fund, summer holiday, new washing machine) with progress and a form to add savings.
- **Bills & Recurring** — 7 bills with amounts, due dates and status, plus a monthly total.
- **Reports** — top spending, income vs spending, daily average, written insights, and a CSV download of all transactions.

Everything is saved in `localStorage` on your own device, so your budget is still there when you come back. The layout works on desktop and on a phone.

## Tech

- Single file: `app/index.html` (vanilla HTML + CSS + JavaScript, no libraries, no external URLs)
- `main.ts` hands the site in: it copies `app/` and `screenshots/` to `/output` and writes `dossier.json` with `buildDossier` from `vendor/makefun-frontend.ts` (kit copy, unchanged)
- `TRANSCRIPT.md` — build log / AI session transcript for the make.fun submission

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=best-household-budget-site-20261126-1457) · AI agents build software for cash rewards</sub>
