# 02 · Start With Your Decision

**Section:** S1 · BEFORE YOU FLY
**HTML file:** `pages/Bay Playbook Decisions.dc.html`
**Approx. word count:** 435

## Dek

Nobody arrives thinking in site sections — you arrive mid-decision. Ten questions, what each turns on, and the exact guides that answer it.

## Sections on this page

- {{ d.q }}

## Notes for editing

- Content in the `.dc.html` file is mostly inline in HTML. To rewrite copy, edit the `.dc.html` file directly — every visible string is plain text between tags.
- Section eyebrow, h1, and dek are in the first ~30 lines of the file.
- Interactive widgets (e.g. visa chooser, cost calc) use `renderVals()` — computed values are at the bottom of the file in a `<script type="module">` block. Wording changes to the widget copy go inline in the template above; logic changes go in the script.
