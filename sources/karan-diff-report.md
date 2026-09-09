# Karan (KP) Content Diff Report

Generated: 2026-09-06. Source: `03-karan-guide.txt` vs. live `.dc.html` pages (verified Aug 2026).

---

## §1 — Money, Credit & ITIN

**Target page:** `Bay Playbook Money.dc.html`

### Already there (overlap)
Both cover the three-lane card sequencing (foreign-history transfer, no-SSN neobank, secured), Zolve as the no-SSN first move, the Amex Nova Credit flow for CIBIL-strong applicants, Capital One Quicksilver Secured as the secured-lane pick, OpenSky as the no-hard-pull fallback, the CAA route for ITIN, the same W-7 reason-code taxonomy (spouse/abroad/treaty), and the money-management bucket model (checking / high-yield savings / Mercury / Wise).

### Missing (Karan says this; page doesn't)
- **Self Visa (Credit Builder Account)** — Karan lists it as a Lane 2/3 hybrid with 0% intro APR, useful for the spouse case once an ITIN arrives. The page explicitly skips Self ("too slow when Zolve exists"), so this isn't missing — but Karan's *rationale* for the spouse-ITIN use case is worth noting.
- **Current Build Card** — Karan includes it as Lane 2. The page says Current requires an SSN, contradicting Karan. Resolution needed (see Conflicts).
- **BofA secured card** — Karan mentions Chase/BofA/Wells secured cards. The page correctly notes only BofA still offers it; no gap there.
- **Month 12+ card recommendations** — Karan names Chase Freedom and Bilt explicitly. The page covers these too (Freedom Rise, Bilt). No gap.
- **Sequencing specifics** — Karan's "month 6–9: soft pull limit increase" and "month 12+: travel card (Amex Gold/Platinum, Chase Sapphire)" for the India route. The page covers month 6–9 but doesn't mention Amex Gold/Platinum or Chase Sapphire as year-one graduation targets. Low priority.
- **Foreign transaction fee trap** — Karan flags that most newcomer/secured cards charge 2.5–3% FX for India spend and recommends getting one no-FX card. The page mentions Zolve's 3% FX fee but doesn't proactively recommend adding a no-FX card for India spend. Could be added as a "watch for" note.
- **Minimum-balance specifics** — Karan gives exact figures: Chase $1,500, BofA $500. The page gives Chase $1,500 and BofA SafeBalance $4.95 waived at $500 — already covered.
- **App stack** — Karan recommends Quicken Simplifi and YNAB by name. The page covers both. No gap.
- **ITIN: 3-year expiry and dormancy** — Karan notes that an unused ITIN lapses after 3 consecutive years. The page covers this in `itinFacts`. No gap.
- **ITIN: state ITIN mortgage programs** — Karan says some banks treat ITIN as sufficient for primary account opening; worth asking. Page does not mention ITIN-only account-opening scenarios for the founder (vs. spouse). Minor add.

### Conflicts (Karan contradicts the page)
- **Current Build Card SSN requirement** — Karan says Current doesn't require an SSN (Lane 2). The page explicitly states: "Current's Build card requires an SSN despite being marketed at newcomers, which defeats the point." One of them is wrong; the page's claim is more recent (Aug 2026) and more specific.
- **Amex/Nova Credit** — Karan says the Nova Credit flow reads CIBIL and gets you "a real, unsecured card on day one with no US history" and "no SSN needed." The page's orange callout directly contradicts: "Amex has required an SSN or ITIN from every US applicant since August 2023. Nova Credit gets your Indian history considered; it no longer gets you around the SSN." The page is correct on current policy. Karan's guide is outdated on this specific claim.
- **ITIN processing time** — Karan says "7–11 weeks, up to ~14 in the January–April crush." The page says "About 7 weeks, stretching to 9 or 11 between mid-January and April, or when applying from abroad." These are substantively the same range, framed slightly differently. No true conflict.

### Page has, Karan doesn't
- The interactive SSN/CIBIL/freeze chip UI that personalizes card recommendations — unique to the page.
- The 2025 credit rule change: "The Child Tax Credit now requires SSNs, and education credits will from 2026, so an ITIN-only household member no longer unlocks those." Karan doesn't flag this.
- The Deserve EDU stale-guide callout (shut 2025). Karan doesn't mention Deserve.
- The 2027 work/student-visa subsidy loss (healthcare page, but related).

---

## §2 — Banking and Setting Up Finance in US

**Target page:** `Bay Playbook Business Banking.dc.html`

