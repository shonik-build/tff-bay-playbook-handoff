# Content sources — Bay Playbook

Working reference for content that feeds the Bay Playbook website. **Not deployed** — this folder is git-ignored so it stays local and does not end up on Netlify.

**Rule:** the live site is the source of truth for what's published. This folder is the source of truth for what should feed it next.

## Files, in order of authority

| # | File | What it is | Live-site status |
|---|---|---|---|
| 01 | `01-article-tracker.csv` | The article tracker: 35 must-have + good-to-have articles, priority (P0/P1/P2), owner, quality-check state, and stage. Original planning artefact. | Reference only. Priorities set the roadmap. |
| 02 | `02-tff-sf-guide-v1-content.pdf` (+ `.txt`) | **V1 content dump** — a 171-page PDF containing a version of every article on the live site (36 articles, numbered 0–35). "Mostly only the version on Netlify is finalised" per Shonik. Older versions live here. | Content that IS on the site: assumed = live for the finalised ones. Content NOT on the site: needs comparison / porting. |
| 03 | `03-karan-guide.pdf` (+ `.txt`) | **Karan's articles** — 31 pages, deeper drafts across 7 sections: Money/Credit/ITIN, US Banking, Healthcare, Desi Directory, Where to Host Events, Sending Money Home & NRI Banking, Wellness. | May or may not all be incorporated on Netlify. Diff needed. |
| 04 | `04-expert-us-entity-delaware-flip.docx` (+ `.txt`) | **Expert-authored article #5** — US Entity & the Delaware Flip. Includes an ESOP crossover section (Incentiv/Tabulate pricing). Contributor: Indranil Tiwary (Incentiv). | Older draft is on Netlify; expert version is fresher and needs porting. |
| 05 | `05-expert-visas-section-4.pdf` (+ `.txt`) | **Expert-authored article #4** — Visas for Indian Founders. 5 pages, covers B-1 / O-1A / L-1A / H-1B + EB-1A green card, with 2026 fees and per-city consulate wait times. Cites OpenSphere as further-reading source. | Newer than what's on Netlify; needs porting. |
| 06 | `06-meeting-balu-murali-2026-09-03.md` | Feedback call with **Balu Murali** (Sprinto — set up their US ops). Sep 3, 2026. Line-by-line walk-through of the live site by someone who spent 2–3+ years in SF. High signal. | Feedback to apply back to live pages. |
| 07 | `07-meeting-ajay-yadav-2026-09-03.md` | Feedback call with **Ajay Yadav** (neatlogs.com, YC founder). Sep 3, 2026. Also a live walk-through + strong opinions on agent-readable content, missing GTM/hiring depth, and a `skill` framing. | Feedback to apply — but Shonik has flagged GTM/hiring feedback as "nice to have, not must have right now." |

## Structural note — TWO live sites

There are **two live Netlify deployments** that host Bay Playbook content, and they are out of sync with each other:

1. **The main TFF product site**: <https://tff-website.netlify.app/guides/the-bay-playbook/> — 37 slot ToC (00–36), rendered against the V1 content in file #02. This is what Balu and Ajay reviewed. Managed by Suhas/Arnav (not this repo).
2. **Our repo's deployment**: <https://the-bay-playbook.netlify.app/> — 21 pages, DSL/`support.js` architecture, deploys from `main` in this repo. This is a companion/dev version.

The two are DIFFERENT products right now. Any conversation about "what's live" needs to specify which one. Sources 02–07 are all about the TFF-website version — the one visitors and founders actually see.

## Article-level cross-reference

Below: every article slot on the live TFF site (via `/guides/the-bay-playbook/`), the file where its content lives, and any owner/quality flag from the tracker.

