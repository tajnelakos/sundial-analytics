---
name: competitor-weekly-brief
description: Turns raw competitor signals (pricing changes, release notes, review excerpts, sales call mentions) into a structured weekly competitive brief with a mandatory "so what" for each item. Use when the user pastes competitor signals collected over the past week and wants a synthesized brief, not a raw summary.
---

# Competitor Weekly Brief

## Purpose

Convert scattered, unstructured competitor signals into a brief a sales leader or exec can read in under three minutes, where every item ties to a concrete implication — never just "here's what happened."

## Instructions

1. **Group signals by competitor**, then by type: pricing, product, market/positioning, customer sentiment.
2. **Discard noise.** Skip anything that doesn't plausibly affect our win rate, pricing power, or positioning. Not every changelog line deserves a brief entry.
3. **For each remaining signal, write three lines:**
   - **What changed** — one factual sentence, no editorializing.
   - **Confidence** — mark as `Confirmed` (from a primary source: their own pricing page, release notes, a direct quote) or `Needs confirmation` (secondhand, inferred, or ambiguous). Never present a `Needs confirmation` item with the same certainty as a `Confirmed` one.
   - **So what** — the implication for us, framed as an action or a talking point, not just an observation. If you cannot articulate a real implication, cut the item — do not pad the brief with filler.
4. **Order by urgency**, not by competitor alphabetically or by when the signal arrived. A pricing move that affects active deals goes above a minor UI change.
5. **Close with a one-line "Watch list"** — one or two things worth checking next week that aren't confirmed yet (e.g. a rumored feature, a pattern across two data points that might become a trend).
6. **Keep total length under ~400 words.** If the input contains more material than that allows, cut lower-urgency items entirely rather than compressing everything.

## What to avoid

- Don't speculate about a competitor's strategy or motive beyond what the signal supports ("they're panicking" is not an analysis).
- Don't recommend pricing or product changes — flag implications for sales/marketing conversations, not roadmap decisions.
- Don't repeat an item from a prior week's brief unless something new happened to it.

## Output format

```
## Competitive Brief — Week of [date]

### [Competitor name]
**[Signal headline]**
What changed: ...
Confidence: Confirmed / Needs confirmation
So what: ...

(repeat per signal, ordered by urgency)

### Watch list
- ...
```