### Already there (overlap)
Both cover Mercury (default for fresh Delaware C-corp), Brex (requires $50k+ or VC backing, now Capital One-owned), Rho (banking + bill pay + cards + treasury in one), Relay (named sub-accounts for multi-person spending), the three-bucket account structure (operating / payroll reserve / tax reserve), ACH vs. wire vs. SWIFT pricing, and the ODI/FEMA framework for Indian entity → US entity transfers.

### Missing (Karan says this; page doesn't)
- **Personal banking bank-by-bank table** — Karan covers Chase, Bank of America, Wells Fargo, HSBC, and credit unions with specific document requirements and newcomer-friendliness ratings. The Business Banking page explicitly scopes to company accounts and cross-links to the Money page. This personal-banking layer has no dedicated home other than a brief mention in the Guides' "Bank, cash & Clipper" section. Karan's BofA detail ("broadest accepted-ID list, including consular IDs") and the HSBC pre-arrival tip ("existing HSBC India customers can sometimes pre-open a US account before landing") are not in any live page.
- **Hacks for branch visits** — "Call ahead, book a 'new-to-country account opening' appointment," "go on a weekday morning," "bring more than the minimum (I-94 printout, Mercury statement)," "if declined, try a different branch." These are Karan's practical tactics; no live page captures them.
- **Wise personal account and Revolut** as digital-first complements to branch banking. The Money page mentions Wise for money in transit; no page mentions Revolut for multi-currency cards during India travel.
- **Mercury $15k monthly card-repayment cap on entry tier** — Karan flags this watch-out. The page says "The IO credit card auto-repays daily until you hold $15k" — same information, different framing. No true gap.
- **Relay: Thread Bank enforcement action** — The page notes this. Karan doesn't. Page is better on this point.
- **ODI 400% net-worth cap detail** — Karan explains that for an early-stage flip, the Indian entity's net worth may be very small, meaningfully constraining direct transfers and pushing founders toward personal LRS remittances. The page covers the 400% cap and flags the audit-lag issue but doesn't spell out the early-stage constraint as clearly.

### Conflicts (Karan contradicts the page)
- **Brex acquisition date** — Karan says "Capital One completed its acquisition of Brex in April 2026." The page says "Capital One closed its $5.15B acquisition in April 2026." Same fact, consistent.
- **Rho FDIC coverage** — Karan says "Up to $75M via Webster Bank." The page says "Checking sits at Webster Bank at $250k standard; savings reach up to $75M via a 400+ bank sweep." Karan slightly oversimplifies; page is more precise.

### Page has, Karan doesn't
- Interactive idle-cash and transfer-cost sliders showing real dollar costs at the user's balance.
- The Thread Bank / Relay enforcement-action warning.
- Relay FDIC coverage at $3M (Karan says "standard single-bank FDIC ($250k) unless upgraded" — page is more specific).
- The 2026 FEMA beneficial-ownership amendment for land-border-country entities — both cover it.

---

## §3 — Healthcare & Insurance

**Target page:** `Bay Playbook Healthcare.dc.html`

### Already there (overlap)
Both cover the 60-day QLE clock from move date, Covered California metal tiers (Bronze/Silver/Gold/Platinum), the 2026 subsidy cliff at 400% FPL, bridge plan options (Insubuy, VisitorsCoverage, Atlas America), telehealth-first triage, the No Surprises Act ER protections, and the Indian meds crossover (OTC vs. Rx, 90-day import limit, PCP wait times).

### Missing (Karan says this; page doesn't)
- **Day-by-day SEP sequence** — Karan gives a specific schedule: Day 1–3 create account, Day 3–14 upload docs, Day 14–30 select plan, Day 60 hard deadline. The page gives the hard deadline and clock but not a phased action timeline with those specific windows.
- **Short-term medical insurance option** — Karan mentions US short-term plans (up to 12 months in California) as a gap-filler if the SEP is missed: they cover unexpected illness/injury but exclude pre-existing conditions and fall outside the No Surprises Act. The page doesn't mention short-term plans as a missed-deadline option at all.
- **Group plan as SEP bypass** — Karan notes that a company group health plan "sidesteps the individual-market SEP question entirely." The page mentions group plans ("what beats all of this") but doesn't call out that group plans have their own more-forgiving enrollment rules, eliminating the 60-day trap.
- **Proof-of-prior-coverage requirement** — Karan warns that the prior-coverage proof trips up founders who assume their Indian insurance is irrelevant. The page directly contradicts this (see Conflicts below).
- **Specific cost numbers for VisitorsCoverage Elite** — Karan quotes "~$20–$170/month depending on age/tier." The page shows Atlas America at "$80–95/mo" and INF Elite X as "pricier." Karan's range is useful context.
- **California state subsidy ceiling** — Karan says California's backstop targets households up to 165% FPL (~$25,800 for a single) and doesn't help the 250–450% FPL range. The page shows the state programme ceiling at ~$25,800 in the salary slider. Same info, Karan's narrative framing of who it doesn't help is missing.
- **2026 Covered California subsidy figure** — Karan says statewide average post-subsidy premium jumped from ~$151/month (2025) to ~$261/month (2026). The page gives one worked example (60-year-old, $80k income: $554 → $1,000+) but not the average. Minor.

