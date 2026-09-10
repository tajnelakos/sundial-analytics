# Battlecard

## The problem

[`competitive-landscape.md`](../../knowledge-base/competitive-landscape.md) is the deep, analyst-maintained reference — the right format for someone building or auditing the competitive picture. It's the wrong format for a rep about to get on a call, who needs something they can skim in under a minute, not read as a document. Someone has to translate the reference doc into a field-ready card, and that translation is real work: deciding which 3-5 differentiators actually matter, phrasing objection handlers the way a person would say them out loud, being explicit about what not to claim.

This is distinct from [`competitor-monitoring`](../competitor-monitoring), which tracks what *changed this week*, and from `competitive-landscape.md` itself, which is the deep reference. This folder is the rep-facing output built from that reference.

## The approach

A skill that takes the data already in `competitive-landscape.md` (plus any new raw research) and produces two things: a full rep-facing HTML battlecard per competitor, and, when new research warrants it, a targeted update to `competitive-landscape.md`'s own entry. Every battlecard follows the same structure so a rep who's used one can navigate any of them cold:

Header info → company overview & strategy → positioning framework ("they say → reality → we win because") → value pillars with proof points → discovery/landmine questions → objection handlers → do-not-say list → an optional feature matrix, only where a real gap justifies one.

Card depth matches actual threat level — the High-threat Bricklane Data card is not the same length as the Low-threat PropIQ card, on purpose.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`example.md`](./example.md) — the targeted-update mode: a battlecard section updated from new raw notes, output as a diff against the existing entry rather than a full regeneration
- [`bricklane-data.html`](./bricklane-data.html) — 🔴 High threat ([view live ↗](https://tajnelakos.github.io/sundial-analytics/sales-tools/battlecard/bricklane-data.html))
- [`estemate.html`](./estemate.html) — 🟡 Medium threat ([view live ↗](https://tajnelakos.github.io/sundial-analytics/sales-tools/battlecard/estemate.html))
- [`valuai.html`](./valuai.html) — 🟠 Medium-high threat ([view live ↗](https://tajnelakos.github.io/sundial-analytics/sales-tools/battlecard/valuai.html)) — refreshed this cycle to reflect ValuAI's July 2026 audit-trail GA launch (see [`competitor-monitoring/bi-monthly-report-2026-07-08.md`](../competitor-monitoring/bi-monthly-report-2026-07-08.md))
- [`propiq.html`](./propiq.html) — ⚪ Low threat ([view live ↗](https://tajnelakos.github.io/sundial-analytics/sales-tools/battlecard/propiq.html)) — deliberately short

## Current limitations

Right now this runs as a manual pass per competitor. Automatically cross-referencing new input against the existing card and flagging contradictions (e.g. new win/loss data suggesting a differentiator no longer holds) is next — see [`staleness-detection`](../../knowledge-base/staleness-detection), which already flags exactly this kind of drift in `competitive-landscape.md`.
