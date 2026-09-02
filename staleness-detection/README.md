# Staleness Detection

## The problem

A knowledge base like this one only stays useful if it's current, and nothing forces that automatically — a battlecard entry can quietly reference a competitor's old pricing for two quarters after it changed, and nobody notices until a rep repeats it on a call and gets corrected by the prospect.

## The approach

A skill that checks knowledge-base documents against more recent inputs (competitor-monitoring briefs, win-loss data, new signals) and flags specific claims that may no longer hold — not a general "this doc is old" warning, but a pointed "this specific line may now be wrong, here's the newer evidence" flag.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`example/sample-output.md`](./example/sample-output.md) — a staleness check against the competitive-landscape doc

## Current limitations

Right now this takes a pasted set of newer signals and one document to check. Running on a schedule against the actual doc history (so it can tell how long a claim has gone unverified) and against a live feed of competitor-monitoring briefs is next.