### Conflicts (Karan contradicts the page)
- **Proof-of-prior-coverage requirement** — Karan says "the proof-of-prior-coverage requirement trips up founders who assume their Indian insurance (or none at all) is irrelevant to a US move. Bring whatever documentation you have." The page says the opposite: "You do not need proof of prior insurance. The federal rule does ask movers to show recent coverage, but the regulation says living in a foreign country during the 60 days before the move satisfies it on its own. Your Indian policy, or the lack of one, is irrelevant." The page cites 45 CFR 155.420 and is almost certainly correct. **Karan's guidance here is wrong.**
- **What Covered California asks for** — Karan says "upload proof of your prior coverage" and "proof-of-move documents." The page says the document they actually ask for is proof of the *new* address (lease, bank statement, attestation) — not prior coverage. Another instance where Karan's guide has the requirement backwards.
- **ER cost figures** — Karan says "Emergency room: $800–3,000+; can exceed $2,863 with imaging." The page says "$1,500–3,000+ before imaging." The page's numbers are higher; Karan's lower bound ($800) may reflect older data or simpler visits. Resolve by keeping the page's more conservative (user-protective) numbers.

### Page has, Karan doesn't
- The interactive 60-day countdown clock tied to an entered move date — unique to the page.
- The 2025 federal tax law change: work/student-visa holders lose subsidy eligibility entirely on 1 January 2027. Karan doesn't mention this.
- The California 2024 rule that state-regulated plans can't balance-bill for ground ambulances. Karan only covers the federal No Surprises Act.
- California's ban on medical debt in credit reports (since 2025). Karan doesn't mention.
- GoodRx pricing for generic drugs (metformin etc. under $8/month). Karan doesn't mention.
- The salary slider showing subsidy cliff in real-time.

---

## §4 — The Desi Directory

**Target page:** `Bay Playbook Directory.dc.html`

**STATUS: Karan never wrote this section.** Verified by extracting pages 1–31 of the source PDF. Karan's ToC lists it, but the actual content jumps straight from Money (§1) → Business Banking (§2). No Directory content exists in the guide.

**Action:** no diff to run. The live Directory page (43-entry filterable database) stands as-is unless we source Directory content from elsewhere.

---

## §5 — Where to Host Events

**Target page:** would be NEW PAGE — but Karan didn't write the content.

**STATUS: Karan never wrote this section.** Verified against all 31 PDF pages. In ToC, no body content. Content jumps Business Banking → Healthcare.

**Action:** if we want this page, source content from elsewhere (V1 content PDF has some, or commission a new draft). Do not scope a Karan-based page.

---

## §6 — Sending Money Home & NRI Banking

**Target page:** `Bay Playbook NRI Banking.dc.html`

### Already there (overlap)
Both cover NRE vs. NRO account distinction (source of funds, India tax treatment, repatriation rules), the 4-step conversion sequence (resident → NRO only, fresh NRE for US income), Form 15CA/15CB mechanics and the April 2026 rename to Form 145/146, Wise vs. Remitly vs. bank wire comparison, the 1% US remittance tax (cash-only), LRS $250k cap and 20% TCS above ₹10 lakh, Form 3520 for foreign gifts above $100k, Form 709 for outbound gifts, FCNR deposits as a USD-parked-in-India option, PPF NRI notification requirement, and the PFIC trap on Indian mutual funds.

