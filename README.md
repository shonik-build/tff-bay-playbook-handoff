# The Bay Playbook — v1 Content Package

Drop-in content for `thefounderfolks.com/guides/the-bay-playbook`. 28 article pages, one landing page, source files, and a UX-audit annotation bundle.

## What's here

```
├── HANDOFF.md              ← audit findings + how the package is structured (read first)
├── design-system.md        ← tokens, fonts, layout rules
├── content/                ← plain-text brief per page (edit these for copy changes)
├── pages/                  ← .dc.html files matching the existing template (drop into repo root)
├── sources/                ← raw sources this content was built from
└── screenshots/            ← annotated audit screenshots
```

## How to preview locally

The `.dc.html` files are self-contained — they load a runtime (`pages/support.js`) that turns them into React pages at runtime. To preview:

```bash
cd pages
python3 -m http.server 8000
# open http://localhost:8000/Bay%20Playbook%20Landing%20v2.dc.html
```

No build step. Netlify serves these files directly.

## How the templates work (2-minute version)

- Each `.dc.html` is HTML with a custom `<x-dc>` root and `{ placeholder }` template syntax.
- Loops: `<sc-for list="{ arr }" as="item">…</sc-for>`
- Conditionals: `<sc-if test="{ expr }">…</sc-if>`
- Computed values come from a `renderVals()` function at the bottom of each page (small script block).
- Persistent UI state (e.g. "which visa did I pick") lives in `localStorage` under `bp-*` keys.

If you're editing **only copy**, you never touch the script block — just edit the visible text between HTML tags.

## The 28 v1 pages

| # | Page | Section | Length | Content brief |
| --- | --- | --- | --- | --- |
| 01 | Reality Check + Who Should NOT Move | S0 · DECIDING | ~2012 words | [`content/01-reality-check.md`](content/01-reality-check.md) |
| 02 | Start With Your Decision | S1 · BEFORE YOU FLY | ~435 words | [`content/02-decisions.md`](content/02-decisions.md) |
| 03 | The 2-week scout trip, from India | S1 · BEFORE YOU FLY | ~2057 words | [`content/03-scout-trip.md`](content/03-scout-trip.md) |
| 04 | Moving with family | S1 · BEFORE YOU FLY | ~2119 words | [`content/04-moving-with-family.md`](content/04-moving-with-family.md) |
| 05 | Visas for Indian Founders | S1 · BEFORE YOU FLY | ~3276 words | [`content/05-visas.md`](content/05-visas.md) |
| 06 | Packing & What to Ship | S1 · BEFORE YOU FLY | ~3074 words | [`content/06-packing.md`](content/06-packing.md) |
| 07 | US Entity & the Delaware Flip | BUSINESS · YOUR COMPANY | ~3512 words | [`content/07-entity-delaware-flip.md`](content/07-entity-delaware-flip.md) |
| 08 | Business banking & moving company money | BUSINESS · YOUR COMPANY | ~3070 words | [`content/08-business-banking.md`](content/08-business-banking.md) |
| 09 | Accelerators (YC / a16z / Neo) | BUSINESS · YOUR COMPANY | ~5127 words | [`content/09-accelerators.md`](content/09-accelerators.md) |
| 10 | SSN, ITIN & Driver's Licence | S2 · GET YOUR US IDs | ~5239 words | [`content/10-ssn-itin-license.md`](content/10-ssn-itin-license.md) |
| 11 | Money & Credit | S3 · MONEY & CREDIT | ~3695 words | [`content/11-money.md`](content/11-money.md) |
| 12 | Send Money Home / NRI Banking | S3 · MONEY & CREDIT | ~3740 words | [`content/12-nri-banking.md`](content/12-nri-banking.md) |
| 13 | Landing Pad (first 1–4 weeks) | S4 · LANDING | ~1301 words | [`content/13-landing-pad.md`](content/13-landing-pad.md) |
| 14 | Day 07 Checklist | S4 · LANDING | ~1206 words | [`content/14-day-07.md`](content/14-day-07.md) |
| 15 | SIM + Phone | S4 · LANDING | ~1413 words | [`content/15-sim-phone.md`](content/15-sim-phone.md) |
| 16 | Housing & Neighborhoods | S4 · LANDING | ~4497 words | [`content/16-housing.md`](content/16-housing.md) |
| 17 | Healthcare & Insurance | S4 · LANDING | ~2760 words | [`content/17-healthcare.md`](content/17-healthcare.md) |
| 18 | Getting Around SF | S4 · LANDING | ~2459 words | [`content/18-getting-around.md`](content/18-getting-around.md) |
| 19 | Apps to Install Day 1 | S4 · LANDING | ~3804 words | [`content/19-apps.md`](content/19-apps.md) |
| 20 | Networking in SF | S5 · LIVE IN IT | ~4028 words | [`content/20-networking.md`](content/20-networking.md) |
| 21 | Live events calendar | S5 · LIVE IN IT | ~1275 words | [`content/21-live-events.md`](content/21-live-events.md) |
| 22 | Groceries & Cooking | S5 · LIVE IN IT | ~2951 words | [`content/22-groceries.md`](content/22-groceries.md) |
| 23 | Weekends & Escapes | S5 · LIVE IN IT | ~5640 words | [`content/23-weekends.md`](content/23-weekends.md) |
| 24 | Remote Team Setup | S5 · LIVE IN IT | ~3495 words | [`content/24-remote-setup.md`](content/24-remote-setup.md) |
| 25 | Culture Shocks | S5 · LIVE IN IT | ~3629 words | [`content/25-culture.md`](content/25-culture.md) |
| 26 | SF ↔ India Travel | S5 · LIVE IN IT | ~1958 words | [`content/26-sf-india-travel.md`](content/26-sf-india-travel.md) |
| 27 | Emergency Contacts | S5 · LIVE IN IT | ~3445 words | [`content/27-emergency.md`](content/27-emergency.md) |
| 28 | Founder Directory | S5 · LIVE IN IT | ~1415 words | [`content/28-directory.md`](content/28-directory.md) |

## Deploying

The live site pulls from Arnob's repo. To ship these:

1. Copy `pages/*.dc.html` into the live repo's article directory.
2. Update the sidebar `navGroups` in each `.dc.html` — same nav is repeated across all pages (yes, this is redundant; consolidating it into a shared JS module is a future refactor).
3. Update the landing page (`Bay Playbook Landing v2.dc.html`) to reflect the 28-page TOC.
4. Push — Netlify auto-deploys from `main`.

## Attribution

Built by Shonik. Sources acknowledged in `sources/INDEX.md`.
