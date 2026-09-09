---
name: battlecard-generator
description: Produces a rep-facing HTML battlecard for one named competitor (header info, company overview, positioning framework, value pillars, discovery questions, objection handlers, do-not-say list, optional feature matrix), sourced from competitive-landscape.md. Can also update just the changed sections of competitive-landscape.md's own deeper reference entry when new raw research comes in. Use for the field-ready, printable/openable card a rep skims before or during a call — not the analyst-maintained reference doc itself.
---

# Battlecard Generator

## Purpose

Turn the deep, analyst-maintained competitor data in `competitive-landscape.md` into a battlecard a rep can actually use live: scannable in under a minute, structured the way a real sales-enablement battlecard is structured, not a research summary reformatted with headers.

## Two outputs, two audiences

1. **The rep-facing battlecard** (primary output, HTML) — for someone about to get on a call. Dense, visual, skimmable, no analysis-speak.
2. **An update to `competitive-landscape.md`'s own entry** (Markdown, targeted) — for whoever maintains the deeper reference doc. Only when new raw research comes in; output only the changed sections, not a full regeneration (see [`example.md`](./example.md) for this mode).

## Instructions — rep-facing battlecard

1. **Header info**: competitor name, last-updated date, and a named battlecard owner (the person responsible for keeping it current — a battlecard with no owner rots silently).
2. **Company overview & strategy**: exactly 2 sentences — who they are, their target market, how they position against us. Not a company history.
3. **Positioning framework ("land mines")**: use the transition formula *"They say X → The reality is Y → We're better because Z."* Pull "X" from their actual public messaging (see `competitive-landscape.md`'s Marketing & Positioning data), not a strawman. "Y" must be sourced, not invented. "Z" must map to a real differentiator, not a generic claim.
4. **Value pillars & differentiators**: 3–5, each with a concrete proof point (a stat, a named capability, a win-rate figure) — never a bare adjective claim ("we're more reliable" without evidence doesn't count).
5. **Discovery/landmine questions**: high-impact questions a rep can ask *before* the competitor comes up, designed to surface the competitor's actual weakness in the prospect's own words rather than the rep asserting it. Phrase them as something a rep would really say out loud, not a research prompt.
6. **Objection handlers**: written as a rep would actually say them — natural sales language, not analysis. Pair each stated objection with the response.
7. **Do-not-say list**: explicit guardrails — overclaims, unverified claims, or comparisons that would backfire if fact-checked by the prospect. Every entry should be something a rep would otherwise be tempted to say.
8. **Feature matrix (optional)**: only if there are genuinely critical gaps worth a table (integrations, pricing model, compliance, deployment). Skip it if the prose above already covers the differentiators — a redundant table is worse than no table.
9. **Match template depth to actual threat level.** A Low-threat competitor (see `competitive-landscape.md`'s Quick reference) gets a visibly shorter card, not a padded one forced into the same length as a High-threat competitor.

## What to avoid

- Don't invent a proof point, a stat, or a quote that isn't backed by `competitive-landscape.md` or the raw research provided.
- Don't write a discovery question that's really just an assertion in question form ("Isn't it true that X is slow?") — a real discovery question invites the prospect to say something, it doesn't lead the witness.
- Don't let the do-not-say list quietly disappear when a claim becomes true (e.g. a competitor ships a feature that used to be fair game to question) — check `competitive-landscape.md`'s "Last verified" date and `staleness-detection` before reusing an old card unchanged.

## Output format — rep-facing battlecard

```
[Header] Competitor · Last updated · Owner
[Company Overview & Strategy] — 2 sentences
[Positioning Framework] They say X → Reality Y → We win because Z
[Value Pillars] 3-5, each: headline + proof point
[Discovery Questions] 3-5, phrased as spoken questions
[Objection Handlers] objection → response, paired
[Do-Not-Say List] explicit guardrails
[Feature Matrix] (optional) — only critical gaps
```

See [`bricklane-data.html`](./bricklane-data.html), [`estemate.html`](./estemate.html), [`valuai.html`](./valuai.html), and [`propiq.html`](./propiq.html) for this format applied to each tracked competitor.
