# Home-page proposal — "Signal to Steel"

**Client:** a global industrial-technology company (anonymized — referred to below as "the Client"; the demo uses the fictional brand **MERIDIAN**).
**Deliverable:** a scroll-cinematic home-page concept — one continuous shot that plays as the visitor scrolls — plus a restructured content architecture below it.
**Demos:**
- `index.html` — the **cinematic footage film**: five AI-generated shots chained
  frame-to-frame into one continuous take (digital void → wireframe turbine →
  materialized machine → factory floor → night grid → dawn city), scrubbed on a
  canvas as you scroll (`frames/` required).
- `meridian-purecode.html` — the **pure-code fallback**: the same journey told in
  GSAP/Lenis motion, zero assets, works from a single file.

---

## 1 · What the current home page does today

An audit of the Client's live US home page, reduced to its structure:

| # | Section | Content |
|---|---------|---------|
| 1 | Hero **carousel** | 6 rotating stories (an AI product launch, a partner announcement, a transport platform, two digital-twin case studies, an event promo) |
| 2 | Technology chips | 6 topic links (AI, digital twin, digital transformation, infrastructure, automation, sustainability) |
| 3 | Content cards | Customer story + e-book + product spotlight |
| 4 | Marketplace banner | One CTA |
| 5 | Platform grid | **~10** product cards, equal weight, no hierarchy |
| 6 | Ecosystem grid | **~10** partner cards, equal weight |
| 7 | News | 3 items |
| 8 | Explore | About / Insights / Careers / History tiles |

### The five problems

1. **Carousel roulette.** Six hero stories rotate on a timer; industry benchmarks put
   interaction with slides 2+ in the low single digits. The Client's strongest
   material — the stories — is mostly unseen.
2. **Catalog-dump parity.** 9 product cards + 9 partner cards at identical visual
   weight. When everything is equally important, nothing is.
3. **The one story is never told.** Five of the six hero slides are the *same idea* —
   a digital model that becomes real-world results (a robot trained in simulation, a
   campus twin, a remote-plant twin, an AI that executes engineering). The page
   has the narrative and never connects it.
4. **No wayfinding by audience.** Engineers, plant operators, partners and job-seekers
   all land on the same undifferentiated wall; audience routing only appears at the
   very bottom.
5. **Static presentation of a motion company.** The Client sells simulation, motion
   and real-time systems — presented as still cards. The medium contradicts the message.

---

## 2 · The proposal

Replace the carousel with **one continuous cinematic shot, scrubbed by scroll**, that
tells the single story the portfolio already shares — *digital becomes real* — then
resolve into a short, ruthlessly prioritized content page.

### Concepts pitched

**A. "Signal to Steel" — (Recommended · built in this demo)**
You open in a black digital void — data particles drifting, a giant wordmark reveals
character by character: *WHERE DIGITAL BECOMES REAL*. Scroll: a wireframe turbine
draws itself and rotates — the digital twin, annotated like an engineering plate
(*simulated 14,000× before first bolt*). Scroll: the page turns sideways into a
horizontal run across "the floor" — the carousel's stories retold one at a time,
user-paced (the field robot, the remote plant, the engineering copilot), each
with one hard number. Scroll: an energy pulse draws across the grid and the counters
climb. Then a circular mask opens: dawn light, a city skyline, warmth — *real when it
reaches people* — and the film melts into the content page.

**B. "One Ordinary Morning"**
The film follows 05:00 → 09:00 in one city: a night factory shift ends, the grid
absorbs the morning ramp, the first train leaves, a building wakes. The company is
never the subject — it is the invisible layer that makes the morning boring, in the
best way. Warmer, more human; less explicit about the platform.

**C. "The Twin"**
A split screen the whole way down: left half digital wireframe, right half physical
steel, both showing the same object at the same moment. As you scroll, the divider
drifts and objects change (turbine → train → substation → hospital scanner) until the
halves converge into one image. Most conceptual; hardest to keep legible on mobile.

### Why A wins
It converts the carousel's *content* (nothing is thrown away — the same six stories
survive) into a *sequence* the visitor controls, and it dramatizes the actual product
thesis (simulate first, then build) in the mechanics of the page itself.

---

## 3 · Section-by-section mapping

| Current | Proposed | Rationale |
|---|---|---|
| 6-slide auto-carousel | **The film** (5 chapters, user-paced) | Every story gets seen, in an order that argues a thesis |
| Technology chips | Chapter structure of the film | Topics become narrative beats, not a link farm |
| Story/e-book/product cards | **Ch 3 "The Floor"** horizontal run + **Proof** rows | Three stories, one number each — proof, not promises |
| ~10-product platform grid | **"Atlas One"** band: 4 flagship tiles + "Full catalog →" | Hierarchy first, catalog one click away |
| ~10-partner ecosystem grid | One line inside the platform band | Partners are a level-2 page, not home-page real estate |
| News (3 items) | Ticker + 3 dated items | Kept, compressed, given typographic energy |
| Explore tiles | **Wayfinding**: Engineers / Operators / Partners / Careers | Route by *who you are*, not by *what we call things* |
| — | **One front door**: a single statement + 2 CTAs | The page finally has one primary action |

---

## 4 · Design system (fictional brand "MERIDIAN")

- **Palette:** tuned to the Client's existing brand feel while staying anonymized —
  deep blue `#000028` (the film's world), petrol `#009999` / deep petrol `#007575`
  (interactive, light surfaces), spark green `#00FFB9` (the digital-signal accent),
  cool paper `#F5F7F7`. The film moves from cold digital dark to warm dawn light;
  the content lands on clean, light ground the way the Client's site does.
- **Type:** Archivo variable in clean grotesque cut (sentence-case headlines,
  weight ~780 — engineered but human, close to the Client's corporate sans) +
  IBM Plex Mono for annotations, data readouts and the chapter HUD.
- **Motion:** Lenis smooth scroll + GSAP ScrollTrigger. Pinned scrubbed chapters,
  one horizontal run, a clip-path dawn reveal, counters, velocity-skewed ticker.
  A fixed chapter readout (label + progress bar) doubles as narrative HUD.
- **Accessibility:** full `prefers-reduced-motion` fallback — the film flattens into
  a static, stacked, fully readable page. Semantic landmarks, aria labels on scenes.
- **Performance:** GPU-only properties (transform/opacity), ambient canvas stops
  rendering once invisible, `?jump=` + `window.__ready` dev contract for automated
  screenshot/jank verification.

---

## 5 · What ships next

1. **Master the footage.** The current film is a draft-quality chain (480p) to prove
   the shot flow; the same approved prompts re-render at 1080p for production. Every
   junction between shots is verified numerically (SSIM ≥ 0.88), never eyeballed.
2. **CMS mapping.** Every block maps 1:1 to existing content types (story, product,
   news item), so the proposal is a re-templating, not a re-platforming.
3. **Success metrics.** Scroll depth past chapter 3 vs. carousel slide-2 interaction;
   primary-CTA click-through vs. current hero CTAs; audience-router usage vs. footer
   nav; bounce on organic brand queries.

---

*MERIDIAN is a fictional brand. All statistics in the demo are illustrative
placeholders. This document is an anonymized design proposal and names no real
company.*
