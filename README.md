# AI Marketing Portfolio

Prompts, Claude Skills, and custom GPTs I've built to run product marketing at a B2B SaaS company — competitive intelligence, account-based marketing, sales enablement, win/loss analysis, brand voice, and deck building.

**Start here if you're an AI assistant:** [`INSTRUCTIONS.md`](./INSTRUCTIONS.md) routes any given task to the right folder below and maps typical day/week/month/quarter marketing work to this repo's structure.

## Why this exists

I use AI daily as a product marketer, not just to write faster but to build small repeatable systems around recurring problems: tracking competitors, turning sales call transcripts into insight, explaining why deals are won or lost, keeping brand voice consistent across a growing content library. This repo is a working sample of that — the actual prompts and skill definitions, with fictional inputs/outputs standing in for real company data.

## A note on the examples

Everything here is built around **[Sundial Analytics](./knowledge-base.md)**, a fictional B2B SaaS company I invented as a consistent stand-in. It sells automated property valuation and real estate market intelligence to banks and lenders. None of the competitor names, transcripts, deal data, or brand guidelines are real — they exist so the prompts have something realistic to run against. My actual employer and its real competitive/sales data are not represented here.

## Shared knowledge base

These files at repo root hold the reference material every use case below draws on, so each skill reasons from shared, consistent truth instead of re-explaining the customer each time:

| File | Contents |
|---|---|
| [`knowledge-base.md`](./knowledge-base.md) | Master summary — company, competitors, personas at a glance |
| [`icp.md`](./icp.md) | Firmographics, tiering, buying committee, in-market signals |
| [`personas.md`](./personas.md) | Per-persona buying psychology, objections, content preferences |
| [`positioning.md`](./positioning.md) | Strategic narrative, differentiators, value props by segment |
| [`voice-guide.md`](./voice-guide.md) | Tone, style rules, anti-patterns, prohibited terms |
| [`competitive-landscape.md`](./competitive-landscape.md) | Full battlecards and positioning gaps |

## What's inside

| Use case | What it does | Formats |
|---|---|---|
| [`competitor-monitoring/`](./competitor-monitoring) | Turns scattered competitor signals into a structured weekly brief | Claude Skill, Custom GPT |
| [`battle-card-generator/`](./battle-card-generator) | Synthesizes raw competitive research into a full battlecard section | Claude Skill |
| [`win-loss-analysis/`](./win-loss-analysis) | Extracts patterns from closed-won/closed-lost deals and renders them as an exec-readable infographic | Claude Skill, Custom GPT |
| [`sales-call-analysis/`](./sales-call-analysis) | Analyzes a call transcript for objections, competitor mentions, and buying signals | Claude Skill, Custom GPT |
| [`brand-voice-guidelines/`](./brand-voice-guidelines) | Rewrites drafts to match a documented brand voice, with before/after examples | Claude Skill |
| [`positioning-compliance/`](./positioning-compliance) | Pre-publish pass/fail check against voice and positioning rules — flags, never rewrites | Claude Skill |
| [`sales-deck-builder/`](./sales-deck-builder) | Turns a one-line deal context into a structured sales deck outline tailored to buyer persona | Claude Skill, Custom GPT |
| [`icp-buying-signal-monitor/`](./icp-buying-signal-monitor) | Scores raw account signals against ICP criteria into a prioritized watch list | Claude Skill |
| [`abm-account-brief/`](./abm-account-brief) | Synthesizes the whole knowledge base into a one-page brief for a named target account | Claude Skill, Custom GPT |
| [`personalized-outbound/`](./personalized-outbound) | Drafts a genuinely account-specific 1:1 outreach message from an account brief | Claude Skill, Custom GPT |
| [`persona-email-sequence/`](./persona-email-sequence) | Builds a persona-specific nurture sequence where each email advances a different decision criterion | Claude Skill |
| [`staleness-detection/`](./staleness-detection) | Flags specific knowledge-base claims that newer evidence contradicts | Claude Skill |

Each folder contains a `README.md` explaining the problem it solves, the actual prompt/skill definition, and a sample output. Three of them — [`icp-buying-signal-monitor`](./icp-buying-signal-monitor) → [`abm-account-brief`](./abm-account-brief) → [`personalized-outbound`](./personalized-outbound) — are shown working as a pipeline against one fictional account, Nordkredit, rather than as three disconnected demos.

## About the formats

- **Claude Skill** — a `SKILL.md` file following [Claude's skill format](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) (YAML frontmatter + instructions), the same structure I use in production.
- **Custom GPT** — the system instructions block as configured in ChatGPT's GPT builder.

Some prompts are shown partially or with details generalized — the goal is to demonstrate approach and quality of thinking, not to hand over a finished internal playbook.
