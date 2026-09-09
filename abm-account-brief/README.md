# ABM Account Brief

## The problem

For named target accounts, the useful version of "who are we selling to" isn't the generic persona doc — it's that persona doc applied to this specific account, with this account's specific likely committee, likely competitive risk, and the one or two positioning angles most relevant to what's actually going on there. Building that by hand means re-reading four different reference docs and holding it all in your head; it rarely happens consistently.

## The approach

A skill that takes a named account (plus whatever's known about it — firmographics, a buying signal, prior contact) and pulls together one brief by applying [`icp.md`](../icp.md), [`personas.md`](../personas.md), [`positioning.md`](../positioning.md), and [`competitive-landscape.md`](../competitive-landscape.md) to that specific account — rather than restating any of them generically. This is the use case that most depends on the shared knowledge-base files actually being good, since the brief is only as sharp as the synthesis across all four files.

This example continues the account flagged by [`icp-buying-signal-monitor`](../icp-buying-signal-monitor) (Nordkredit) and feeds [`personalized-outbound`](../personalized-outbound).

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`gpt.md`](./gpt.md) — ChatGPT custom GPT version
- [`example.md`](./example.md) — the Nordkredit brief

## Current limitations

Right now account facts are given directly in the prompt. Pulling firmographic data from an enrichment tool and past CRM activity automatically is next.
