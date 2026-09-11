# Sample output — same account, different persona

**Account:** Nordkredit (fictional) · **Persona:** VP of Mortgage Lending · **Signal strength:** Strong (same signal as [`example.md`](./example.md))

Holds the account and trigger fixed from [`example.md`](./example.md) and changes only the persona, to isolate what a persona swap alone changes. This is a real, common rep move — multi-threading an account by writing to a second stakeholder using the same known signal, read through that stakeholder's own priorities rather than restating the first email with a new name at the top.

---

## Input

> Same underlying signal as the [Nordkredit account brief](../../sales-tools/abm-account-brief/example.md): new Head of Credit Risk hired ~3 weeks ago; engineering job postings this month reference migrating valuation workflows off legacy tooling.
>
> This message is not to that new Head of Credit Risk hire — it's a parallel outreach to Nordkredit's VP of Mortgage Lending, multi-threading the account. No new facts beyond what the original brief established; the persona reading it changes, not the underlying trigger.
>
> **Lead persona for this message:** VP of Mortgage Lending — per `personas.md`, this persona owns cycle time and workflow, will defer to Credit Risk on explainability, and won't advocate internally for the risk side of a purchase.
> **Positioning angle:** "Minutes, not days, without giving up defensibility" (the Mortgage Ops row in `positioning.md`'s segment table) — distinct from the Head of Credit Risk email's defensibility-first framing.

## Output

```
## Outbound Draft — Nordkredit — Email

Subject: What the tooling migration means for cycle time

Hi [Name],

I saw your team's already in motion on migrating valuation tooling off your current vendor — usually a risk-driven decision, but the workflow impact lands on lending ops either way.

A change like this tends to go one of two ways for a quarter or two: cycle time quietly improves, or it quietly gets worse while everyone adjusts to a new step. Worth 15 minutes on what the transition actually looks like week-to-week for your loan officers — separate from whatever your risk team is evaluating on the explainability side?

[Rep name]

---
Personalization used: the same tooling-migration signal used in the Head of Credit Risk outreach to this account, re-read through the Lending Ops lens instead — no new fact, a different persona's angle on it.
```

## Why this email is different from the Head of Credit Risk version, not just re-addressed

- **Opens on workflow disruption risk, not audit trail** — this persona's top decision criterion (`personas.md`) is cycle-time/throughput, not explainability.
- **The ask is about the transition itself**, not a conversation about methodology — matches what this persona actually owns.
- **Explicitly stays out of the risk/compliance conversation** ("separate from whatever your risk team is evaluating") — this persona's profile states plainly that being asked to carry the internal risk case is a trust breaker, so the email doesn't lean on them for that even implicitly.
- **No mention of audit trails, examiners, or defensibility** — those words would be exactly right in the Head of Credit Risk email and exactly the wrong opener here; a persona-blind template would have included them by default.
