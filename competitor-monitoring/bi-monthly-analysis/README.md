# Bi-Monthly Competitive Intelligence Report

## The problem

A weekly brief (see [`../claude-skill/SKILL.md`](../claude-skill/SKILL.md)) is built for speed — synthesize whatever came in this week. It's not built to be a citable reference six months later, and it's not the format a VP wants to skim before a board update. Some competitive intelligence needs a slower, more rigorous cadence: every claim dated and sourced, a fixed structure so period N is actually comparable to period N-1, and a version that's genuinely pleasant to open rather than another wall of bullets.

## The approach

This is adapted from a real prompt used for a similar recurring report at a proptech company, genericized here (competitors and region swapped out — this version is region-agnostic rather than tracking one market) and with one deliberate change: the original is kept strictly neutral, no strategic framing at all, because a trusted intelligence function shouldn't read as one person's opinion. This version adds a **Market Patterns** and **Strategic Signals** section on top of that neutral base — seeing the synthesis step, not just the monitoring step, is more useful for a portfolio.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the skill definition
- [`example/report-2026-07-08.md`](./example/report-2026-07-08.md) — the July–August 2026 report, written up
- [`example/report-2026-07-08.html`](./example/report-2026-07-08.html) — the same report as a designed, one-page HTML version

## Current limitations

Right now this is run manually against pasted or researched material per period. Automatically diffing this period's claims against the prior period's (so a repeated claim gets flagged rather than silently re-verified from scratch) is next.
