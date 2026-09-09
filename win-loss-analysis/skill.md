---
name: win-loss-infographic
description: Analyzes a batch of closed-deal notes (close reasons, rep summaries, call excerpts) and produces a quantified win/loss breakdown rendered as a single-page infographic with concrete next actions. Use when the user has a batch of closed deals from one quarter/segment and wants patterns, not a deal-by-deal summary.
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
