# 22 · Groceries & Cooking

**Section:** S5 · LIVE IN IT
**HTML file:** `pages/Bay Playbook Groceries.dc.html`
**Approx. word count:** 2951

## Dek

Where to buy dal, paneer and atta{{ g.atta.tag }}{{ g.atta.def }}, what the American-store equivalents actually are, and how to eat well without cooking every night.

## Sections on this page

- What do you actually need this week?
- The translation table
- Where to go
- Delivery, if you're in the city without a car
- Tiffin, when you stop cooking
- Eating out, by area
- Do this now

## Notes for editing

- Content in the `.dc.html` file is mostly inline in HTML. To rewrite copy, edit the `.dc.html` file directly — every visible string is plain text between tags.
- Section eyebrow, h1, and dek are in the first ~30 lines of the file.
- Interactive widgets (e.g. visa chooser, cost calc) use `renderVals()` — computed values are at the bottom of the file in a `<script type="module">` block. Wording changes to the widget copy go inline in the template above; logic changes go in the script.
