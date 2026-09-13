# Sundial Analytics — Marketing AI Systems

> **Portfolio note:** Sundial Analytics is a fictional company. This repo is a portfolio project demonstrating applied AI work in product marketing — not a real employer's data. Full context in [`ABOUT-THIS-REPO.md`](./ABOUT-THIS-REPO.md).

This repo holds the prompts, Claude Skills, and custom GPTs behind Sundial Analytics' product marketing operations — competitive intelligence, account-based marketing, sales enablement, win/loss analysis, brand voice, and deck building.

**Start here if you're an AI assistant:** [`INSTRUCTIONS.md`](./INSTRUCTIONS.md) routes any given task to the right folder below and maps typical day/week/month/quarter marketing work to this repo's structure.

## What this covers

Product marketing runs on recurring problems, not one-off projects: tracking competitors, turning sales call transcripts into insight, explaining why deals are won or lost, keeping brand voice consistent across a growing content library, getting the right message to the right account at the right time. This repo is the set of small, repeatable systems built around those problems — the actual prompts and skill definitions, not just a description of the workflow.

## About the company

Everything here is built around **[Sundial Analytics](./knowledge-base/knowledge-base.md)**, which sells automated property valuation and real estate market intelligence to banks, mortgage lenders, and real estate brokerages across Europe. [`knowledge-base/`](./knowledge-base) describes the company, its market, and its customers in full.

## Three kinds of folder

- **[`knowledge-base/`](./knowledge-base)** — accumulated understanding: the core reference docs (company, ICP, personas, positioning, voice, competitive landscape), plus the analysis work that builds and maintains that understanding (call analysis, win/loss analysis, staleness detection).
- **[`sales-tools/`](./sales-tools)** — what a rep or sales-facing process actually uses: competitor monitoring, battlecards, account briefs, buying-signal monitoring, deck building.
- **[`marketing-assets/`](./marketing-assets)** — content marketing produces and ships: outbound messages, nurture sequences, case studies, one-pagers, blog posts, social posts, and the pre-publish compliance check.

### `knowledge-base/`

| File | Contents |
|---|---|
| [`knowledge-base.md`](./knowledge-base/knowledge-base.md) | Master summary — company, competitors, personas at a glance |
| [`icp.md`](./knowledge-base/icp.md) | Firmographics, tiering, buying committee, in-market signals |
| [`personas.md`](./knowledge-base/personas.md) | Per-persona buying psychology, objections, content preferences |
| [`positioning.md`](./knowledge-base/positioning.md) | Strategic narrative, differentiators, value props by segment |
| [`branding-guideline/`](./knowledge-base/branding-guideline) | Full brand system — mission, values, tone-by-channel, logo files, color palette, typography, naming conventions — plus the rewrite skill that applies the voice rules |
| [`competitive-landscape.md`](./knowledge-base/competitive-landscape.md) | Full battlecards and positioning gaps |
| [`sales-call-analysis/`](./knowledge-base/sales-call-analysis) | 15 call transcripts plus a [designed rollup](https://tajnelakos.github.io/sundial-analytics/knowledge-base/sales-call-analysis/call-analysis-summary.html) of objections, competitors, and new findings across them |
| [`win-loss-analysis/`](./knowledge-base/win-loss-analysis) | Patterns from closed-won/closed-lost deals — a quarterly infographic, plus a [100-record CRM deep dive](https://tajnelakos.github.io/sundial-analytics/knowledge-base/win-loss-analysis/win-loss-detailed-analysis.html) |
| [`staleness-detection/`](./knowledge-base/staleness-detection) | Flags specific knowledge-base claims that newer evidence contradicts |

### `sales-tools/`

| Folder | What it does | Formats |
|---|---|---|
| [`competitor-monitoring/`](./sales-tools/competitor-monitoring) | A structured weekly brief, plus a sourced [bi-monthly deep-dive](https://tajnelakos.github.io/sundial-analytics/sales-tools/competitor-monitoring/bi-monthly-report-2026-07-08.html) | Claude Skill, Custom GPT |
| [`battlecard/`](./sales-tools/battlecard) | A designed, rep-facing HTML battlecard per tracked competitor | Claude Skill |
| [`abm-account-brief/`](./sales-tools/abm-account-brief) | Synthesizes the whole knowledge base into a one-page brief for a named target account | Claude Skill, Custom GPT |
| [`icp-buying-signal-monitor/`](./sales-tools/icp-buying-signal-monitor) | Scores raw account signals against ICP criteria into a prioritized watch list | Claude Skill |
| [`sales-deck-builder/`](./sales-tools/sales-deck-builder) | Turns a one-line deal context into a structured sales deck outline tailored to buyer persona | Claude Skill, Custom GPT |

### `marketing-assets/`

| Folder | What it does | Formats |
|---|---|---|
| [`personalized-outbound/`](./marketing-assets/personalized-outbound) | Drafts a genuinely account-specific 1:1 outreach message from an account brief | Claude Skill, Custom GPT |
| [`persona-email-sequence/`](./marketing-assets/persona-email-sequence) | Builds a persona-specific nurture sequence where each email advances a different decision criterion | Claude Skill |
| [`case-study-builder/`](./marketing-assets/case-study-builder) | Builds a Challenge/Solution/Results case study from a real closed-won deal's CRM record and call transcript — never an invented result or quote | Claude Skill |
| [`one-pager-builder/`](./marketing-assets/one-pager-builder) | Builds a single-page, persona-specific leave-behind — one angle, sourced proof points, an actual designed HTML page | Claude Skill |
| [`blog-post-builder/`](./marketing-assets/blog-post-builder) | Drafts a blog post built around one real, sourced point of view or finding, not a generic SEO topic | Claude Skill |
| [`social-media-post-builder/`](./marketing-assets/social-media-post-builder) | Drafts a social post built around one real, cited proof point, platform mechanics applied after | Claude Skill |
| [`positioning-compliance/`](./marketing-assets/positioning-compliance) | Pre-publish pass/fail check against voice and positioning rules — flags, never rewrites | Claude Skill |

Each folder contains a `README.md` explaining the problem it solves, the actual prompt/skill definition, and a sample output. Three of them — [`icp-buying-signal-monitor`](./sales-tools/icp-buying-signal-monitor) → [`abm-account-brief`](./sales-tools/abm-account-brief) → [`personalized-outbound`](./marketing-assets/personalized-outbound) — are shown working as a pipeline against one target account, Nordkredit, rather than as three disconnected tools; [`case-study-builder`](./marketing-assets/case-study-builder) picks that same account back up as the pipeline's actual closed-won ending.

## About the formats

- **Claude Skill** — a `SKILL.md` file following [Claude's skill format](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) (YAML frontmatter + instructions), the same structure used in production.
- **Custom GPT** — the system instructions block as configured in ChatGPT's GPT builder.

Some prompts are shown partially or with details generalized rather than as a finished, ready-to-run internal playbook — see [`ABOUT-THIS-REPO.md`](./ABOUT-THIS-REPO.md) for why.
