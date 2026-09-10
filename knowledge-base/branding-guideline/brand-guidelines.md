# Brand Guidelines — Sundial Analytics

The full brand system: who we are, how we sound, and how we look. For the detailed voice/tone rules a rewrite skill actually applies, see [`skill.md`](./skill.md) — this document covers the fuller identity those rules serve, plus everything visual. See [`positioning.md`](../positioning.md) for the strategic narrative these guidelines express.

---

## Core Identity

### Mission

Give lenders a property valuation they can actually defend, not just receive.

### Vision

A market where every automated financial decision — not just Sundial's — can withstand scrutiny, so "the model said so" stops being an acceptable answer anywhere in lending.

### Brand values

1. **Defensible over impressive.** A claim that survives being questioned beats a claim that only sounds good in a demo.
2. **Precision, not hype.** Say exactly what the product does. If we can't name the specific mechanism, we don't make the claim.
3. **Transparency by default.** Show the work — the comparables, the weighting, the methodology — rather than asking for trust.
4. **Respect the skeptic.** Our best-fit buyer is trained to distrust vendor claims. That skepticism is correct more often than not, and we build and write for it rather than around it.
5. **Substance before speed.** Speed is real value, but never the whole pitch — see [`positioning.md`](../positioning.md)'s "what this is not."

### Brand voice and tone

Full rules (style standards, anti-patterns, prohibited terms, approved substitutions) live in [`skill.md`](./skill.md) — summarized here: confident and specific, never hyped, written for a technically skeptical, regulator-adjacent reader who trusts precision over enthusiasm.

Tone shifts by channel, but the underlying values above never do:

| Channel | Tone | What changes |
|---|---|---|
| Marketing pages | Confident, declarative | Leads with the claim; still no hype language or unexplained AI claims |
| Sales decks | Persona-adapted | Structure and emphasis change by buyer (see [`personas.md`](../personas.md)); the voice rules don't |
| Support / product emails | Direct, plain, helpful | Shorter sentences, no persuasion register at all — a support email that sounds like marketing copy erodes trust fast with this audience |
| Sales conversation / call | Consultative, willing to say "I don't know, let me find out" | The one channel where admitting a limitation live is a trust *builder*, not a liability — see the sales-call-analysis examples in [`../sales-call-analysis`](../sales-call-analysis) |
| Internal docs (this repo included) | Direct, reasoned, can be more casual | Precision matters as much as externally; hype matters less |
| Social / conference presence | Minimal, factual | We don't chase attention with urgency language — see the Anti-patterns in [`skill.md`](./skill.md) |

---

## Visual Identity

### Logo

- [`logo.svg`](./logo.svg) — primary lockup (mark + wordmark), for light backgrounds
- [`logo-reversed.svg`](./logo-reversed.svg) — white version, for dark/navy backgrounds
- [`logo-mark.svg`](./logo-mark.svg) — icon alone, for favicons, social avatars, and spaces too small for the wordmark
- [`logo-usage.svg`](./logo-usage.svg) — clear space, minimum size, and misuse reference sheet

**Clear space:** minimum clear space on every side equals the height of the mark itself. Nothing — text, edges, other logos — enters that space.

**Minimum size:** 24px height (digital) / 10mm (print) for the mark alone; below that, use the mark only, never the full lockup with the wordmark.

**On dark surfaces:** always use `logo-reversed.svg`. Never place the primary (navy) mark on a dark background at reduced opacity as a substitute.

