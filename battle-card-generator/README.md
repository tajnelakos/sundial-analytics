# Battle Card Generator

## The problem

[`strategy/competitive-landscape.md`](../strategy/competitive-landscape.md) is the finished artifact. This is the tool that builds and refreshes it: raw competitive research (win/loss notes, sales call mentions, public reviews, pricing pages) rarely arrives pre-organized into a battlecard — someone has to synthesize it into the strengths/weaknesses/objection-handling structure a rep can use live on a call.

This is distinct from [`competitor-monitoring`](../competitor-monitoring), which tracks what *changed this week*. This tool builds or refreshes the whole evergreen document from accumulated raw material.

## The approach

A skill that takes a pile of raw competitive inputs about one competitor and produces (or updates) a full battlecard section in the same structure as `strategy/competitive-landscape.md` — positioning, strengths, weaknesses, how we win/lose, objection handling, trigger signals. When updating an existing card, it's explicit about what changed and why, rather than silently overwriting.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`example/sample-output.md`](./example/sample-output.md) — a battlecard built from raw notes about a fictional competitor

## What's simplified from the real version

The production version cross-references new input against the existing battlecard automatically and flags contradictions (e.g. new win/loss data suggesting a "weakness" entry may no longer hold). Here it's a single generation pass, to keep the example self-contained.
