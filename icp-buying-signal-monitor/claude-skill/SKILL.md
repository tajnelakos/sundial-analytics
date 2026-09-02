---
name: icp-buying-signal-monitor
description: Scores raw signals about named accounts (exec hires, job postings, tech migrations, news) against defined ICP tiering and in-market signal criteria, producing a prioritized account watch list. Use when the user pastes signals about one or more accounts and wants them evaluated for buying readiness, not just logged.
---

# ICP Buying Signal Monitor

## Purpose

Turn raw, per-account signals into a ranked watch list, using the tiering and signal definitions already established in `strategy/icp.md` rather than judging fit ad hoc each time.

## Instructions

1. **Reference the ICP tiering criteria** (firmographics, technographics, geography — see `strategy/icp.md`) to first sanity-check the account is even in-segment. Don't score a signal for an account that doesn't fit the ICP at all — flag it as out-of-segment instead.
2. **Classify each signal by strength**, not just presence:
   - **Strong**: new risk/credit leadership hire, an announced audit finding, a job posting naming a specific legacy competitor tool
   - **Medium**: LOS/core system migration announced, executive turnover at a company using a competitor
   - **Weak**: generic hiring growth, unspecific "digital transformation" language
3. **One strong signal outranks several weak ones.** Don't average signal strength into a single score that hides this — a Weak+Weak+Weak account should not outrank a Strong-only account.
4. **State the specific evidence for every signal**, not just the classification — "job posting for Credit Risk Analyst mentions migrating off Estemate" is usable; "hiring activity" is not.
5. **Flag time sensitivity.** A signal tied to a dated event (e.g. "Q3 audit" from a hire announcement) matters more urgently than an undated one — surface the implied timeline if the signal contains one.
6. **Output a ranked list, not a report per account.** The point is prioritization across accounts, so someone can act on the top 2-3 rather than read through all of them.

## What to avoid

- Don't treat a single job posting or hire as certain proof of an active evaluation — these are signals worth watching, not confirmed intent. Say "worth outreach" not "about to buy."
- Don't score accounts outside the documented ICP tiers just because a signal exists — fit comes first, signal second.

## Output format

```
## Buying Signal Watch List — [date]

1. [Account name] — [Tier] — Signal strength: Strong
   Evidence: ...
   Time sensitivity: ...

(ranked, strongest/most time-sensitive first)

Out-of-segment (signal present, doesn't fit ICP): [account names, if any]
```
