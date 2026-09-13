# Sample output

The rendered one-pager: [`one-pager-head-of-credit-risk.html`](./one-pager-head-of-credit-risk.html) ([view live ↗](https://tajnelakos.github.io/sundial-analytics/marketing-assets/one-pager-builder/one-pager-head-of-credit-risk.html)).

---

## Input

> Build a one-pager for the Head of Credit Risk persona, Tier 1 bank/lender segment.

## Output

```
## One-Pager — Head of Credit Risk, Tier 1 Bank/Lender

**Positioning angle used:** "A valuation you can defend, not just receive" — positioning.md's primary message, not the Mortgage Ops or Brokerage segment rows.
**Format:** designed single-page HTML — see one-pager-head-of-credit-risk.html

**Headline:** A valuation you can defend, not just receive.
**Subhead:** Most valuation tools give you a number and a confidence score. If an examiner asks how that number was reached, "the model said so" isn't an answer — and increasingly, regulators are asking.
**Proof points:**
1. Per-valuation audit trail — every output includes the specific comparables used and their weighting, inspectable, not just a confidence score.
2. Disclosed accuracy methodology — benchmarking approach documented and available for technical evaluators to scrutinize.
3. Built for regulated lending from inception — audit-log format and integration points designed around lending compliance from the start.
4. A recent deal proof point (anonymized, pending sign-off) — a Nordics regional bank displaced its incumbent specifically over this gap.
**CTA:** See a live audit trail on one of your own past valuations — real data, no prepared demo, about 15 minutes.

---
Sourced from: positioning.md (headline, subhead, proof points 1-3, exact wording) · win-loss-analysis/win-loss-crm-export.csv OPP-1001 + case-study-builder/example.md (proof point 4, anonymized until customer sign-off)
```

## Why this is a one-pager and not a mini pitch deck

- **One angle, not three.** This targets Head of Credit Risk specifically — it doesn't also try to land the Mortgage Ops cycle-time pitch or the Brokerage adoption pitch on the same page. A VP of Mortgage Lending version would need its own one-pager with a different headline and different proof points, not this one with a different logo.
- **Every proof point is checkable.** None of the four claims is an adjective — each traces to `positioning.md`'s differentiators table or a real, sourced deal, per this persona's own stated distrust of unsourced case studies (`personas.md`).
- **The CTA matches this persona's specific trust trigger** — "a vendor who volunteers a live demo on the buyer's own real data, unprompted" (`personas.md`) — not a generic "book a demo" button.
- **The customer-proof-point strip is honest about consent status**, same discipline as [`case-study-builder`](../case-study-builder) — anonymized, with the real named version flagged as pending sign-off rather than presented as already available.
