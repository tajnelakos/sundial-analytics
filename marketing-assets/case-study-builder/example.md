# Sample output

Nordkredit — the same account [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor/example.md) flagged, [`abm-account-brief`](../../sales-tools/abm-account-brief/example.md) briefed, and [`personalized-outbound`](../personalized-outbound/example.md) reached out to. This case study is that thread's actual ending: [`sales-call-analysis/call-01-nordkredit.md`](../../knowledge-base/sales-call-analysis/call-01-nordkredit.md) is the resulting discovery call, and the deal closed won per [`win-loss-analysis/win-loss-crm-export.csv`](../../knowledge-base/win-loss-analysis/win-loss-crm-export.csv) (OPP-1001).

---

## Input

> Account: Nordkredit. Source: `win-loss-crm-export.csv` row OPP-1001 (Won, closed 2026-09-08, 65-day cycle, €56,924 ACV, competitor Estemate quoted €57,313, decision driver "Explainability / audit trail", product feedback "Standout: comparable-level audit trail") + `sales-call-analysis/call-01-nordkredit.md` (discovery call with Lena Virtanen, Head of Credit Risk).

## Output

```
## Case Study — Nordkredit

**Status:** Draft — pending Nordkredit's explicit sign-off before publishing named or quoting Lena Virtanen publicly

**Title:** Nordkredit replaces a "confidence score only" valuation tool ahead of a board audit
**Snapshot:** Bank/Lender · Tier 1 · Nordics · ~€600M annual origination · Displaced: Estemate (incumbent) · Deal size: €56,924 ACV · Sales cycle: 65 days

### Challenge
Nordkredit's newly hired Head of Credit Risk inherited an internal audit finding on her first day: the bank's existing valuation tool produced a confidence score and a generic methodology document, not the specific comparables used for an individual property. When an examiner or internal risk committee asked "why this number," the only honest answer was "the model said so" — not something the team wanted to repeat at an upcoming board audit.

### Solution
Rather than a prepared demo, Sundial ran a live audit trail on one of Nordkredit's own past valuations, at the prospect's request — showing the actual comparables used and their weighting for that specific property, not a templated walkthrough. Nordkredit had already used this same standard (push past the first demo, ask for a real breakdown) to evaluate and rule out another vendor earlier in its process.

### Results
- Closed in 65 days — inside Nordkredit's own Tier 1 typical sales-cycle range (per `icp.md`: 2-4 months)
- Logged decision driver: "Explainability / audit trail" (win-loss-crm-export.csv, OPP-1001)
- Logged product feedback: "Standout: comparable-level audit trail" (same record)
- Won at effective price parity, not on discount — Sundial's ACV (€56,924) closely tracked the competitor's own quoted price (€57,313) for the same deal

### Quote
No public-use quote available yet. Lena Virtanen's discovery-call comments about the "the model said so" problem are exactly the kind of language a real testimonial should use — but they were said on a sales call, not given as a public statement, so using them here requires her explicit sign-off first, not just because they exist in our call notes.

---
Positioning tie-in: "Explainable by design" (positioning.md's message house) — the specific proof point this account decided on (named comparables and weighting, not a confidence score) is exactly this pillar, not a generic accuracy claim.
Sourced from: win-loss-crm-export.csv (OPP-1001) · sales-call-analysis/call-01-nordkredit.md
What's not confirmed: whether Nordkredit's implementation was completed before their stated board-audit date (tentatively the second week of September, per the call transcript) — the CRM close date (2026-09-08) falls right around that window, but "deal closed" isn't the same claim as "audit passed," and the source material doesn't confirm the latter. This case study should not assert it did.
```

Note what this example deliberately does *not* do: it doesn't smooth over the audit-timing question just because it would make a cleaner ending — the "what's not confirmed" line exists specifically so a genuinely unverified detail doesn't get published as fact.
