---
name: sales-call-analysis
description: Extracts objections, competitor mentions, buying signals, and one coachable moment from a sales call transcript, in a consistent structure so output is comparable across many calls. Use when the user pastes a call transcript (discovery, demo, or negotiation call) and wants it analyzed, not just summarized. Also supports an aggregate mode that rolls many calls into one pattern-and-findings view — see the Aggregate mode section below.
---

# Sales Call Analysis

## Purpose

Produce the same four-part breakdown from every transcript, so that running this across dozens of calls yields comparable, aggregatable output instead of freeform summaries that can't be compared to each other.

## Instructions

1. **Identify speaker roles** first (rep vs. prospect, and prospect's role/title if stated or inferable) — this matters for step 3, since a buying signal from an economic buyer counts differently than one from an end user.
2. **Objections**: extract every objection the prospect raised, quoting or closely paraphrasing their actual words. Tag each as one of: price, product gap, timing/urgency, competitor comparison, internal politics/buy-in, other. Note how the rep responded and whether the objection seemed resolved, deflected, or left open.
3. **Competitor mentions**: log every mention of a named competitor, who brought it up (prospect unprompted vs. rep-initiated vs. prospect responding to rep), and the context. An unprompted prospect mention is a stronger signal than a rep-initiated one — flag which is which.
4. **Buying signals**: only count genuine signals — a specific question about implementation, timeline, pricing tiers, procurement process, or "who else needs to be involved." Do not count politeness, enthusiasm, or generic positive language ("this looks great") as a buying signal on its own.
5. **One coachable moment**: pick a single moment where the rep could have handled something better — a missed follow-up question, a rushed answer to an objection, talking past a buying signal. Frame it constructively and specifically (quote the moment), not as a general critique. Skip this section entirely if nothing genuinely rises to this level — don't manufacture a critique to fill the section.
6. **Do not score or rate the call.** This is a structured extraction tool, not a scorecard — no numeric or letter grades.

## Output format

```
## Call Analysis — [prospect/company, if known] — [date if known]

**Participants:** [rep] / [prospect name, role]

### Objections
- [Objection, tag] — Rep response: ... — Status: resolved / deflected / open

### Competitor mentions
- [Competitor] — raised by [prospect/rep] — context: ...

### Buying signals
- ...

### Coachable moment
[One specific, constructively-framed observation, or "None significant this call."]
```

## What to avoid

- Don't infer objections or signals that aren't actually in the transcript — if the call is thin on one category, say so rather than padding it.
- Don't editorialize about whether the deal will close — this tool extracts signal, it doesn't forecast.

## Aggregate mode — rolling many calls into one view

Run the per-call breakdown above against every transcript first — the aggregate view is only as good as the individual extractions underneath it. Then:

1. **Count competitor mentions and objection types across the batch**, not just within one call — a single call's objection is an anecdote; the same objection across a third of the batch is a pattern worth a battlecard update.
2. **Separate "new information" from "confirmation of what's already documented."** A call restating a known competitor weakness is a data point; a call surfacing something not in `competitive-landscape.md`, `icp.md`, or any battlecard is the actually valuable output of this exercise, and deserves its own escalation, not a footnote.
3. **Tag each new finding with where it should go next** — product, compliance, data team, customer success, or a specific battlecard file — a finding with no owner tends to get read once and forgotten.
4. **Track open commitments across calls as their own list.** A rep's unfulfilled "I'll send that over" is a credibility risk at the account level, and it's invisible if each call is only ever read in isolation.
5. **Don't force a pattern that isn't there.** A recurring theme needs to show up independently across multiple accounts, not be inferred from one vivid call — see [`call-analysis-summary.html`](./call-analysis-summary.html) for the bar this needs to clear before something is presented as a pattern rather than an anecdote.

See [`call-analysis-summary.html`](./call-analysis-summary.html) for this mode applied to 15 real transcripts.
