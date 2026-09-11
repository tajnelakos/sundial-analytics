# Staleness Detection

## The problem

A knowledge base like this one only stays useful if it's current, and nothing forces that automatically — a battlecard entry can quietly reference a competitor's old pricing for two quarters after it changed, and nobody notices until a rep repeats it on a call and gets corrected by the prospect.

## The approach

Two modes: a **repo-wide sweep** that checks every knowledge-base doc and relevant battlecard against this repo's own newest artifacts (the latest competitor-monitoring report, win-loss deep dive, sales-call-analysis rollup) and applies direct fixes where the update is a simple factual correction — not just a general "this doc is old" warning, but a pointed "this specific line was wrong, here's what it says now and why." And a **single-document, ad hoc mode** for checking one doc against a specific set of newer inputs someone hands over directly.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition, covering both modes
- [`sweep-2026-09.md`](./sweep-2026-09.md) — a real repo-wide sweep, run for real, with the fixes actually applied — see [`competitive-landscape.md`](../competitive-landscape.md), [`positioning.md`](../positioning.md), and the [ValuAI](../../sales-tools/battlecard/valuai.html) and [Estemate](../../sales-tools/battlecard/estemate.html) battlecards for the results
- [`example.md`](./example.md) — the single-document mode, a smaller ad hoc check against pasted inputs

## How it actually runs

A skill file has no scheduler of its own — nothing in markdown can trigger anything by itself. This one is invoked by an actual scheduled cloud routine, live as of September 2026: **"Sundial Analytics – Monthly Staleness Sweep,"** firing on the 1st of every month. It clones this repo fresh, reads `skill.md`'s repo-wide sweep mode, checks the knowledge base against whatever's newest, and — only if it actually finds something to fix — commits its changes to a new branch and opens a pull request for review. It never pushes straight to `main`; a monthly automated content change to a public portfolio gets a human look first.

If a given month's evidence hasn't changed since the last sweep (nothing new in `competitor-monitoring`, `win-loss-analysis`, or `sales-call-analysis`), the routine says so plainly and opens no PR at all, rather than manufacturing a finding to look useful — confirmed in its first test run, which correctly found nothing new (the manual [`sweep-2026-09.md`](./sweep-2026-09.md) pass had happened minutes earlier) and exited cleanly with no duplicate report and no PR.

## Current limitations

The monthly routine handles invocation now, but the sweep itself still re-derives "what's new since last time" by checking file modification history each run, rather than reading a structured diff against its own prior report. That's worked correctly so far, but it's inference, not a guarantee — a more explicit this-sweep-vs-last-sweep comparison is the natural next step.
