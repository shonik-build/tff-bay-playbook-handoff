# 27 · Emergency Contacts

**Section:** S5 · LIVE IN IT
**HTML file:** `pages/Bay Playbook Emergency.dc.html`
**Approx. word count:** 3445

## Dek

Dial 911 from a cellphone in San Francisco and you might get the California Highway Patrol instead of SFPD. Fremont's police department says it on their own site: a 911 call from a cell outside the immediate area lands with CHP first, and CHP doesn't receive an address from cell callers. Usually the transfer takes a few seconds. Sometimes it doesn't.

## Sections on this page

- Your city, not just the city
- The consulate does less than it used to
- If you lose your passport
- Urgent care or the ER?
- Break-ins, landlords, crashes
- The earthquake setup
- Do this now
- Nobody tells you
- The part that contradicts everything above

## Notes for editing

- Content in the `.dc.html` file is mostly inline in HTML. To rewrite copy, edit the `.dc.html` file directly — every visible string is plain text between tags.
- Section eyebrow, h1, and dek are in the first ~30 lines of the file.
- Interactive widgets (e.g. visa chooser, cost calc) use `renderVals()` — computed values are at the bottom of the file in a `<script type="module">` block. Wording changes to the widget copy go inline in the template above; logic changes go in the script.