| # | Article | V1 PDF | KP Guide | Expert file | Owner (tracker) | Priority |
|---|---|---|---|---|---|---|
| 00 | The 2-Week Scout Trip | ✅ p.1 | — | — | — | P1 |
| 01 | The Move Checklist | ✅ p.127 | — | — | — | P1 |
| 02 | Start With Your Decision | ✅ p.254 | — | — | — | P2 |
| 03 | Reality Check + Who Should NOT Move | ✅ p.374 | — | — | — | P1 |
| 04 | Visas for Indian Founders | ✅ p.491 | — | ✅ #05 (5pg) | Suhas | P0 |
| 05 | US Entity & the Delaware Flip | ✅ p.612 | — | ✅ #04 (Indranil/Incentiv) | Suhas | P0 |
| 06 | Money, Credit & ITIN | ✅ p.738 | ✅ §1 | — | Karan | P0 |
| 07 | Banking & Setting Up US Finances | ✅ p.876 | ✅ §2 | — | Karan | P1 |
| 08 | Healthcare & Insurance | ✅ p.1024 | ✅ §3 | — | Karan | P0 |
| 09 | Housing & Neighborhoods | ✅ p.1148 | — | — | Suhas | P0 |
| 10 | Networking in SF | ✅ p.1435 | — | — | Suhas | P1 |
| 11 | Getting Around SF | ✅ p.1741 | — | — | Shonik | P0 |
| 12 | The Landing Pad Playbook | ✅ p.1851 | — | — | Suhas | P0 |
| 13 | Day 0–7 Checklist | ✅ p.1951 | — | — | Shonik | P1 |
| 14 | Before You Fly: Remote Setup | ✅ p.2037 | — | — | Shonik | — |
| 15 | Apps to Download | ✅ p.2362 | — | — | Suhas | P0 |
| 16 | The Desi Directory | ✅ p.2584 | ✅ §4 | — | Karan & Suhas | P1 |
| 17 | Live Events Calendar | ✅ p.2747 | — | — | Together | P1 |
| 18 | Emergency Contacts & Consulate | ✅ p.2882 | — | — | Shonik | P1 |
| 19 | SF Culture for Indian Founders | ✅ p.3183 | — | — | Shonik | P1 |
| 20 | What To Do on Weekends | (in V1) | — | — | Shonik | P1 |
| 21 | Where to Host Events | ✅ p.3525 | ✅ §5 | — | Karan | P1 |
| 22 | Indian Groceries, Food & American Equivalents | ✅ p.3638 | — | — | Suhas | P1 |
| 23 | Packing + Medications List | ✅ p.3770 | — | — | Suhas | P1 |
| 24 | Moving with Family | ✅ p.3899 | — | — | — | — |
| 25 | Taxes Across the Corridor | ✅ p.4036 | — | — | RallyTax (partner) | P2 |
| 26 | When It Goes Wrong | ✅ p.4162 | — | — | — | — |
| 27 | First 10 US Customers | ✅ p.4299 | — | — | Jellyfish / TripleDart | P1 |
| 28 | Hiring: US vs Keep-Team-in-India | ✅ p.4415 | — | — | Abhay Jani | P2 |
| 29 | Where We Actually Work | ✅ p.4534 | — | — | Suhas & Karan | P1 |
| 30 | Programs & Accelerators — India-Founder Lens | ✅ p.4638 | — | — | Shonik | P1 |
| 31 | SSN, ITIN & Driver's License Walkthroughs | ✅ p.4760 | — | — | Shonik | P1 |
| 32 | Sending Money Home & NRI Banking | ✅ p.4873 | ✅ §6 | — | Karan | — |
| 33 | The SF↔India Travel Playbook | ✅ p.5025 | — | — | Jitesh | P0 |
| 34 | Wellness & Isolation — Done Properly | ✅ p.5150 | ✅ §7 | — | Karan | P2 |
| 35 | The Give-Back Page | ✅ p.5264 | — | — | — | — |
| 36 | Business Banking & Moving Company Money | (not in V1; on live site) | — | — | — | — |

Line numbers refer to the extracted text file `02-tff-sf-guide-v1-content.txt`.

## Key open questions before making changes

1. **Which live site is the target?** The two deployments (`tff-website.netlify.app` vs `the-bay-playbook.netlify.app`) have different architectures and different content. Confirm which one edits should land in — or whether they need to converge.
2. **Expert-authored replacements (#04, #05):** are these the final versions to ship, or drafts still awaiting a review pass? The DOCX for #04 has an Aug 2026 date; the Section 4 PDF for #05 has no date but the fees quote "2026" throughout.
3. **KP Guide integration:** the 7 Karan sections need a diff pass against the live equivalents to see what's already incorporated vs what's missing.
4. **Meeting feedback bucketing:** Balu's feedback is dense and mostly minor tweaks (add refundable-flight tip, mark Tenderloin bold, add car mention, schools footnote for older founders, laptop-theft warning, Louma calendar tie-in). Ajay's core signal is "make it agent-readable / a skill" and the missing GTM+hiring depth (which Shonik explicitly said is nice-to-have, not must-have right now).

## Why this folder is gitignored

The repo publishes to Netlify at the site root. If these files were committed, they would be publicly downloadable at `the-bay-playbook.netlify.app/content-sources/*` — which is wrong for:

- meeting transcripts (named individuals: Balu Murali, Ajay Yadav)
- expert-authored drafts (Indranil / Incentiv, OpenSphere-cited visa doc)
- Karan's original guide (unreviewed for publication)

Keep this folder local unless we make a deliberate decision to publish specific files.
