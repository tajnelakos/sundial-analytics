# Sample output

Sequence for the Head of Credit Risk persona ([`personas.md`](../../knowledge-base/personas.md)).

---

## Input

> Persona: Head of Credit Risk. Trigger: downloaded our "Explainability in Automated Valuation" whitepaper from the site.

## Output

```
## Email Sequence — Head of Credit Risk — Trigger: whitepaper download

### Email 1 — "The part most 'explainable AI' claims skip" — Day 0
You downloaded our piece on explainability in automated valuation, so you're probably already skeptical of the term — most vendors use it to mean "we show a confidence score," not "we can show our work."
The difference matters most in an audit, not a demo. If you want to see what a comparable-level audit trail actually looks like on a real valuation (not a curated example), it takes about 15 minutes.
Decision criterion this advances: auditability / explainability of individual decisions (top-ranked criterion) — moves from the whitepaper's general argument to a concrete, inspectable example.

### Email 2 — "How we validate accuracy (and how to check our work)" — Day 4
Following up on explainability — the other question worth asking any vendor is how they validate accuracy, and whether that methodology is something you can actually scrutinize or just a headline number.
Our benchmarking approach is documented, not just claimed. Worth a look if you're building a shortlist criteria doc for this evaluation.
Decision criterion this advances: model accuracy validated against a disclosed methodology (2nd-ranked criterion) — distinct from email 1's audit-trail focus.

### Email 3 — "What changes (and what doesn't) if you switch" — Day 9
Last thing worth covering before I stop filling your inbox: what actually changes operationally if you moved off your current tooling, and what stays the same.
Integration effort is real but usually smaller than teams expect going in — happy to walk through what that'd look like for your setup specifically, no pressure if the timing isn't right.
Decision criterion this advances: vendor stability / integration effort (3rd/4th-ranked criteria) — closes the loop on the remaining lower-ranked concerns without urgency tactics.
```

Note: no 4th email pushing "last chance" urgency — this persona is described in `personas.md` as more skeptical, not less, of pressure tactics, so the sequence ends on a low-pressure, real-effort answer instead.
