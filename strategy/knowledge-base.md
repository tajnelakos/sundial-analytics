# Knowledge Base — Sundial Analytics (fictional)

Master source of truth for every prompt, skill, and example in this repo. Every other file in `strategy/` is a derived, deeper view of one section of this doc — kept separate so a skill can reference just the piece it needs (voice rules, competitor detail, persona psychology) instead of the whole thing.

All examples in this repo are built around one consistent fictional company, so the prompts and outputs read as a coherent body of work rather than disconnected demos. **None of this is real** — no real competitor, customer, or deal data is represented anywhere in this repo.

## Company

**Sundial Analytics** — B2B SaaS. Sells automated valuation models (AVMs) and real estate market intelligence, via API and web app, to banks, mortgage lenders, and real estate brokerages across Europe (core markets: DACH, Benelux, Nordics).

- **ICP**: mid-size regional banks and mortgage lenders who need instant, defensible property valuations for lending decisions; secondary ICP is real estate brokerages wanting market analytics for agents.
- **Pricing**: usage-based API pricing (per valuation call) for banks, seat-based for the brokerage web app.
- **Positioning**: "valuations you can defend to a regulator," i.e. accuracy + explainability, not just speed.

## Fictional competitors

| Competitor | Angle |
|---|---|
| **Bricklane Data** | Cheaper, faster valuations; weaker explainability — sells on speed and price |
| **Estemate** | Legacy incumbent, strong in France/Benelux, dated UI, slow release cycle |
| **ValuAI** | Well-funded new entrant, leads with "AI-native" messaging, thin on regulatory compliance features |
| **PropIQ** | Brokerage-focused, doesn't really compete for the bank/lender segment but comes up in brokerage deals |

Derived: full battlecards, positioning gaps, and objection handling → [`competitive-landscape.md`](./competitive-landscape.md)

## Fictional buyer personas

- **Head of Credit Risk** (bank buyer) — cares about model accuracy, audit trail, regulatory defensibility. Skeptical of "black box AI" claims.
- **VP of Mortgage Lending** — cares about speed-to-decision and integration effort.
- **Broker Team Lead** (brokerage buyer) — cares about agent adoption and how valuations help close listings.

Derived: full buying psychology, objections, content preferences → [`personas.md`](./personas.md)

## Derived reference files

This doc is the quick summary. Everything below expands one section of it into the depth an actual skill needs:

- [`icp.md`](./icp.md) — firmographics, tiering, buying committee, in-market signals
- [`personas.md`](./personas.md) — per-persona psychology, objections, content preferences
- [`positioning.md`](./positioning.md) — narrative, differentiators, value props by segment
- [`voice-guide.md`](./voice-guide.md) — tone, style rules, anti-patterns, prohibited terms
- [`competitive-landscape.md`](./competitive-landscape.md) — full battlecards and positioning gaps

Use this file and the ones above as the reference for names, roles, and competitive angles whenever a prompt or example needs a stand-in for real data.
