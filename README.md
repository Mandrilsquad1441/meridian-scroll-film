# MERIDIAN — "Signal to Steel"

An anonymized **scroll-cinematic home-page concept** for a global industrial-technology
company. The whole hero is one continuous shot that scrubs as you scroll — from a digital
wireframe model, through a materializing machine and a factory floor, out to a night grid
and a dawn city — then dissolves into a restructured content page.

*MERIDIAN is a fictional brand created for this design proposal. No real company is named.*

## What's here

| File | What it is |
|------|------------|
| `index.html` | The **cinematic footage film** — 5 generated shots chained frame-to-frame, scrubbed on a `<canvas>`. Needs the `frames/` folder beside it. |
| `meridian-purecode.html` | The **pure-code fallback** — the same journey in GSAP/Lenis motion, zero assets. |
| `PROPOSAL.md` | The written rationale: audit of the current page, concepts, section-by-section mapping. |
| `frames/` | 301 JPEG frames the film scrubs through. |

## Run it

It's static — open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

Respects `prefers-reduced-motion` and degrades to a readable static page without JavaScript.
