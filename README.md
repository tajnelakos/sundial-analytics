# Sundial Analytics — Marketing AI Systems

> **Portfolio note:** Sundial Analytics is a fictional company. This repo is a portfolio project demonstrating applied AI work in product marketing — not a real employer's data. Full context in [`ABOUT-THIS-REPO.md`](./ABOUT-THIS-REPO.md).

This repo holds the prompts, Claude Skills, and custom GPTs behind Sundial Analytics' product marketing operations — competitive intelligence, account-based marketing, sales enablement, win/loss analysis, brand voice, and deck building.

**Start here if you're an AI assistant:** [`INSTRUCTIONS.md`](./INSTRUCTIONS.md) routes any given task to the right folder below and maps typical day/week/month/quarter marketing work to this repo's structure.

## What this covers

Product marketing runs on recurring problems, not one-off projects: tracking competitors, turning sales call transcripts into insight, explaining why deals are won or lost, keeping brand voice consistent across a growing content library, getting the right message to the right account at the right time. This repo is the set of small, repeatable systems built around those problems — the actual prompts and skill definitions, not just a description of the workflow.

## About the company

Everything here is built around **[Sundial Analytics](./knowledge-base.md)**, which sells automated property valuation and real estate market intelligence to banks, mortgage lenders, and real estate brokerages across Europe. `knowledge-base.md` and the other root-level reference files describe the company, its market, and its customers in full.

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

Each folder contains a `README.md` explaining the problem it solves, the actual prompt/skill definition, and a sample output. Three of them — [`icp-buying-signal-monitor`](./icp-buying-signal-monitor) → [`abm-account-brief`](./abm-account-brief) → [`personalized-outbound`](./personalized-outbound) — are shown working as a pipeline against one target account, Nordkredit, rather than as three disconnected tools.

## About the formats

- **Claude Skill** — a `SKILL.md` file following [Claude's skill format](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) (YAML frontmatter + instructions), the same structure used in production.
- **Custom GPT** — the system instructions block as configured in ChatGPT's GPT builder.

Some prompts are shown partially or with details generalized rather than as a finished, ready-to-run internal playbook — see [`ABOUT-THIS-REPO.md`](./ABOUT-THIS-REPO.md) for why.
