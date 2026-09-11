# Sample output — same persona, different account (and a weaker signal)

**Account:** Court Street Lending (fictional) · **Persona:** Head of Credit Risk (same as [`example.md`](./example.md)) · **Signal strength:** Medium (single, uncorroborated signal)

Holds the persona fixed from [`example.md`](./example.md) and changes the account — and, deliberately, the signal strength, since [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor/example.md) scored this account's signal as Medium, not Strong like Nordkredit's. The point of this example isn't just "different company, same pitch" — it's that a thinner signal should produce a more exploratory ask, not a confidently-pitched email dressed up with a weaker hook.

This is the fictional cold outreach that could plausibly have opened the door before the later, second call documented in [`sales-call-analysis/call-03-court-street-lending.md`](../../knowledge-base/sales-call-analysis/call-03-court-street-lending.md) — at this point in the timeline, David Okafor's name and title aren't yet public information a rep would have, so the message doesn't use them.

---

## Input

> ## Account Brief — Court Street Lending (condensed)
> **Tier:** Tier 2 — €5B+ annual origination volume (per `icp.md`, this size moves an account into the longer-cycle, more-procurement-layers tier).
> **Lead persona for this brief:** Head of Credit Risk.
> **Positioning angle:** "Fast and unexplainable is a liability, not a feature" — same angle as the Nordkredit brief, since the persona is the same.
> **Why now:** A senior risk hire was recently announced — per `icp-buying-signal-monitor`, this is a Medium-strength signal (one data point, no corroborating tooling-migration signal the way Nordkredit had two).
> No prior contact with this account. No named contact yet — the hire was announced, not individually identified.

## Output

```
## Outbound Draft — Court Street Lending — Email

Subject: Your team's new risk hire

Hi [Name],

Congratulations on stepping into the role. I don't know yet whether a valuation-tooling review is anywhere on your list this early in — it often isn't for the first month or two — so I'd rather ask than assume it is.

If it does end up there this year, the question worth raising early is whether your current setup could hold up if an examiner asked exactly how a number was reached, not just what the number is. It's usually a gap teams inherit rather than one they chose.

If it'd help, happy to share what that conversation has looked like for other risk leads stepping into a similar seat recently — genuinely no pressure if it's too early for this.

[Rep name]

---
Personalization used: the recent Head of Credit Risk hire itself — the only confirmed detail about this account. No tooling migration is asserted, unlike the Nordkredit email, because none is confirmed here; per the skill's own rule against inventing a trigger, the message stays at the confidence level the actual signal supports.
```

## Why this is a weaker, more exploratory ask than the Nordkredit email — on purpose

- **No assumed trigger beyond the hire itself.** Nordkredit's brief had two corroborating signals (the hire *and* tooling-migration job postings), which earned a confident, specific ask ("worth a 15-minute conversation about how you're thinking about that requirement for the new setup"). This account has one signal, so the email doesn't borrow Nordkredit's confidence it hasn't earned here.
- **The ask is explicitly conditional** ("if it does end up there this year") rather than presuming an active evaluation — matches what's actually known, not what would make a punchier email.
- **Still specific, not generic** — this isn't a fallback to a template. "Congratulations on the hire, wondering if tooling is on your radar" is still built entirely from this account's one real, true detail; it's just honest about how much that one detail supports.
- **A rule worth generalizing:** match the confidence of the ask to the strength of the underlying signal, the same way [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor) already distinguishes Strong from Medium signals — this skill's output should visibly inherit that distinction rather than treating every brief as equally confident.
