# Win/Loss Analysis

## The problem

Most win/loss "analysis" is a CRM close-reason dropdown nobody trusts, because reps pick whatever's fastest to log. The real reasons a deal was won or lost usually live in call notes, the final email exchange, and the rep's memory — and by the time someone tries to synthesize it quarterly, it's guesswork.

## The approach

A skill that takes in raw deal notes (CRM close reasons, rep summaries, call transcript excerpts) across a batch of closed deals and does two things:

1. **Classifies and quantifies** the real reasons behind wins and losses — not the dropdown reason, the actual one buried in the notes, reconciled against what the rep logged.
2. **Renders it as one infographic** an exec will actually look at, with a "what this means for product marketing" section — because a chart without an implication is just decoration.

The output is intentionally opinionated: it always ends in 2-3 concrete next actions (a battlecard update, a flag to product, a new case study angle), not just a breakdown of percentages.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`gpt.md`](./gpt.md) — ChatGPT custom GPT version
- [`win-loss-infographic.svg`](./win-loss-infographic.svg) — sample output, Q1 data for Sundial Analytics' banking segment ([view live ↗](https://tajnelakos.github.io/sundial-analytics/knowledge-base/win-loss-analysis/win-loss-infographic.svg))

![Win/loss infographic example](./win-loss-infographic.svg)

## Current limitations

Right now this takes pasted deal notes directly. Pulling from the CRM export and cross-referencing logged close reasons against transcript mentions to catch mismatches (e.g. rep logs "price" but the transcript shows the real blocker was a missing feature) is next.
