# Ideal Customer Profile — Sundial Analytics (fictional)

Reference context for [Sundial Analytics](./knowledge-base.md). Used by prompts/skills that need to reason about fit or in-market signals rather than have it re-explained inline every time.

## Tiered customer profiles

| | Tier 1 (best fit) | Tier 2 | Tier 3 (opportunistic) |
|---|---|---|---|
| **Segment** | Regional banks & mortgage lenders | National/multi-region lenders | Real estate brokerages |
| **Loan volume** | €200M–€2B annual origination | €2B+ (longer sales cycle, more procurement layers) | N/A — seat-based, not volume-based |
| **Geography** | DACH, Benelux | Nordics, wider EU | DACH, Benelux |
| **Core banking / LOS** | Mid-market systems with open APIs (e.g. modern LOS platforms) | Legacy core banking, heavier integration lift | Any CRM (Sundial's brokerage product is standalone) |
| **Regulatory posture** | Subject to periodic valuation audits, actively modernizing | Subject to audits, slower to change vendors | Not regulator-facing |
| **Sales cycle** | 2–4 months | 6–12 months | 3–6 weeks |

Tier 1 is the focus for outbound and content strategy — best combination of pain intensity (explainability is a real audit problem) and reachable buying committee size.

## Buying committee (Tier 1, bank/lender deals)

| Role | Typical title | Stake |
|---|---|---|
| Economic buyer | Chief Risk Officer / Head of Credit Risk | Owns budget, cares about audit defensibility and vendor risk |
| Technical evaluator | Credit Risk Analyst / Data lead | Validates model accuracy and integration feasibility |
| End user | Underwriter / Loan officer | Uses the tool daily, cares about speed and workflow fit |
| Procurement / blocker | Vendor risk / Compliance | Gates the deal on data handling, SLAs, certifications — usually enters late |

A deal without early technical evaluator buy-in tends to stall at the procurement gate later, even if the economic buyer is enthusiastic — worth surfacing this in deck/outline prompts (see [`sales-deck-builder`](./sales-deck-builder)).

## External signals that indicate a company is in-market

- New Head of Credit Risk or Chief Risk Officer hire within the last 2 quarters (frequently a mandate-holder for modernization)
- Public statements about an upcoming regulatory audit cycle or a recent adverse audit finding
- Job postings for "credit risk analyst" or "valuation" roles mentioning a specific legacy tool by name (signals dissatisfaction or planned migration)
- LOS (loan origination system) migration announced or underway — valuation tooling often gets revisited alongside it
- Executive turnover at a competitor's existing customer (new leadership frequently re-evaluates inherited vendor choices)

These signals feed the [`competitor-monitoring`](./competitor-monitoring) brief and outbound targeting — not a hard qualification checklist, but a prioritization signal.
