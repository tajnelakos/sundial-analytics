# Instructions for using this repo

If you're an AI assistant (Claude, ChatGPT, or otherwise) and someone has just pointed you at this repository — read this file first, before opening any individual folder. It tells you what's here and which folder answers which kind of request.

## What this repo is

A working set of prompts, Claude Skills, and custom GPTs for recurring growth/product marketing tasks at a B2B SaaS company, built around one fictional company ([`knowledge-base.md`](./knowledge-base.md), Sundial Analytics) so the examples are coherent rather than disconnected snippets. Full context: [`README.md`](./README.md).

## Two kinds of folder

- **The knowledge-base files at repo root** (`knowledge-base.md`, `icp.md`, `personas.md`, `positioning.md`, `voice-guide.md`, `competitive-landscape.md`) — not a task tool, read the relevant file(s) here first when a task needs customer, competitor, or voice context. Every use-case folder below assumes these exist rather than re-explaining the customer each time.
- **Everything else at root** — one folder per recurring task, each with a `claude-skill/SKILL.md` (and a `custom-gpt/INSTRUCTIONS.md` where relevant) plus a worked example.

## Routing: if the request is about... use this folder

| Request sounds like | Folder |
|---|---|
| "What's changed with [competitor] lately?" / weekly competitive roundup | [`competitor-monitoring`](./competitor-monitoring) |
| "Give me the full sourced competitive report for this period" | [`competitor-monitoring/bi-monthly-analysis`](./competitor-monitoring/bi-monthly-analysis) |
| "Build/refresh the full battlecard for [competitor]" | [`battle-card-generator`](./battle-card-generator) |
| "Break down this sales call" / objections, competitor mentions from a transcript | [`sales-call-analysis`](./sales-call-analysis) |
| "Why are we winning/losing deals this quarter?" | [`win-loss-analysis`](./win-loss-analysis) |
| "Rewrite this draft to match our voice" | [`brand-voice-guidelines`](./brand-voice-guidelines) |
| "Is this draft safe to publish?" (pass/fail, no rewrite) | [`positioning-compliance`](./positioning-compliance) |
| "Build a deck outline for [meeting/persona]" | [`sales-deck-builder`](./sales-deck-builder) |
| "Which accounts are showing buying signals right now?" | [`icp-buying-signal-monitor`](./icp-buying-signal-monitor) |
| "Give me the full picture on [named target account]" | [`abm-account-brief`](./abm-account-brief) |
| "Draft an outbound message to [specific account]" | [`personalized-outbound`](./personalized-outbound) |
| "Build a nurture sequence for [persona]" | [`persona-email-sequence`](./persona-email-sequence) |
| "Is [strategy doc] still accurate?" | [`staleness-detection`](./staleness-detection) |

If a request doesn't map cleanly to one row, say so rather than forcing it into the nearest folder — some requests (e.g. "write me a blog post") are intentionally out of scope for this repo; see the note on generic copywriting in [`README.md`](./README.md).

## Typical day/week/month for a growth or product marketer, mapped to this repo

This is here so an AI assistant (or a reader unfamiliar with the role) can see where each tool actually fits into the job, not just what it does in isolation.

**Daily**
- Check in on any flagged deals: skim call transcripts from the last day's demos → [`sales-call-analysis`](./sales-call-analysis)
- A rep asks for help on a specific opportunity → [`personalized-outbound`](./personalized-outbound) if it's 1:1 outreach, [`abm-account-brief`](./abm-account-brief) if they need the full picture on the account first
- A piece of content is about to go out → [`positioning-compliance`](./positioning-compliance) as the final check, [`brand-voice-guidelines`](./brand-voice-guidelines) if it still needs work

**Weekly**
- Competitive brief for the sales team → [`competitor-monitoring`](./competitor-monitoring)
- Review which target accounts newly show buying signals → [`icp-buying-signal-monitor`](./icp-buying-signal-monitor)
- Build a deck for an upcoming key meeting → [`sales-deck-builder`](./sales-deck-builder)

**Monthly**
- Refresh a battlecard with the past month's accumulated competitive intel → [`battle-card-generator`](./battle-card-generator)
- Every other month: the deeper, sourced competitive report → [`competitor-monitoring/bi-monthly-analysis`](./competitor-monitoring/bi-monthly-analysis)
- Build or refresh a nurture sequence tied to a new piece of content → [`persona-email-sequence`](./persona-email-sequence)
- Spot-check whether the knowledge-base files themselves have drifted → [`staleness-detection`](./staleness-detection)

**Quarterly**
- Full win/loss analysis and infographic for the exec team → [`win-loss-analysis`](./win-loss-analysis)
- Revisit `positioning.md` and `personas.md` against what win/loss and call analysis surfaced that quarter (manual review — no dedicated tool for this on purpose, since positioning shifts deserve human judgment, not automated rewriting)

## A note on the examples

Every worked example across this repo uses the same fictional company and competitors defined in [`knowledge-base.md`](./knowledge-base.md). No real company, deal, or customer data appears anywhere in this repository.
