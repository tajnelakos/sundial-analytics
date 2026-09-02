# ICP Buying Signal Monitor

## The problem

[`icp.md`](../icp.md) documents what an in-market signal looks like (exec hires, job postings mentioning a specific legacy tool, LOS migrations, adverse audit findings). Documenting it isn't the hard part — noticing it happen, for the right accounts, before a competitor does, is. Left as a static doc, it's just knowledge; it needs to run against real signal sources on a cadence to be useful.

## The approach

A skill that takes raw signals about named accounts (job postings, LinkedIn hires, news mentions, review site activity) and scores them against the tiering and signal criteria already defined in `icp.md` — rather than re-deriving "what counts as a signal" from scratch each time. Output is a prioritized watch list, not a raw signal dump: an account with one strong signal (new Head of Credit Risk hire) outranks one with three weak ones.

This is the first step in a small pipeline demonstrated across three use cases: a flagged account here feeds [`abm-account-brief`](../abm-account-brief) (build the full picture) and [`personalized-outbound`](../personalized-outbound) (act on it) — see the [Nordkredit example](./example/sample-output.md) carried through both.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`example/sample-output.md`](./example/sample-output.md) — fictional signals scored for a fictional target account, Nordkredit

## What's simplified from the real version

The production version pulls from a job-posting scraper and a news/LinkedIn monitoring tool on a weekly cron, and writes flagged accounts into the CRM as a task for the account's owner. Here it takes pasted signals and returns a scored list, to keep the example self-contained.