**Don't** (see [`logo-usage.svg`](./logo-usage.svg) for each of these rendered):
- Stretch or distort the proportions
- Recolor outside the palette below
- Place it on a busy or low-contrast background
- Add a drop shadow, outline, or other effect
- Rebuild the wordmark in a different typeface
- Separate the mark from the wordmark arbitrarily (the icon alone is fine — see `logo-mark.svg` — but don't split the primary lockup and space its pieces independently)

### Color palette

See [`color-palette.svg`](./color-palette.svg) for the swatch reference. CMYK values are the standard mathematical conversion — verify against your actual print profile before a physical print run.

| Role | Name | HEX | RGB | CMYK |
|---|---|---|---|---|
| Primary | Sundial Navy | `#1A3A5C` | 26, 58, 92 | 72, 37, 0, 64 |
| Secondary | Meridian Gold | `#C1892E` | 193, 137, 46 | 0, 29, 76, 24 |
| Neutral | Ink | `#1C1C1A` | 28, 28, 26 | 0, 0, 7, 89 |
| Neutral | Slate | `#8A8782` | 138, 135, 130 | 0, 2, 6, 46 |
| Neutral | Paper | `#F4F3EF` | 244, 243, 239 | 0, 0, 2, 4 |
| Status — good | — | `#0CA30C` | 12, 163, 12 | reserved for success states only |
| Status — warning | — | `#D68A1F` | 214, 138, 31 | distinct from Secondary on purpose — a status color should never double as the brand accent |
| Status — critical | — | `#D03B3B` | 208, 59, 59 | reserved for error/critical states only |

Primary and Secondary are for brand and marketing use. Status colors are reserved for product UI state (success/warning/error) and never repurposed as decoration — status color and brand accent stay visually distinct on purpose, so one never impersonates the other.

### Typography

- **Display / headings:** Archivo (weights 600–800). Used for logo wordmark, page titles, section headers.
- **Body:** IBM Plex Sans (weights 400–600). Used for all running text, UI labels, and email copy.
- **Data / mono:** IBM Plex Mono (weights 400–500). Reserved for dates, source citations, tabular figures, and code — never for prose.

| Use | Face | Weight | Notes |
|---|---|---|---|
| H1 / page title | Archivo | 700–800 | `text-wrap: balance`; never all-caps |
| H2 / section header | Archivo | 600–700 | |
| Body copy | IBM Plex Sans | 400 | ~65-character line length target |
| UI labels, buttons | IBM Plex Sans | 500–600 | Sentence case, never all-caps except small eyebrow labels |
| Eyebrow / small label | IBM Plex Mono | 500 | Uppercase with letter-spacing is the one place all-caps is correct |
| Data, dates, citations | IBM Plex Mono | 400 | `font-variant-numeric: tabular-nums` where digits line up in columns |

This is the same type system already used across this repo's designed artifacts ([`competitor-monitoring`](../../sales-tools/competitor-monitoring)'s report, [`battlecard`](../../sales-tools/battlecard)'s cards, [`sales-call-analysis`](../sales-call-analysis)'s rollup) — those weren't a one-off design choice each time, they were this brand system applied consistently.

### UI/UX visual styles

So the product and marketing site read as one brand, not two:

- **Buttons:** square or minimally rounded corners (2–4px), never full pill-shaped by default. Primary action in Sundial Navy with white text; secondary action outlined, not filled. No gradient fills.
- **Forms:** labels above fields, not placeholder-only. Error state uses Status — critical with a text explanation, never color alone.
- **Cards:** hairline border (`#E1E0D9`-equivalent) over drop shadows — shadows read as decorative, not this brand's register. Flat, bordered panels over "floating" elevated cards.
- **Icons:** see Image and Icon Style below — the same line-weight rule applies inside the product UI, not just marketing.

---

## Content and Assets

### Naming conventions

- **Pricing tiers** (brokerage/seat-based product): **Dawn** (entry), **Meridian** (mid), **Zenith** (enterprise) — a sundial's-day theme, used consistently and only for this purpose (not reused as a generic naming device elsewhere).
- **Feature names:** literal and descriptive, never invented proper nouns or trademarked-sounding names. "Audit Trail," not "TraceIQ™." "Coverage Map," not "SmartArea." This follows directly from the "precision, not hype" brand value — a cute feature name reads as marketing packaging on something that should read as infrastructure.
- **Product terminology (use consistently):**

| Use this | Not this |
|---|---|
| Valuation | Appraisal, estimate |
| Comparable | Comp |
| Audit trail | Explainability report, transparency log |
| Lender / bank | Client (in product copy — "client" is fine in casual internal use) |
| Loan origination system (LOS) | Origination platform, loan system |

### Image and icon style

- **No stock photography.** Especially no generic finance-stock clichés (handshakes, skyline photos, people pointing at monitors). This audience recognizes stock photography instantly and it reads as substance-free.
- **Prefer real product surfaces and data visualization** — an actual (or realistic mock) audit trail screenshot, a real comparable-weighting chart — over any illustration standing in for the product.
- **Where illustration is needed** (e.g. a concept with no literal screenshot, like "data residency"), use abstract geometric illustration consistent with the logomark's style — flat shapes, no gradients, no 3D renders, no isometric-office-life scenes.
- **Icon style:** line icons only, 1.5–2px stroke weight, no fills, consistent corner radius. No skeuomorphic, glossy, or 3D icon sets. This matches the logomark's own construction (a simple stroked arc plus a solid geometric mark) — the icon system and the logo should look like they were drawn by the same hand.
