# Battle Card Generator

## The problem

[`competitive-landscape.md`](../competitive-landscape.md) is the finished artifact. This is the tool that builds and refreshes it: raw competitive research (win/loss notes, sales call mentions, public reviews, pricing pages) rarely arrives pre-organized into a battlecard — someone has to synthesize it into the strengths/weaknesses/objection-handling structure a rep can use live on a call.

This is distinct from [`competitor-monitoring`](../competitor-monitoring), which tracks what *changed this week*. This tool builds or refreshes the whole evergreen document from accumulated raw material.

## The approach

A skill that takes a pile of raw competitive inputs about one competitor and produces (or updates) a full battlecard section in the same structure as `competitive-landscape.md` — positioning, strengths, weaknesses, how we win/lose, objection handling, trigger signals. When updating an existing card, it's explicit about what changed and why, rather than silently overwriting.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`example.md`](./example.md) — a battlecard built from raw notes about a competitor

## Current limitations

Right now this runs as a single generation pass. Automatically cross-referencing new input against the existing battlecard and flagging contradictions (e.g. new win/loss data suggesting a weakness entry no longer holds) is next.
