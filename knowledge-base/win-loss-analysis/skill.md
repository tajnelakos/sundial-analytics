---
name: win-loss-infographic
description: Analyzes a batch of closed-deal notes (close reasons, rep summaries, call excerpts) and produces a quantified win/loss breakdown rendered as a single-page infographic with concrete next actions. Use when the user has a batch of closed deals from one quarter/segment and wants patterns, not a deal-by-deal summary. Also supports a deep-dive mode against a structured CRM export — see below.
---

# Win/Loss Infographic

## Purpose

Turn a pile of closed-deal notes into one page an exec will read: what we actually win and lose on, quantified, with a mandatory "what to do about it" section.

## Instructions

1. **Read every deal note before classifying anything.** Don't classify off the CRM close-reason field alone — it's frequently a rep's shorthand, not the real reason. If the notes suggest a different or additional reason than the logged one, use what the notes actually support.
2. **Build two ranked lists**: top reasons deals were won, top reasons deals were lost. Each reason should be specific enough to act on ("no on-prem deployment option") not generic ("product gap").
3. **Cap each list at 4-5 reasons.** Group anything smaller into "Other" rather than listing every one-off reason — a list of 12 reasons is not a pattern, it's a data dump.
4. **Compute percentages against total won / total lost**, not total deals — win reasons should sum to ~100% of wins, loss reasons to ~100% of losses.
5. **Note competitor concentration**: if losses cluster against one competitor, call that out explicitly — a 38% loss-to-price rate means something different if it's all against one aggressively-priced competitor vs. spread evenly.
6. **Compare to the prior period if data is available.** A reason that jumped in rank (e.g. "missing on-prem" moving from #4 to #2) is often more actionable than the current #1, because it signals a new or growing blocker.
7. **End with 2-3 concrete next actions**, each tied to a specific finding, addressed to a specific function (sales enablement, product, content). Never end on the chart alone — an unquantified "so what" is a required section, not optional color commentary.
8. **Render as a single infographic**: header stat row (win rate, deals analyzed, top competitor), two horizontal bar sections (won / lost reasons), and a takeaway panel. Use one hue for the "won" bars and a different single hue for "lost" bars — this is categorical-by-section, not a multi-series legend.

## What to avoid

- Don't editorialize about individual reps or deals — this is a pattern-level analysis, not a performance review.
- Don't present a reason as quantified if fewer than ~5 deals support it — note it as anecdotal instead, or omit it.
- Don't recommend pricing changes directly — flag pricing pressure as a finding for the pricing/product team to act on, not a decision this skill makes.

## Deep-dive mode — structured CRM export

The infographic above is built for a quarterly, exec-facing cadence. This mode is for a deeper, less frequent pass against an actual CRM export (deal size, sales cycle, lead source, assigned rep, and outcome per opportunity) — a richer input deserves a richer output, not the same one-page infographic with more rows squeezed in.

1. **Compute every statistic from the export, never estimate it.** If a number appears in the output (a win rate, an average deal size, a percentage), it must trace to a real aggregation over real rows — this mode's entire value is that its numbers are computed, not asserted.
2. **Structure the analysis around five core components**, each a real section, not a paragraph: **Buyer Demographics** (company size, industry/segment, current tech stack), **Decision Drivers** (why the buyer chose us or a competitor), **Competitor Data** (who we faced, their quoted price if known, their perceived strength), **Product Feedback** (missing features or bugs behind losses, standout features behind wins), and **Sales Process Insights** (rep performance, response time, demo quality).
3. **Pull in [`sales-call-analysis`](../sales-call-analysis) as a second data source where it exists.** A CRM export tells you *that* a deal was lost to price; a call transcript tells you *how* that conversation actually went. Cite the transcript directly rather than re-deriving what it already shows.
4. **Look for findings that cut across components**, not just within one — e.g. whether the deals we lose tend to be larger than the ones we win, or whether response time (a process metric) predicts outcome better than demo quality (also a process metric) does. These cross-cutting findings are usually more useful than any single component's breakdown.
5. **Flag a 0%-win-rate segment as urgent, not as a footnote.** A competitor or condition with an extreme result on a small sample is still worth surfacing prominently — just say the sample size plainly rather than either hiding it or overstating its certainty.
6. **Never let a rep-performance finding read as a performance review of a named individual.** Report the aggregate pattern (e.g. response time correlating with win rate across the team) and, if a specific rep's documented work elsewhere contradicts a shallow read of their aggregate numbers, say so explicitly rather than leaving the contradiction for the reader to notice.
7. **Render as a full analysis page**, not a single infographic — this mode has too much real structure (five components, cross-cutting findings, source citations) to compress into one exec-glance visual. See [`win-loss-detailed-analysis.html`](./win-loss-detailed-analysis.html).
