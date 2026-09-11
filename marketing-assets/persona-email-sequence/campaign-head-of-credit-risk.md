# Deep-Dive Campaign — Head of Credit Risk

The [`example.md`](./example.md) quick-mode sequence for this persona, extended into a full 5-email, A/B-tested campaign — same trigger context, same decision-criteria backbone, run for real against a 240-contact segment. Results: [`campaign-metrics.csv`](./campaign-metrics.csv) (raw sends) and [`campaign-performance-analysis.html`](./campaign-performance-analysis.html) (what the data actually says). See [`personas.md`](../../knowledge-base/personas.md#head-of-credit-risk-economic-buyer-banklender-segment) for the persona this is built from.

**Trigger:** downloaded the "Explainability in Automated Valuation" whitepaper.

**A/B design note:** every email tests two subject-line framings against the same body copy — Variant A states the point directly (declarative, matches this persona's stated preference for a "specific, named methodology detail rather than a general claim"); Variant B names their specific fear as a direct question. Body copy is held constant across variants on purpose — varying both subject and body at once would make it impossible to attribute a performance difference to either one. **Variant B won on every tracked metric for this persona** (see the analysis) — naming the exact question they're afraid an examiner will ask outperformed stating the same fact declaratively, even for a buyer who is explicitly skeptical of anything that sounds like a marketing hook.

---

### Email 1 — Day 0

**Variant A:** "The part most 'explainable AI' claims skip"
**Variant B:** "What your auditor will actually ask"

You downloaded our piece on explainability in automated valuation, so you're probably already skeptical of the term — most vendors use it to mean "we show a confidence score," not "we can show our work."

The difference matters most in an audit, not a demo. If you want to see what a comparable-level audit trail actually looks like on a real valuation (not a curated example), it takes about 15 minutes.

**Decision criterion advanced:** auditability / explainability of individual decisions (ranked #1) — moves from the whitepaper's general argument to a concrete, inspectable example.

---

### Email 2 — Day 4

**Variant A:** "How we validate accuracy (and how to check our work)"
**Variant B:** "Show me your math: our accuracy methodology"

Following up on explainability — the other question worth asking any vendor is how they validate accuracy, and whether that methodology is something you can actually scrutinize or just a headline number.

Our benchmarking approach is documented, not just claimed. Worth a look if you're building a shortlist criteria doc for this evaluation.

**Decision criterion advanced:** model accuracy validated against a disclosed methodology (ranked #2) — distinct from Email 1's audit-trail focus.

---

### Email 3 — Day 9

**Variant A:** "What changes (and what doesn't) if you switch"
**Variant B:** "The migration conversation, without the sales spin"

Last thing worth covering before this starts feeling like too many emails: what actually changes operationally if you moved off your current tooling, and what stays the same.

Integration effort is real but usually smaller than teams expect going in — happy to walk through what that'd look like for your setup specifically, no pressure if the timing isn't right.

**Decision criterion advanced:** vendor stability / integration effort (ranked #3–4) — closes the loop on the remaining lower-ranked concerns without urgency tactics.

---

### Email 4 — Day 15

**Variant A:** "A community bank's examiner asked the same question you're asking"
**Variant B:** "What a similarly-regulated peer told their examiner"

A regional bank on our platform got asked, mid-exam, to walk the examiner through exactly how three flagged valuations were reached — comparables, weighting, all of it. Their risk lead pulled the audit trail directly and answered it in the room, not with a follow-up call two weeks later.

That's a peer reference you can actually check, not a case study with the names filed off — happy to connect you directly if that'd be useful before you go further with this.

**Decision criterion advanced:** auditability, re-approached through a peer reference — this persona's own trust triggers name "peer references from similarly-regulated institutions" specifically, and this is the email built around that trigger rather than another angle on the same product claim.

---

### Email 5 — Day 22

**Variant A:** "Worth 15 minutes on your own data?"
**Variant B:** "An offer other vendors won't make you"

This is the last email in this sequence — not because the conversation has to end here, but because a fifth follow-up on the same topic stops being useful and starts being noise.

If it'd help, we'll run a live valuation on a property you pick, not one we've prepared, and walk through the audit trail on it together. If the timing genuinely isn't right, that's a fine answer too.

**Decision criterion advanced:** closes the sequence on the persona's strongest stated trust trigger — "a vendor who volunteers a live demo on the buyer's own real data, unprompted" — rather than an urgency push, which this persona's `personas.md` entry explicitly flags as a trust *breaker*, not a trigger.

---

## Reply handling for this campaign

See [`reply-handling-playbook.md`](./reply-handling-playbook.md)'s Head of Credit Risk section for response templates by reply type (technical objection, peer-reference request, "forwarded to our analyst," hard no).
