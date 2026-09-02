# Sample output

Fictional raw notes, run as an **update** to the existing ValuAI section of [`competitive-landscape.md`](../../competitive-landscape.md) — demonstrating the "output only what changed" instruction rather than a full regeneration.

---

## Input (raw notes)

> - Lost deal note (Feb 2026): prospect said ValuAI's "regulatory audit trail" feature, mentioned in their sales demo, turned out to be "still in beta with no committed GA date" when the prospect asked procurement to confirm in writing.
> - Another lost deal note (Jan 2026), different prospect, same pattern: audit trail feature demoed but not contractually available at time of signing.
> - A sales call transcript: prospect asked us directly "does your audit trail actually ship today, not 'in beta'?" — implies this is becoming a known concern in the market, not just two isolated incidents.

## Output

```
## Update to: ValuAI battlecard

Changed sections: Weaknesses, Objection handling, Trigger signals
Reason: Two independent lost-deal notes plus a live sales call reference now corroborate a pattern (previously the battlecard flagged this as a single unconfirmed release-note mention).

### Weaknesses (updated)
- Explainability claims reportedly don't hold up under technical follow-up (per call transcript reference — unchanged from prior version)
- NEW, per 2 lost-deal notes (Jan/Feb 2026): their "regulatory audit trail" feature is demoed in sales cycles but was not contractually available (GA) at the point prospects tried to confirm it — this is now a corroborated pattern, not a single data point, and upgrades from "needs confirmation" to "confirmed, source: 2 lost-deal notes."

### Objection handling (updated)
- "ValuAI showed us an audit trail feature too" → Ask directly whether it's committed in their contract/SLA today, not demoed as in-progress. Two recent deals independently hit this same gap between demo and GA availability — this is a fair, specific question for a prospect to ask any vendor, not an attack on ValuAI.

### Trigger signals (updated)
- NEW: prospect mentions being shown an audit-trail or explainability feature in a ValuAI demo without being told whether it's GA — increasingly common enough (2 of 2 recent competitive losses) to treat as a live pattern, not a one-off.
```