### Missing (Karan says this; page doesn't)
- **Concrete Wise vs. Remitly crossover numbers** — Karan gives a worked example: "on a $5,000 transfer at ~₹95/USD, Wise nets ~₹4,65,500; Remitly nets ~₹4,68,350–4,73,100. At $1,000, Remitly typically delivers a couple hundred more rupees." The page's interactive calculator shows these comparisons live but notes (correctly for Aug 2026) that Remitly beat Wise at both $1,000 and $5,000 on this corridor. The page is more useful; Karan's static numbers are stale.
- **FCNR USD rates as of 2026** — Karan quotes "4.5–5.2% on 1–2 year USD deposits, some banks (RBL, YES Bank) up to ~4.85%." The page mentions "roughly 3.5 to 5% on one to two year tenures" in the loose-ends section and a separate callout for the RBI rate-ceiling lift (6.25–6.75% on 3–5 year deposits until 30 September 2026). Karan's specific bank names (RBL, YES Bank) are not in the page — minor add if rates are still accurate.
- **Gift-splitting on Form 709** — Karan notes married founders can give $38,000 per recipient by electing gift-split. The page covers this in `formNotes` ("Gift-splitting doubles the room"). Already there.
- **Form 3520 mailing logistics** — Karan says "mailed separately to IRS's Ogden, Utah office — cannot be e-filed." The page says "paper-only, mailed separately to Ogden, Utah." Already covered.
- **NRO interest TDS rate** — Karan says "taxable at 30.9% TDS." The page says "31.2% TDS. The treaty caps it at 15% if you file the paperwork. Karan quotes 30.9% — older guides quote that rate; the page's 31.2% is the post-surcharge rate. **Karan's number may be stale** (see Conflicts).
- **PPF: since October 2024 rule** — Karan says PPF accounts with undisclosed NRI status can have interest cut. The page says "since October 2024 accounts with undisclosed NRI status can have interest cut to the savings rate or to zero." The page is more specific and more current than Karan.

### Conflicts (Karan contradicts the page)
- **NRO TDS rate** — Karan says 30.9%; the page says 31.2% and explicitly calls out "The NRO rate is 31.2%, NOT the 30.9% older guides quote." Karan's guide is one of those older guides. The page is correct.
- **Wise vs. Remitly crossover** — Karan says "above ~$3,000 Wise wins; at $1,000 Remitly wins." The page says this crossover "did not show up" in August 2026 and Remitly landed more rupees at both amounts. This is a real-time data point, not a permanent conflict — the principle (compare both) is the same.

### Page has, Karan doesn't
- FBAR coverage (FinCEN Form 114) and Form 8938 (FATCA) — both absent from Karan's guide. The page has an interactive form-checker for all four US disclosure forms.
- The RBI temporary FCNR rate-ceiling lift (6.25–6.75% on 3–5 year deposits until 30 September 2026). Karan doesn't mention the RBI ceiling lift.
- The NRO Treaty-rate mechanics: Tax Residency Certificate (Form 6166) + e-filed Form 10F required for the 15% treaty rate. Karan says "reducible under the India–US DTAA" without explaining how. The page is more actionable.
- KYC modification logistics: "one modification through the KYC registration agency plus notifying fund registrars covers your folios." Karan says update KYC but doesn't explain the mechanics.

---

## §7 — Wellness & Isolation — Done Properly

**Target page:** would be NEW PAGE — but Karan didn't write the content.

**STATUS: Karan never wrote this section.** Verified — extracted PDF pages 25–31 confirmed the content ends with the NRI Banking checklist. Wellness is in the ToC only.

**Action:** if we want this page, source content elsewhere. The scope Karan implied (immigrant-founder isolation, culturally competent therapy, 988 vs 911, year-one burnout, structural loneliness) is a legitimate P1/P2 page — but it's a brand-new draft, not a port.

---

## Summary of highest-priority actions

1. **Resolve the proof-of-prior-coverage conflict (§3):** Karan says bring prior coverage docs; the page (correctly, citing 45 CFR) says living abroad satisfies it. Do not port Karan's guidance here — it would make the page worse.
2. **Resolve the Amex/Nova Credit conflict (§1):** Karan says no SSN needed for Amex via Nova Credit. The page correctly states SSN/ITIN has been required since August 2023. Do not port Karan's framing.
3. **Port the personal banking bank-by-bank detail (§2):** HSBC pre-arrival tip, BofA consular ID acceptance, branch-visit hacks — none of this is on any live page. Belongs either in the Money page or the Guides' "Bank, cash & Clipper" section.
4. **Verify the Wellness section exists in the PDF (§7):** Check `03-karan-guide.pdf` pages 25–31 before scoping a new page.
5. **Check for an Events venue section in the PDF (§5):** Same — the .txt extract doesn't contain it.
6. **Minor: add no-FX-card recommendation for India spend (§1):** Karan's 2.5–3% FX trap callout adds useful nuance missing from the Money page's card table.
