---
name: staleness-detection
description: Sweeps the knowledge base (and, where relevant, sales-tools artifacts built from it) against this repo's own most recent evidence — the latest competitor-monitoring brief, win-loss deep dive, and sales-call-analysis rollup — and flags or, where safe, directly updates specific claims that evidence now contradicts. Use monthly, or whenever a major new artifact (a bi-monthly report, a fresh CRM export) lands. Also supports the original single-doc, single-input mode for an ad hoc check.
---

# Staleness Detection

## Purpose

Flag specific, potentially-outdated claims with their contradicting evidence — never a vague "this might be old" warning, which nobody can act on. Where the fix is a simple, unambiguous factual update (a date, a stat, a status), make it directly rather than only flagging it; where it requires real judgment (rewriting a talk track, changing a strategic recommendation), route it to the skill that owns that judgment instead of guessing.

## Repo-wide sweep mode (the primary mode — run this monthly)

1. **Gather the evidence sources first, all of them, before touching any target doc:**
   - The latest [`competitor-monitoring`](../../sales-tools/competitor-monitoring) bi-monthly report
   - The latest [`win-loss-analysis`](../win-loss-analysis) deep dive (CSV + HTML)
   - The [`sales-call-analysis`](../sales-call-analysis) rollup
   - Any other artifact newer than the target doc's own "Last verified" or "Last updated" date
2. **Check every doc that makes a factual claim about the market, a competitor, or a customer against those sources**, at minimum: `competitive-landscape.md`, each file in [`battlecard`](../../sales-tools/battlecard), `positioning.md`, `icp.md`, `personas.md`. Go claim by claim within each — a staleness check is only useful at the level of individual factual assertions, not whole sections.
3. **Classify every finding into one of three actions, not two:**
   - **Direct fix** — a simple, unambiguous factual update (a "Last verified" date, a statistic, a status like "beta" → "GA"). Make the edit yourself, and say plainly in the sweep report that you did, with the old and new value.
   - **Route to a generator skill** — anything requiring judgment about phrasing, strategy, or talk tracks (a battlecard's objection-handling copy, a positioning narrative). Name the specific skill and file; don't attempt the rewrite yourself.
   - **Soft flag** — unverified but not contradicted by anything in hand; worth a recheck next sweep, not urgent now.
4. **Look for evidence that *strengthens* a claim, not only evidence that contradicts one.** A new data point that confirms and sharpens an existing claim (e.g. a battlecard's qualitative argument now has a hard statistic behind it) is worth adding even though nothing was "wrong" — staleness isn't only about errors, it's about a knowledge base falling behind what's actually known.
5. **Cite the specific source** for every finding — a rep or writer needs to see the evidence, not just trust the flag.
6. **Produce one sweep report** covering everything checked this pass, structured by target document, not by evidence source — see [`sweep-2026-09.md`](./sweep-2026-09.md) for the format and a real worked pass.

## Single-document mode (ad hoc check)

For checking one document against a specific set of newer inputs someone hands you directly, without running the full sweep above:

1. **Go claim by claim through the target document.**
2. **Compare each claim against the newer inputs provided.** Only flag a claim if a newer input actually contradicts or updates it — don't flag a claim just because it's old if nothing newer speaks to it either way.
3. **Distinguish "contradicted" from "unverified but plausibly still true."** A claim with direct newer evidence against it is a hard flag. A claim that simply hasn't been re-confirmed recently, with no evidence either way, is a soft flag.
4. **Cite the specific newer input** that triggers each flag.
5. **Do not rewrite the flagged claim in this mode** — route hard flags to the appropriate generator skill instead (e.g. a stale competitor claim → `battlecard`; a stale persona claim → note it for `personas.md`'s owner). This mode is detection-only; the repo-wide sweep above is the one that also applies direct fixes.
6. **If nothing is flagged, say so plainly** — don't manufacture a soft flag just to show the check did something.

See [`example.md`](./example.md) for this mode.

## What to avoid

- Don't flag a claim as stale just because no explicit "last verified" date exists — absence of a date isn't evidence of inaccuracy.
- Don't treat this as a style or quality review — that's out of scope; this only checks factual currency.
- Don't apply a "direct fix" to anything that changes a recommendation, a talk track, or a strategic argument — if it takes judgment, it's a route, not a fix, no matter how confident you are.

## Output format — sweep report

```
## Staleness Sweep — [date]

Evidence reviewed: [list of sources and their dates]

### [Target document 1]
- **Direct fix applied:** "[old claim]" → "[new claim]" — Source: [evidence] — [date/detail of the edit made]
- **Routed to [skill/owner]:** "[claim]" — Source: [evidence] — Why this needs judgment, not a direct edit
- **Soft flag:** "[claim]" — no contradicting evidence yet, last supported by [evidence/date]

(repeat per document checked; state "Nothing to report" for scanned-but-clean documents)
```

## Output format — single-document mode

```
## Staleness Check — [document checked] — against [newer inputs, briefly described]

### Hard flags (contradicted by newer evidence)
- Claim: "[quoted claim]" — Contradicted by: [specific newer input] — Recommended action: [route to which skill/owner]

### Soft flags (unverified, no contradicting evidence, worth a recheck)
- Claim: "[quoted claim]" — Last supporting evidence: [what it was, if known]

(If none in a category, state "None found.")
```
