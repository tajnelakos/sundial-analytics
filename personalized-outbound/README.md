# Personalized Outbound

## The problem

"Personalized" outbound usually means a first-name merge field on a template. Real personalization means the message is actually different because of something specific and true about this account — a real trigger, not a generic pain point restated with their logo. That takes more per-message effort than most outbound volume targets allow, unless the synthesis work (why this account, why now, what angle) has already been done upstream.

## The approach

A skill that takes an account brief (like the one [`abm-account-brief`](../abm-account-brief) produces) and drafts one outbound message — email or LinkedIn — that references the actual trigger signal specifically, uses the positioning angle already selected for that account, and follows [`voice-guide.md`](../voice-guide.md). This deliberately does not generate outbound from scratch off a generic template; it requires the upstream brief as input, because the whole point is to not sound like outbound that could have been sent to any account.

Closes the loop on the pipeline demonstrated across three use cases: [`icp-buying-signal-monitor`](../icp-buying-signal-monitor) flags Nordkredit → [`abm-account-brief`](../abm-account-brief) builds the account picture → this drafts the actual message.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`custom-gpt/INSTRUCTIONS.md`](./custom-gpt/INSTRUCTIONS.md) — ChatGPT custom GPT version
- [`example/sample-output.md`](./example/sample-output.md) — the Nordkredit outreach message

## Current limitations

Right now the account brief is pasted in manually. Pulling it directly from the CRM record, and logging the sent message back to the account timeline, is next.
