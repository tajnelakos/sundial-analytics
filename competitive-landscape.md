# Competitive Landscape — Sundial Analytics

Full battlecard reference. The summary table in [`knowledge-base.md`](./knowledge-base.md) is the quick version; this is what [`competitor-monitoring`](./competitor-monitoring) and [`win-loss-analysis`](./win-loss-analysis) draw on for deeper context.

## Market map

|  | Bank/lender segment | Brokerage segment |
|---|---|---|
| **Compete directly** | Bricklane Data, Estemate, ValuAI | PropIQ |
| **Compete indirectly / rarely** | PropIQ (occasionally shows up in brokerage-adjacent bank deals) | Bricklane Data, Estemate (not brokerage-focused) |

---

## Bricklane Data

**Positioning:** Speed and price. Their pitch is "valuations in seconds, at the lowest per-call cost in the market."

**Strengths:** Genuinely fast, aggressive pricing, easy self-serve API onboarding — appeals to buyers who haven't yet hit an audit-defensibility problem.

**Weaknesses:** Explainability is thin — confidence score with no comparable-level breakdown. No dedicated compliance/audit-log feature.

**How we win:** Reframe the conversation from price-per-call to cost-of-an-indefensible-decision. Works best once the Head of Credit Risk (not just procurement) is in the room — see [`personas.md`](./personas.md).

**How we lose:** Deals that stay procurement-led and never reach a real risk conversation; deals where price sensitivity dominates because the institution hasn't yet had an audit incident.

**Objection handling:** "Bricklane is 15% cheaper" → don't price-match; quantify the audit/rework cost of an unexplainable valuation instead, and offer a side-by-side audit trail comparison.

**Trigger signals it's in the deal:** Prospect asks about per-call pricing early, before asking about methodology.

---

## Estemate

**Positioning:** Legacy incumbent, especially entrenched in France/Benelux. Sells on relationship tenure and breadth of historical data.

**Strengths:** Long-standing customer relationships, large historical dataset, strong brand recognition in Benelux specifically.

**Weaknesses:** Dated UI, slow release cadence, publicly documented support responsiveness issues (see [`competitor-monitoring/example`](./competitor-monitoring/example/sample-output.md)).

**How we win:** Modern integration experience and faster implementation timeline; strongest against Estemate when the buying committee includes someone frustrated with the current tool's UX or support.

**How we lose:** Deeply entrenched relationships where switching cost (real or perceived) outweighs product gaps; risk-averse buyers who default to "nobody gets fired for choosing the incumbent."

**Objection handling:** "We've used Estemate for 10 years" → don't attack the relationship; focus on a specific, current pain point (support responsiveness, release velocity) rather than a general pitch to switch.

**Trigger signals it's in the deal:** Prospect is Benelux-based; prospect mentions a slow support ticket or a feature request that's been open a long time.

---

## ValuAI

**Positioning:** "AI-native" challenger, well-funded, leads with technology-forward messaging.

**Strengths:** Strong initial sales narrative, modern-feeling product demo, aggressive marketing presence.

**Weaknesses:** Explainability claims reportedly don't hold up under technical follow-up (see the [sales call example](./sales-call-analysis/example/sample-output.md)); thin on regulatory-specific features.

**How we win:** This is our clearest differentiation lane — let the buyer's own follow-up questions expose the gap rather than attacking ValuAI directly; offer to show our audit trail live on their own data as the resolution.

**How we lose:** Early-stage deals where the buyer hasn't yet pressure-tested ValuAI's claims and is still impressed by the demo.

**Objection handling:** "ValuAI says they're explainable too" → don't dispute it in the abstract; invite direct comparison ("ask them to show the actual comparable-level audit trail on a real valuation, then ask us the same").

**Trigger signals it's in the deal:** Buyer uses the word "AI-native" or references a recent, polished ValuAI demo.

---

## PropIQ

**Positioning:** Brokerage-focused, doesn't meaningfully compete in the bank/lender segment.

**Relevance:** Comes up mainly in brokerage deals or occasionally when a bank buyer also has a brokerage arm evaluating tools separately. Not a primary battlecard priority outside the brokerage segment.

---

## Positioning gaps to exploit

1. **No competitor has a credible, specific answer to "show me the audit trail on a real valuation, not a demo one"** — this is the single highest-leverage moment in a competitive deal (see [`positioning.md`](./positioning.md)).
2. **Support responsiveness is a live, public weakness for Estemate** — usable in Benelux-specific battlecards without needing to fabricate anything, since it's evidenced in public reviews.
3. **Bricklane's price-led positioning has no answer to a risk-framed objection** — reframing the conversation away from price is more effective than matching it.
