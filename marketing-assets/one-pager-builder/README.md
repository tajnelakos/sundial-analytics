# One-Pager Builder

## The problem

Most one-pagers try to be a mini pitch deck instead of a one-pager — every stakeholder's angle crammed onto one page in increasingly small type, so it ends up saying nothing clearly to anyone. A real one-pager requires picking exactly one audience and one angle and being willing to leave the rest out.

## The approach

A skill that builds a single-page, persona-specific piece of sales collateral — one positioning angle from [`positioning.md`](../../knowledge-base/positioning.md), 3-4 sourced proof points, one CTA matched to that persona's actual trust trigger from [`personas.md`](../../knowledge-base/personas.md). Unlike this repo's text-only skills, the output is an actual designed HTML page using [`branding-guideline`](../../knowledge-base/branding-guideline)'s real color palette and typography, not just copy in a markdown block — a one-pager is a visual artifact, and it's checked as one.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`one-pager-head-of-credit-risk.html`](./one-pager-head-of-credit-risk.html) — the rendered one-pager ([view live ↗](https://tajnelakos.github.io/sundial-analytics/marketing-assets/one-pager-builder/one-pager-head-of-credit-risk.html))
- [`example.md`](./example.md) — the input/output behind it

## Current limitations

Only one persona/segment combination is built out (Head of Credit Risk, Tier 1 Bank/Lender). A VP of Mortgage Lending or Brokerage version needs its own pass with a different angle and proof set, not a find-and-replace on this one — see `skill.md`'s explicit rule against fitting two personas on one page.
