# Sample output

Checking [`competitive-landscape.md`](../competitive-landscape.md) against a fictional newer signal — continuing the ValuAI thread from [`battle-card-generator`](../battle-card-generator/example.md).

---

## Input

> Newer signal (April 2026, hypothetical): ValuAI's release notes now state their "regulatory audit trail" feature is Generally Available as of this month, with a named enterprise customer reference.
>
> Document to check: competitive-landscape.md, ValuAI section.

## Output

```
## Staleness Check — competitive-landscape.md (ValuAI section) — against April 2026 ValuAI release notes

### Hard flags (contradicted by newer evidence)
- Claim: "explainability claims reportedly don't hold up under technical follow-up" / battlecard's objection-handling line assuming the audit trail feature is not GA — Contradicted by: April 2026 ValuAI release notes stating the feature is now GA with a named customer reference. Recommended action: route to `battle-card-generator` to refresh the ValuAI Weaknesses and Objection Handling sections — the "ask if it's GA" talk track no longer works as-is if it now is. Note: this doesn't necessarily mean the feature is good, only that the "still beta" framing is now outdated — the refreshed card should investigate the GA feature directly rather than just removing the old claim.

### Soft flags (unverified, no contradicting evidence, worth a recheck)
- Claim: "PropIQ... not a primary battlecard priority outside the brokerage segment" — Last supporting evidence: original battlecard assumption, no recent signal has confirmed or contradicted this either way — worth a periodic recheck rather than treating it as settled, since competitive landscape assumptions like this tend to go stale silently.
```

Note the recommended action routes to the correction skill rather than attempting the fix here — staleness detection's job stops at flagging.
