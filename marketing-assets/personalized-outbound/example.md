# Sample output

Outreach closing the loop from [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor) → [`abm-account-brief`](../../sales-tools/abm-account-brief) → this.

**Account:** Nordkredit (fictional) · **Persona:** Head of Credit Risk · **Signal strength:** Strong (two corroborating signals)

This is one cell of a three-example grid — see [`README.md`](./README.md#the-account--persona-grid). [`example-nordkredit-vp-mortgage-lending.md`](./example-nordkredit-vp-mortgage-lending.md) holds the account fixed and changes the persona; [`example-court-street-lending-head-of-credit-risk.md`](./example-court-street-lending-head-of-credit-risk.md) holds the persona fixed and changes the account (and the signal strength).

---

## Input

The [Nordkredit account brief](../../sales-tools/abm-account-brief/example.md), pasted in full.

## Output

```
## Outbound Draft — Nordkredit — Email

Subject: Explainability for the new valuation tooling

Hi [Name],

Congratulations on the new role — and on the timing, since I saw your team is actively migrating valuation workflows off your current tooling.

That's usually the exact point where explainability becomes a real requirement rather than a nice-to-have, especially with a new risk mandate in place. Most valuation tools we come across can tell you a number; fewer can show a comparable-level audit trail an examiner would actually accept.

Worth a 15-minute conversation about how you're thinking about that requirement for the new setup? Happy to just listen if it's early days.

[Rep name]

---
Personalization used: the new Head of Credit Risk hire and the concurrent tooling-migration job postings — both from the account's specific trigger signal, not a generic opener.
```

Note what's absent: no product name in the subject line, no feature list, no demo ask — the brief indicated this account is early and unaware, so the ask stays small.
