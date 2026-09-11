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

This skill has no scheduler of its own — nothing in a markdown file can trigger anything. It runs when a person (or an automation someone builds outside this repo) invokes it. In this repo, that invocation is a monthly scheduled task — see the note in `INSTRUCTIONS.md`'s cadence section — that hands Claude this skill plus the repo's latest artifacts each month.

## Current limitations

The repo-wide sweep still requires someone (or a scheduled run) to point it at the current state of the repo each time — it doesn't yet diff against its own prior sweep report to know what changed since last time versus what's simply unconfirmed again. Building that comparison (this sweep vs. last sweep, not just this sweep vs. the underlying docs) is the natural next step.
