# Personalized Outbound

## The problem

"Personalized" outbound usually means a first-name merge field on a template. Real personalization means the message is actually different because of something specific and true about this account — a real trigger, not a generic pain point restated with their logo. That takes more per-message effort than most outbound volume targets allow, unless the synthesis work (why this account, why now, what angle) has already been done upstream.

## The approach

A skill that takes an account brief (like the one [`abm-account-brief`](../../sales-tools/abm-account-brief) produces) and drafts one outbound message — email or LinkedIn — that references the actual trigger signal specifically, uses the positioning angle already selected for that account, and follows [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules. This deliberately does not generate outbound from scratch off a generic template; it requires the upstream brief as input, because the whole point is to not sound like outbound that could have been sent to any account.

Closes the loop on the pipeline demonstrated across three use cases: [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor) flags Nordkredit → [`abm-account-brief`](../../sales-tools/abm-account-brief) builds the account picture → this drafts the actual message.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`gpt.md`](./gpt.md) — ChatGPT custom GPT version
- [`example.md`](./example.md) — the Nordkredit × Head of Credit Risk outreach message
- [`example-nordkredit-vp-mortgage-lending.md`](./example-nordkredit-vp-mortgage-lending.md), [`example-court-street-lending-head-of-credit-risk.md`](./example-court-street-lending-head-of-credit-risk.md) — two more examples, see below

## The account × persona grid

Personalization here happens on two independent axes: the **account's specific trigger** (from its brief) and the **persona** being written to (from [`personas.md`](../../knowledge-base/personas.md)) — a good draft depends on both, and changing either one should visibly change the message, not just the name at the top. Three examples, each holding one axis fixed to isolate what the other one changes:

| Example | Account | Persona | Signal strength |
|---|---|---|---|
| [`example.md`](./example.md) | Nordkredit | Head of Credit Risk | Strong (two corroborating signals) |
| [`example-nordkredit-vp-mortgage-lending.md`](./example-nordkredit-vp-mortgage-lending.md) | Nordkredit (same) | VP of Mortgage Lending (different) | Strong (same signal, re-read through a different persona) |
| [`example-court-street-lending-head-of-credit-risk.md`](./example-court-street-lending-head-of-credit-risk.md) | Court Street Lending (different) | Head of Credit Risk (same) | Medium (weaker — one signal, not two) |

The third example also demonstrates a rule that isn't obvious from the first two alone: the *confidence* of the ask should track the strength of the underlying signal from [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor), not just its presence — a single uncorroborated signal earns a more exploratory message than a corroborated one, even for the same persona and the same positioning angle.

## Current limitations

Right now the account brief is pasted in manually. Pulling it directly from the CRM record, and logging the sent message back to the account timeline, is next.
