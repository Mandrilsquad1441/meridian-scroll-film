# Product-page proposal — "Write once, run real"

**Client:** a global industrial-technology company (anonymized — "the Client"; the demo
uses the fictional brand **MERIDIAN** and its fictional product **Atlas Automate**).
**Subject:** the product page for the Client's flagship **automation-engineering
software** — the environment where industrial engineers configure hardware, program
controllers, simulate, commission and operate.
**Deliverable:** a scroll-cinematic product-page concept (`automate/index.html`,
real generated footage scrubbed by scroll) + this rationale. Companion to the
home-page proposal (`PROPOSAL.md`) — same world, same design system.

---

## 1 · What the current product page does today

| # | Section | Content |
|---|---------|---------|
| 1 | Hero | Product name + one-paragraph value prop, static render, 2 CTAs |
| 2 | Event banner | Conference promo interrupting the product story |
| 3 | "More than a framework" | 4 pillars as prose paragraphs (AI assistant, simulate-first workflow, integrated engineering, transparent operations) |
| 4 | Product list | Flat link list: the AI agent + 3 tool modules + a cross-sell + training |
| 5 | Options overview | One paragraph + "Read" link |
| 6 | FAQ | 3 questions |
| 7 | Contact form | **~20 required fields** (name, company, country picker with 200+ entries, industry, job role, job function, phone…) |

### The five problems

1. **The biggest news is buried.** The generative-AI engineering assistant — the one
   thing on this page competitors can't match — is the fourth bullet and the first
   item of a flat list. It deserves the spotlight, not a line item.
2. **The product never moves.** This is software whose entire pitch is *motion* —
   code becoming a running line — presented as a static render and prose.
3. **Pillars as paragraphs.** Four strong arguments formatted as a wall of text.
4. **The form is a wall.** Twenty required fields (including job function and a
   200-country dropdown) between an interested engineer and a conversation.
5. **No lifecycle story.** Configure → program → simulate → commission → operate is
   the product's actual shape; the page never walks it.

---

## 2 · The proposal

One continuous cinematic shot that *is* the product story — code becomes a running
line — then a short, conversion-focused product page.

### Concepts pitched

**A. "Write once, run real" — (Recommended · built in this demo)**
You open inside the engineering canvas: holographic function-block diagrams drifting
in a deep blue void, the headline *Write once. Run real.* and a trial CTA right in
the hero. Scroll: the blocks converge and assemble into a physical control cabinet —
racks materializing from wireframe to metal, status LEDs blinking on (*Engineer it
once*). Scroll: a teal pulse leaves the cabinet and races along the cable trays into
a dark production hall; robots and conveyors wake as it passes (*Download. Then watch
it wake.*). The film ends on the whole line running in rhythm (*The line runs. You
iterate.*) and melts into the content: pillars as cards, the copilot promoted to its
own band with a 3-step "how it works", three module rows, FAQ, and a two-button
contact band replacing the form.

**B. "The night shift"**
The film follows the AI copilot working overnight — a dark office, a project
assembling itself, tests passing — and dawn breaking as the engineer arrives to
finished work. Strong copilot story, but it makes the *assistant* the hero rather
than the *environment*, and office interiors read less premium than machinery.

**C. "One project"**
A single camera orbit around an exploded-view machine that assembles as you scroll —
controllers, drives, safety, HMI layers flying together into one whole. Clear
"one data model" metaphor; weaker narrative arc (no journey, just assembly).

### Why A wins
It walks the product's actual lifecycle in one unbroken move, gives the film a
physical payoff (the running line), and lands the visitor on the trial CTA twice —
once in the hero, once after the proof.

---

## 3 · Section-by-section mapping

| Current | Proposed | Rationale |
|---|---|---|
| Static hero + 2 CTAs | **The film** (4 chapters) with trial CTA *in* the hero | The product pitch is motion; show it |
| Event banner | Removed from the product page | Events live in the newsroom, not mid-pitch |
| 4 pillar paragraphs | **4 pillar cards** | Scannable, equal-weight arguments |
| AI agent as list item #1 | **Dedicated copilot band** with stats + 3-step flow | The differentiator gets the spotlight |
| Flat module link list | **3 module rows** (program / visualize / commission) + one options line | Hierarchy: the environment first, SKUs second |
| Options paragraph | One mono line inside modules | Detail belongs one click deeper |
| FAQ | Kept — 3 native, accessible disclosures | It earns its place |
| 20-field contact form | **Two buttons** (free trial / walkthrough) + a one-working-day promise | Every removed field is measurable funnel |

---

## 4 · Design system

Same anonymized-but-Client-toned system as the home-page proposal: deep blue
`#000028`, petrol `#009999`/`#007575`, spark green `#00FFB9`, cool paper `#F5F7F7`,
Archivo sentence-case display + IBM Plex Mono HUD. The footage for this film is
generated in the teal/petrol family end-to-end, so film and UI share one palette.
Accessibility: `prefers-reduced-motion` and no-JS visitors get a static, fully
readable page; FAQ uses native `<details>`; skip-link jumps past the film.

## 5 · Success metrics

Trial-CTA click-through (hero vs. post-film placement), contact-band conversion vs.
the legacy form's completion rate, scroll depth past chapter 2, copilot-band dwell
time, and assisted conversions from the home page's platform tile.

---

*MERIDIAN and Atlas Automate are fictional brands. All statistics are illustrative
placeholders. This document is an anonymized design proposal and names no real
company or product.*
