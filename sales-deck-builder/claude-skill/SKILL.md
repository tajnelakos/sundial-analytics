---
name: sales-deck-outline
description: Generates a slide-by-slide sales deck outline (headline, purpose, key point per slide) tailored to a specific buyer persona and deal stage, from minimal deal context. Use when the user gives a one-line deal context and wants a customized deck structure, not full slide copy.
---

# Sales Deck Outline Builder

## Purpose

Produce a slide-by-slide outline — not written slide copy — customized by buyer persona and deal stage, fast enough to sanity-check and hand off to a rep or designer.

## Instructions

1. **Ask for (or infer from context given) three things** before outlining: who's in the room (role/persona), what deal stage this is for (first meeting vs. late-stage/procurement), and any specific objection or theme already known from prior calls. If deal stage isn't given, default to "first substantive meeting."
2. **Match structure to persona, not just content.** A risk/compliance buyer's deck should lead with credibility and explainability before ROI. An operations buyer's deck should lead with workflow/time impact before going deep on methodology. Do not use the same slide order for both just because the product is the same.
3. **Every slide gets exactly three lines**: headline (what's on the slide, as the audience would read it — not an internal label), purpose (why this slide exists in this deck, one sentence), key point (the single thing the rep must land on this slide).
4. **Cap at 8-10 slides** for a first meeting, up to 12-14 for late-stage/procurement decks that need more proof points. A longer deck for an early meeting is a sign the outline is padded, not thorough.
5. **If a known objection or competitor is in the deal context, build a slide for it explicitly** rather than hoping the objection-handling happens verbally — a named objection deserves a named slide.
6. **End every outline with a single, specific next step slide** (not a generic "Thank You" slide) — what happens after this meeting, stated as an action ("Schedule technical validation call") not a sentiment.

## What to avoid

- Don't write full slide copy — this tool stops at outline level on purpose, so it stays fast to review and doesn't lock in wording prematurely.
- Don't default to a generic "About Us" slide unless the deal context specifically calls for company credibility to be established (e.g. an unfamiliar/skeptical buyer) — most decks don't need it and it wastes an early slide.
- Don't pad the slide count to hit a "standard" deck length.

## Output format

```
## Deck Outline — [deal context, one line]
Persona: [role] · Stage: [stage]

1. [Headline]
   Purpose: ...
   Key point: ...

(repeat per slide)
```
