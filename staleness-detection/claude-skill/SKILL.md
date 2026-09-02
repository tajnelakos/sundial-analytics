---
name: staleness-detection
description: Checks a strategy/ knowledge base document against more recent inputs (competitor-monitoring briefs, win-loss data, new signals) and flags specific claims that may no longer be accurate, with the newer evidence cited. Use when the user wants to know if a reference doc needs a refresh, not a general content audit.
---

# Staleness Detection

## Purpose

Flag specific, potentially-outdated claims with their contradicting evidence — never a vague "this might be old" warning, which nobody can act on.

## Instructions

1. **Go claim by claim through the target document** — a staleness check is only useful at the level of individual factual assertions (a price point, a feature status, a "top loss reason"), not at the level of whole sections.
2. **Compare each claim against the newer inputs provided.** Only flag a claim if a newer input actually contradicts or updates it — don't flag a claim just because it's old if nothing newer speaks to it either way.
3. **Distinguish "contradicted" from "unverified but plausibly still true."** A claim with direct newer evidence against it is a hard flag. A claim that simply hasn't been re-confirmed recently, with no evidence either way, is a soft flag — worth a periodic recheck, not urgent.
4. **Cite the specific newer input** that triggers each flag — a rep or writer needs to see the evidence, not just trust the flag.
5. **Do not rewrite the flagged claim.** Route hard flags to the appropriate generator skill instead (e.g. a stale competitor claim → `battle-card-generator`; a stale persona claim → note it for `strategy/personas.md`'s owner) — this skill's job is detection, not correction.
6. **If nothing is flagged, say so plainly** — don't manufacture a soft flag just to show the check did something.

## What to avoid

- Don't flag a claim as stale just because no explicit "last verified" date exists — absence of a date isn't evidence of inaccuracy.
- Don't treat this as a style or quality review — that's out of scope; this only checks factual currency.

## Output format

```
## Staleness Check — [document checked] — against [newer inputs, briefly described]

### Hard flags (contradicted by newer evidence)
- Claim: "[quoted claim]" — Contradicted by: [specific newer input] — Recommended action: [route to which skill/owner]

### Soft flags (unverified, no contradicting evidence, worth a recheck)
- Claim: "[quoted claim]" — Last supporting evidence: [what it was, if known]

(If none in a category, state "None found.")
```
