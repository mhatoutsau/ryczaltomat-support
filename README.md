# Kalkulator Ryczaltu — Support

**A privacy-first, offline-first lump-sum tax calculator for Polish sole proprietors (JDG).**

👉 **Open the app: [Calculator app](https://ryczaltomat.app/)**

This repository is the **support hub** for the app. The source code is not public — you do not need a GitHub account to use the calculator, and nothing about your data ever touches GitHub.

| I want to… | Go to |
|---|---|
| Report a bug | [**Issues**](../../issues) |
| Ask how something works / request a feature | [**Discussions**](../../discussions) |
| Use the app | [**Calculator app**](https://ryczaltomat.app/) |

---

## What the app does

- **PIT (Ryczałt)** — lump-sum income tax across 9 brackets (3%–17%), applied to net revenue with proportional social/health insurance deductions.
- **ZUS** — social and health contributions, with the relief scheme pipeline handled automatically:
  - *Ulga na Start* — 6 months, zero social
  - *Preferencyjne ZUS* — 24 months, reduced base (30% of the minimum wage)
  - *Mały ZUS Plus* — 36 months, income-proportional base
  - *Duży ZUS* — standard, full rates
  - *ZUS holiday* — 1 month/year without social contributions
- **VAT** — all Polish rates (23%, 8%, 5%, 0%, zw, np), reverse charge for imported services, 50% auto-deduction for mixed-use vehicles, monthly or quarterly filing.
- **PKD codes** — built-in registry with localized names and associated rates.
- **Fleet** — company cars with usage type (mixed / business) and engine type (ICE / hybrid / electric), linked to expenses for VAT purposes.
- **Expenses & periods** — per-period expense entries with VAT breakdown, browsable and editable history, YTD cumulative summaries.
- **Analytics** — revenue, tax and ZUS trends across periods.
- **PDF export** — printable reports via jsPDF.
- **Languages** — Polish (default), English, Russian, Ukrainian, Belarusian.
- **Themes** — 4 palettes plus dark mode.

## Privacy & data

- **No backend, no accounts, no login, no telemetry, no analytics.**
- Everything you enter is stored **only in your browser** (IndexedDB).
- The app works fully offline once loaded.
- Clearing site data / browser cache / using private mode **deletes your history permanently**. There is no cloud backup and no sync — export a PDF before wiping.

## Before you open an issue — known limitations

Please check these first; they're known behaviour, not bugs:

- Tax law changes (rates, brackets, ZUS minimum wage, VAT limits) are only as current as the last update — always cross-check against [gov.pl](https://www.gov.pl) or your accountant.
- Calculations assume a single business, one tax year, and no joint/spouse income, foreign income, or IP-box — those cases are not supported.
- Data does not move between browsers or devices. Copy/paste of periods is not implemented; use PDF export.
- Progressive/instalment payments (raty PIT/ZUS) are not calculated — the app shows the period totals you owe.
- The app is **not** an accounting ledger and cannot file declarations with the tax office.

## How to file a good bug report

1. Search existing issues first — the bug may already be tracked.
2. Open a new issue and include:
   - **App version** (bottom of Settings → About) and **browser + OS**
   - **Language** of the UI
   - **What you did**, step by step
   - **What you expected** vs **what happened**
   - **Screenshot** (screenshot or paste directly into the issue)
   - **The numbers** — the period (YYYY-MM), revenue, expenses, business start date, chosen reliefs, PKD codes — anonymized if you prefer, but enough to reproduce
3. Don't include real company names, NIP, addresses, or any personal data. Replace them with placeholders.

Do **not** paste your full IndexedDB export or a screenshot containing genuine financial data unless you're comfortable sharing it publicly.

## Discussions — good topics

- "How is X computed?" (quote the formula shown in the app)
- Feature requests and workflow ideas
- Which PKD code / relief scheme fits a given situation
- UX friction, translations, themes, PDF layout
- Ideas for better explanations inside the app

Search existing topics before starting a new one — questions like these get asked more than once.

## Scope of support

This is a **community support** repository. The maintainer reads issues and discussions, but:

- ❌ **No tax, legal or accounting advice.** Use a licensed tax adviser (`doradca podatkowy`) or your accountant. Always verify results against official sources.
- ❌ **No priority support, SLAs or guaranteed response times.**
- ✅ **No support for the tax office, ZUS, or gov.pl portals** — those are separate systems.
- ✅ Bug reports, translation corrections, and reproducible crashes are welcome and get fixed.

## Responsible reporting

Security or privacy issues: open an issue but mark it clearly as sensitive with minimal reproduction details, or contact the maintainer privately if a public thread would expose data. Responsible disclosure is appreciated.

## License

This repository contains documentation only and is released under the same terms as the application. The calculator itself is provided as-is, without warranty of any kind.
