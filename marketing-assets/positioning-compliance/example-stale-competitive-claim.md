# Sample output — a claim that was true when written, false now

Demonstrates the check category [`skill.md`](./skill.md) added against [`competitive-landscape.md`](../../knowledge-base/competitive-landscape.md): a named-competitor claim that isn't unverifiable or badly worded — it's just factually out of date, because the competitor shipped something after the claim was written. This is the same underlying drift [`staleness-detection`](../../knowledge-base/staleness-detection) exists to catch in the knowledge base itself; this example shows it surfacing in an actual piece of outbound content before publish, not months later in a sweep.

---

## Input

> Sundial is the only valuation platform on the market with a real, working audit trail — every other AI-powered vendor gives you a confidence score and nothing else.

## Output

```
## Compliance Check — Ad copy draft, "only audit trail" claim

**Result:** FAIL

### Hard fails (block publish)
- "Sundial is the only valuation platform on the market with a real, working audit trail" — violates: competitive-landscape.md's current ValuAI section. ValuAI shipped a GA audit trail feature in July 2026 (see competitive-landscape.md's Capability Comparison table and battlecard/valuai.html). This claim was accurate before that date and is factually false now — not unverifiable, wrong. A "we're the only one" claim naming a competitive space has to be re-checked against competitive-landscape.md's current state every time it's reused, not carried forward from whenever it was first approved.
- "every other AI-powered vendor gives you a confidence score and nothing else" — violates: same section, and additionally overbroad — competitive-landscape.md tracks four named competitors specifically (Bricklane Data, Estemate, ValuAI, PropIQ), not "every" vendor in the category; a claim this absolute isn't supportable even before the ValuAI correction.

### Soft flags (reviewer's call)
- None found.
```

## Why this matters as its own category, not just another positioning overclaim

An unverifiable claim (like "industry-leading accuracy" in [`example.md`](./example.md)) is a problem because no evidence was ever offered for it. This is a different failure mode: real evidence existed for this claim once, and it stopped being true on a specific date (ValuAI's July 2026 GA) that the writer wasn't tracking. The fix isn't "don't make unsupported claims" — it's "re-verify a competitive claim against the current source doc every time it's reused," since the doc, not the writer's memory of it, is what changes. See [`compliance-rules-reference.md`](./compliance-rules-reference.md)'s category 4, and [`compliance-trends-analysis.html`](./compliance-trends-analysis.html) for how often this exact failure mode showed up in the month after ValuAI's launch, before competitive-landscape.md itself was refreshed.
