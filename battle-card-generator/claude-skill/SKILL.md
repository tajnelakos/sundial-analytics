---
name: battle-card-generator
description: Synthesizes raw competitive research (win/loss notes, call mentions, reviews, pricing pages) about one competitor into a full battlecard section (positioning, strengths/weaknesses, how we win/lose, objection handling, trigger signals). Use when the user has accumulated raw material about a competitor and wants it turned into (or merged into) a structured battlecard, not a summary.
---

# Battle Card Generator

## Purpose

Produce a battlecard section in the same structure as `strategy/competitive-landscape.md`, so a new or updated competitor entry is immediately usable by a rep, not just a research summary someone else has to restructure later.

## Instructions

1. **Read all raw input before drafting anything.** A battlecard built section-by-section from partial input tends to produce a "weaknesses" list that contradicts the "how we lose" section, because they weren't reasoned about together.
2. **Every strength and weakness needs a source type**, even if brief (e.g. "per 3 lost deals," "per public reviews," "per rep-reported call mentions") — a battlecard where every claim looks equally certain gets misused in live calls.
3. **"How we win" and "how we lose" must be genuinely asymmetric** — if they read as mirror images of each other, the analysis hasn't gone deep enough. Losing usually isn't just "the opposite of winning circumstances."
4. **Objection handling must be an actual talk track**, not a restated fact. "They're cheaper" → what a rep should actually say, not just "we are more accurate."
5. **Trigger signals should be things a rep can notice in real time** on a call or in a deal (specific phrases, specific behaviors) — not abstract firmographic criteria.
6. **When updating an existing battlecard entry**, output only the changed sections plus a one-line note on what changed and why — don't regenerate the whole card silently.
7. **Flag low-confidence claims explicitly** rather than smoothing them into confident-sounding prose — a battlecard is worse than useless if a rep repeats an unverified claim to a prospect who can fact-check it.

## What to avoid

- Don't fabricate a strength or weakness to fill out the structure — an incomplete section is better than an invented one.
- Don't write objection handling that argues on price if the actual differentiation is elsewhere — redirect, don't compete on the competitor's chosen ground.

## Output format

Match the structure used in `strategy/competitive-landscape.md`: Positioning / Strengths / Weaknesses / How we win / How we lose / Objection handling / Trigger signals — each claim tagged with its source type.
