# Bay Playbook — Design System Reference

The site uses an inline-styles-only approach; no CSS classes are shipped as global rules. This doc names the tokens each page uses so anything new stays consistent.

## Colors

| Token | Value | Use |
| --- | --- | --- |
| `--accent` | `#E8500A` | primary CTA, section eyebrows, links |
| ink | `#1A1712` | body text, headlines |
| body-dim | `#3D3629` | secondary body copy |
| meta | `#8A8172` | small caps meta, "min read" labels |
| page bg | `#FAF7F1` | body background |
| card bg | `#FFFDF8` | interactive cards |
| divider | `#E2DACA` | 1.5px hairlines between sections |
| soft bg | `#F1EBDD` | hover states on nav rows |

## Fonts

Loaded from Google Fonts (see `<helmet>` in each `.dc.html`):

- **Archivo** (400–900) — default body + headlines
- **IBM Plex Mono** (400–700) — meta, section eyebrows, chip labels
- **Caveat** (600–700) — the handwritten "The … Playbook" wordmark
- **Silkscreen** (400–700) — the pixel-style "bay" in the wordmark

## Type scale (rough)

| Role | Size | Line-height | Weight |
| --- | --- | --- | --- |
| h1 (article) | 38px | 1.05 | 900 |
| h2 (section) | 22–26px | 1.15 | 800 |
| dek | 17px | 1.55 | 400 |
| body | 15–16px | 1.55 | 400 |
| card body | 13.5px | 1.55 | 400 |
| meta / eyebrow | 10–11px | 1 | 600, letter-spacing 0.1em, uppercase |

## Layout

- Article page: `grid-template-columns: 280px 1fr; max-width:1240px;` — 280px sidebar, article content maxes at 900px.
- Card grids: `grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 10–14px;`
- Section spacing: 40–56px vertical padding between article sections.

## Widget conventions

Interactive widgets (visa chooser, cost calc, week planner, wizard) share a pattern:

1. State lives in `localStorage` under keys prefixed `bp-` (e.g. `bp-visa-picks`, `bp-week1-checked`).
2. Computed presentation values are built in a `renderVals()` function at the bottom of each `.dc.html`.
3. The template uses `{{ path }}` placeholders (a custom template DSL in `support.js`) — no React JSX.
4. Loops use `<sc-for list="{{ items }}" as="item">`, conditionals use `<sc-if test="{{ path }}">`.

## Mobile

Currently the pages break at 390px because `.pbl__ch-*` classes are fixed-width. See §2.3 of `HANDOFF.md` for the exact CSS fix.

## Accent placement rules

- Use `--accent` for: primary CTA button, section eyebrow ("S1 · BEFORE YOU FLY"), active link.
- Do NOT use `--accent` for: body links (use ink black, orange on hover), decorative dividers, background fills larger than a chip.
