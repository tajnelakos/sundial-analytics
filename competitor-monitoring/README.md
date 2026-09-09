# Competitor Monitoring

## The problem

Competitive intel usually shows up as noise: a pricing page change someone notices by accident, a G2 review a sales rep forwards, a changelog nobody reads end to end. Without a system, it either doesn't get synthesized at all, or it eats an afternoon every time someone asks "what's Bricklane doing lately?"

## The approach

A weekly-cadence skill that takes in raw, unstructured signals (pricing page snapshots, release notes, review site excerpts, sales call mentions) and produces one structured brief: what changed, why it matters for our positioning, and what — if anything — sales or product marketing should do about it. The goal is a brief a sales leader will actually read in three minutes, not a wall of bullet points.

Two constraints are built in on purpose:
- **No unverified claims.** If a signal is ambiguous (e.g. a pricing page number without context), the skill flags it as "needs confirmation" rather than asserting it.
- **"So what" is mandatory.** Every item must end with an implication, not just an observation — otherwise it's just news, not intelligence.

## Files — weekly brief

- [`weekly-brief-skill.md`](./weekly-brief-skill.md) — the Claude Skill definition
- [`weekly-brief-gpt.md`](./weekly-brief-gpt.md) — the same logic adapted as a ChatGPT custom GPT
- [`weekly-brief-example.md`](./weekly-brief-example.md) — a weekly brief run against [Sundial Analytics](../knowledge-base.md)'s competitors

## Files — bi-monthly deep-dive

A slower, deeper cadence for the same competitor set — sourced and comparable-over-time rather than a fast weekly synthesis (see [`bi-monthly-report-skill.md`](./bi-monthly-report-skill.md) for how and why it differs from the brief above).

- [`bi-monthly-report-skill.md`](./bi-monthly-report-skill.md) — the skill definition
- [`bi-monthly-report-2026-07-08.md`](./bi-monthly-report-2026-07-08.md) — the July–August 2026 report, written up
- [`bi-monthly-report-2026-07-08.html`](./bi-monthly-report-2026-07-08.html) — the same report as a designed, one-page HTML version

## Current limitations

Right now this takes plain pasted text. Pulling from the Slack channel where the team drops raw links/screenshots, and referencing the shared doc of past briefs for trend continuity week over week, is next.
