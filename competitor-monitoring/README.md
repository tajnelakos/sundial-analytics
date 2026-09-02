# Competitor Monitoring

## The problem

Competitive intel usually shows up as noise: a pricing page change someone notices by accident, a G2 review a sales rep forwards, a changelog nobody reads end to end. Without a system, it either doesn't get synthesized at all, or it eats an afternoon every time someone asks "what's Bricklane doing lately?"

## The approach

A weekly-cadence skill that takes in raw, unstructured signals (pricing page snapshots, release notes, review site excerpts, sales call mentions) and produces one structured brief: what changed, why it matters for our positioning, and what — if anything — sales or product marketing should do about it. The goal is a brief a sales leader will actually read in three minutes, not a wall of bullet points.

Two constraints I built in on purpose:
- **No unverified claims.** If a signal is ambiguous (e.g. a pricing page number without context), the skill flags it as "needs confirmation" rather than asserting it.
- **"So what" is mandatory.** Every item must end with an implication, not just an observation — otherwise it's just news, not intelligence.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`custom-gpt/INSTRUCTIONS.md`](./custom-gpt/INSTRUCTIONS.md) — the same logic adapted as a ChatGPT custom GPT
- [`example/sample-output.md`](./example/sample-output.md) — a fictional weekly brief run against [Sundial Analytics](../knowledge-base.md)'s fictional competitors

## What's simplified from the real version

The production version pulls from a Slack channel where the team drops raw links/screenshots and a shared doc of past briefs (for trend continuity week over week). Here it takes plain pasted text instead, to keep the example self-contained.
