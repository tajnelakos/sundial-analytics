# Positioning — Sundial Analytics

Used by prompts/skills that generate customer-facing content — see [`sales-deck-builder`](../sales-tools/sales-deck-builder), [`branding-guideline`](./branding-guideline), and [`abm-account-brief`](../sales-tools/abm-account-brief) (which picks the specific angle below that fits a named account, rather than the general pitch).

## Market category

Sundial doesn't try to create a new category — "automated valuation model" is an established, understood term, and fighting that understanding would cost more than it earns. The positioning instead claims a **sub-category within it**: not "the AVM," but "the AVM built to be defended," treating explainability as core infrastructure rather than a bolt-on feature. This is a deliberate choice — category creation is expensive and slow, and the market is already primed to ask the right question (see [`competitive-landscape.md`](./competitive-landscape.md)'s Market Patterns, where two competitors independently started reaching for the same "audit-ready" language this period — the sub-category is becoming contested, not proprietary).

## Competitive alternatives

What a prospect does instead of buying Sundial, in rough order of how often it's the actual alternative:

1. **An existing AVM vendor** (Bricklane Data, Estemate, ValuAI, or occasionally PropIQ in brokerage-adjacent deals) — the most common alternative, see [`competitive-landscape.md`](./competitive-landscape.md) for the full battlecard set.
2. **Staying with a fully manual valuation process** — more common at smaller Tier 2 accounts or ones without a dedicated risk function (see [`icp.md`](./icp.md)'s Anti-ICP section); the pitch here is about the risk of *no* audit trail, not a better one.
3. **An in-house-built model** — the hardest alternative to displace, since the buyer isn't evaluating a product, they're defending a prior internal decision. Positioning here has to avoid sounding like an attack on the team that built it — see [`icp.md`](./icp.md)'s note on this as a near-Anti-ICP case.
4. **Doing nothing / deferring the decision** — the real competitor in a large share of stalled deals (see the Delta Mortgage Partners pattern in [`sales-call-analysis`](./sales-call-analysis/call-07-delta-mortgage-partners.md)), where the honest positioning response is patience, not more pressure.

## Strategic narrative

The valuation industry solved for *speed* over the last decade — automated valuation models got fast and cheap. It did not solve for *defensibility*. Regulators and internal risk teams are asking harder questions about how automated decisions are made, and most "AI-powered" valuation tools cannot answer them beyond "the model said so." The institutions that will hold up under scrutiny are the ones that treated explainability as core infrastructure from the start, not a feature bolted on after a compliance complaint.

Sundial's narrative is not "we're more accurate" (most credible vendors in this space are within a defensible accuracy range of each other) — it's **"we're the one you can actually defend."**

## Message house

One primary message, three pillars that support it, each with its own proof point — the structure every other positioning artifact in this repo should trace back to.

**Primary message:** *A valuation you can defend, not just receive.*

| Pillar | Claim | Proof point |
|---|---|---|
| Explainable by design | Every valuation includes the specific comparables used and their weighting | Inspectable output, not a confidence score — see [`competitive-landscape.md`](./competitive-landscape.md)'s capability comparison |
| Accuracy you can scrutinize | Benchmarking methodology is disclosed, not asserted | Available to technical evaluators on request — see the [Credit Risk Analyst / Data Lead persona](./personas.md#credit-risk-analyst--data-lead-technical-evaluator) |
| Built for regulated lending, not retrofitted | Audit-log format and integration points were designed around lending compliance from inception | Distinct from a general AI product with a compliance feature added later |

## Points of view that ladder to this

1. **"Fast and unexplainable is a liability, not a feature."** Speed only has value if the decision survives scrutiny later. A valuation that's 2 seconds faster but can't be explained to an auditor creates risk it doesn't remove.
2. **"AI-powered" is not a differentiator anymore — everyone claims it.** The differentiator is what happens when a buyer or regulator asks *how*, specifically, a number was reached. Most vendors' answer degrades under that question; this is where the real gap is.
3. **"Explainability" needs a definition or it's marketing, not a capability.** Sundial defines it concretely: named comparables, weighting logic, and a reproducible audit trail per valuation — not a general claim.

## Differentiators, with proof points

| Differentiator | Proof point (fictional, for illustration) |
|---|---|
| Per-valuation audit trail | Every output includes the specific comparables used and their weighting — inspectable, not just a confidence score |
| Accuracy validated against a disclosed methodology | Benchmarking approach is documented and available for technical evaluators to scrutinize, not just a headline accuracy percentage |
| Built for the regulated-lending workflow, not adapted from a consumer product | Integration points and audit-log format were designed around lending compliance requirements from the start |

## Positioning by segment and tier

Value proposition changes by who's buying; tier (see [`icp.md`](./icp.md)) changes how much proof the pitch needs to carry before it lands.

| Segment | Pain | Value proposition | Tier-specific note |
|---|---|---|---|
| Credit Risk (bank/lender) | Can't defend automated decisions to an auditor | A valuation you can explain, not just deliver | Tier 1: the pain is often anticipatory (a coming audit). Tier 2: frequently a *lived* pain — a specific past finding, which makes the pitch easier to land but the sales cycle longer regardless (more procurement layers) |
| Mortgage Ops (bank/lender) | Manual review slows down loan cycle time | Minutes, not days, without giving up defensibility | Matters most at Tier 1, where lending-ops and risk are both active, present stakeholders — see the [persona interaction map](./personas.md#persona-interaction-map) |
| Brokerage | Agent tools go unused after initial rollout | Valuation insight that helps agents win the listing conversation, not another dashboard | This is Tier 3's entire positioning — defensibility and audit trails are largely irrelevant here; adoption and listing-conversation value are the whole pitch |

## Positioning against specific competitors — strategic framing

This is the strategic posture behind each competitor's tactical talk track in [`competitive-landscape.md`](./competitive-landscape.md) and its [battlecards](../sales-tools/battlecard) — the "why we lead with this" behind the "what to say."

- **Against Bricklane Data:** Don't compete on their terms (price, speed). Reframe the axis of comparison entirely, to cost-of-an-indefensible-decision — competing on their chosen metric is a losing position even when the product argument is sound.
- **Against Estemate:** Don't position as "the disruptor" — this reads as a risk to a buyer who's already risk-averse by function. Position as "the modernization that doesn't require you to bet on an unproven vendor," which lets a switching decision feel safe rather than bold.
- **Against ValuAI:** The strategic ground has shifted, not disappeared. Before their July 2026 GA launch, the position was "they don't have this." Now it has to be "having it and proving it at scale are different claims" — see [`battlecard/valuai.html`](../sales-tools/battlecard/valuai.html) for how the tactical talk track already reflects this shift.
- **Against PropIQ:** Don't compete directly — different buying committee, different job to be done. The only strategic posture needed is "one platform covers both your lending and brokerage needs," and only when both actually exist inside one prospective account.

## Elevator pitches

- **One sentence:** "Sundial gives lenders a property valuation they can actually defend to a regulator, not just a number."
- **One paragraph (customer-facing):** "Most valuation tools give you a number and a confidence score. If an examiner asks how that number was reached, 'the model said so' isn't an answer — and increasingly, regulators are asking. Sundial's audit trail shows the specific comparables used and how they were weighted, for every valuation, so your team can explain a decision as confidently as it made it."
- **Internal onboarding version:** "We don't win on being the most accurate AVM — most credible vendors are close enough on raw accuracy that it's not a defensible sole claim. We win by being the one whose decisions survive being questioned, which matters more every year as regulatory scrutiny of automated lending decisions increases."

## Objections to the positioning itself

The positioning has to survive skepticism aimed at the positioning, not just the product:

- **"Every vendor now claims some version of 'explainable.'"** True, and increasingly so (see [`competitive-landscape.md`](./competitive-landscape.md)'s Market Patterns). The response isn't to abandon the claim, it's to make it concrete and provable rather than asserted — see "How this positioning needs to evolve" below.
- **"This sounds like it's just about compliance, not better lending outcomes."** Fair challenge — the value proposition table above exists specifically to connect the same underlying capability to a different, non-compliance pain for the Mortgage Ops persona.
- **"If accuracy is roughly equivalent across vendors, why does this matter at all?"** Because the cost of an unexplainable decision is realized later, not at the moment of the valuation — this is the single hardest part of the pitch to make concrete, and the reason [`sales-deck-builder`](../sales-tools/sales-deck-builder) leads with the buyer's pain before the product.

## How this positioning needs to evolve

This narrative was built on a real, durable gap — but that gap is not static, and the positioning has to be honest about that rather than defend a fixed claim indefinitely. The bi-monthly competitive report ([`competitor-monitoring/bi-monthly-report-2026-07-08.md`](../sales-tools/competitor-monitoring/bi-monthly-report-2026-07-08.md)) flagged this directly: two of four tracked competitors shifted toward "audit-ready" language in the same period, and ValuAI shipped a real (if unproven-at-scale) audit trail feature. The wedge is narrowing faster than expected.

The adaptation already reflected in [`battlecard/valuai.html`](../sales-tools/battlecard/valuai.html) is the right direction for the whole narrative, not just that one battlecard: as competitors close the *capability* gap, the positioning needs to shift its center of gravity from "we have explainability" toward **proof at scale** — named reference customers speaking specifically to the audit trail, a public benchmark, a track record measured in years of production use rather than a launch announcement. Capability claims are becoming table stakes; production-proven trust is not yet.

*(Updated via `staleness-detection` sweep, September 2026 — see [`sweep-2026-09.md`](./staleness-detection/sweep-2026-09.md): the [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html) now gives this argument a concrete number — 0 wins for ValuAI across 8 head-to-head deals since their GA launch — which is the strongest "proof at scale" evidence we currently have for our own side of the claim. Cite it, but don't lean on it as settled: 8 deals is a small, recent sample, and the same sweep also found we're losing nearly three-quarters of deals against Estemate, the least "exciting" competitor in this book — a reminder that this narrative's real test is the boring incumbent as much as the flashy new entrant.)*

## What this is not

Not a claim of superior raw accuracy over every competitor in every scenario — that claim is not reliably defensible and erodes credibility with a technically skeptical buyer (see the [Head of Credit Risk persona](./personas.md#head-of-credit-risk-economic-buyer-banklender-segment)). The narrative wins on defensibility and transparency, not a race to the highest accuracy number.
