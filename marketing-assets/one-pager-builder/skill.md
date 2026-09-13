---
name: one-pager-builder
description: Builds a single-page, persona/segment-specific sales collateral piece (a "leave-behind") from personas.md, positioning.md, and icp.md — forces ruthless prioritization to one headline, one angle, and 3-4 proof points, since a real one-pager has no room for a general pitch. Use when the user wants a one-pager for a specific persona or segment, not a company overview.
---

# One-Pager Builder

## Purpose

A one-pager fails the moment it tries to say everything. The actual skill isn't writing copy — it's choosing the one angle and the one proof set that fit a specific persona or segment, and cutting everything else, rather than shrinking the type to fit more in.

## Instructions

1. **Identify the persona and/or segment this targets**, from [`personas.md`](../../knowledge-base/personas.md) and [`icp.md`](../../knowledge-base/icp.md). A one-pager for "everyone" is a one-pager for no one — if the user hasn't named one, ask, or point at `positioning.md`'s segment table for options.
2. **Select exactly one positioning angle** from [`positioning.md`](../../knowledge-base/positioning.md)'s per-segment value proposition table — not the general pitch, and not two angles hedging against each other.
3. **Enforce the budget: one headline (under 10 words), one subhead, 3-4 proof points, one CTA.** If the source material suggests more is relevant, cut — don't compress the type to fit more in. A one-pager that needs a second page is a different document.
4. **Every proof point must be a specific, checkable claim** from `positioning.md`'s differentiators table or a real case study (see [`case-study-builder`](../case-study-builder)) — not an adjective standing in for evidence.
5. **Match the target persona's actual content preferences** from `personas.md` — e.g. the Head of Credit Risk persona explicitly distrusts case studies without a named, checkable source, so a proof point citing a customer result needs the same sourcing discipline `case-study-builder` requires, not an invented stat.
6. **Follow [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s full visual system** (color palette, typography, card/button rules), not just its voice rules — unlike this repo's text-only skills, a one-pager is a designed artifact.
7. **Run the finished draft through [`positioning-compliance`](../positioning-compliance) before treating it as ready to send or print.**

## What to avoid

- Don't write "for [persona]" and keep the generic company pitch underneath unchanged — the angle itself has to change per persona/segment, the same way [`personalized-outbound`](../personalized-outbound) already requires for a single email.
- Don't cite a customer stat that hasn't been sourced through `case-study-builder`'s discipline or an equivalent real citation.
- Don't try to fit two personas on one page — build two one-pagers instead.

## Output format

```
## One-Pager — [Persona/Segment]

**Positioning angle used:** [angle, from positioning.md]
**Format:** designed single-page HTML (see accompanying .html file)

**Headline:** ...
**Subhead:** ...
**Proof points:**
1. ...
2. ...
3. ...
**CTA:** ...

---
Sourced from: [citation for each proof point]
```
