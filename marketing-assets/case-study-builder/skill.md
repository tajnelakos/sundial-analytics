---
name: case-study-builder
description: Builds a customer case study from a real closed-won deal's actual data — CRM record, call transcript, logged decision driver — never inventing a result, quote, or outcome that isn't traceable to that source. Use when the user names a specific closed-won account and wants a case study, not a generic customer-story template.
---

# Case Study Builder

## Purpose

Case studies are usually the most fabricated piece of B2B content in the building — a customer story assembled from a rep's memory, a testimonial quote nobody actually said out loud, and a result rounded up because the real number wasn't impressive enough. This skill applies the same real-source discipline the rest of this repo already requires ([`personalized-outbound`](../personalized-outbound), [`positioning-compliance`](../positioning-compliance)) to case studies specifically.

## Instructions

1. **Require real source material.** A CRM record (deal size, sales cycle, logged decision driver, competitor faced) and/or a call transcript or rep notes for the named account. If given only a company name with no real detail behind it, say so and ask for the source — don't invent a plausible-sounding challenge and result.
2. **Structure:** Title, Snapshot, Challenge (the buyer's actual pain, in their own language if a transcript exists), Solution (the specific thing that won this deal, not a generic feature list), Results (quantified, each traceable to source), Quote (only if real and attributable), Positioning tie-in.
3. **Every quantitative claim must trace to the CRM record or transcript.** Treat this the same way [`positioning-compliance`](../positioning-compliance/skill.md) treats an unsupported claim — a hard fail, not a stylistic nitpick. Run the finished case study through that skill before treating it as ready to publish.
4. **A quote from an internal sales-call transcript is not automatically a usable public testimonial.** Flag explicitly that the customer's separate consent to be quoted and named publicly is required before this ships — "it's in our call notes" is not "we're allowed to publish it." State plainly whether the draft is meant to run named (pending sign-off) or anonymized.
5. **Don't borrow a result from a different account** to make this one look stronger — a common failure mode when the real numbers for this specific deal aren't as striking as another deal's.
6. **Follow [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules.**
7. **Tie the outcome to exactly one [`positioning.md`](../../knowledge-base/positioning.md) message-house pillar** — not "we help with everything."

## What to avoid

- Don't fabricate a customer quote or attribute words to someone that aren't in the source transcript.
- Don't invent a numeric result beyond what's in the CRM/transcript — mark anything unconfirmed as a follow-up question for the account team, not a filled-in guess.
- Don't treat "closed-won" as "we know the full story" — state plainly what the source material does and doesn't confirm.

## Output format

```
## Case Study — [Account Name]

**Status:** Draft — pending customer sign-off to publish / Ready to publish

**Title:** [Customer] chose Sundial to [specific result]
**Snapshot:** [segment · tier · region · deal size · sales cycle · competitor displaced]

### Challenge
[the real pain, sourced]

### Solution
[what was actually evaluated and won, sourced]

### Results
- [quantified outcome, traceable to source]
- [quantified outcome, traceable to source]

### Quote
[a real, attributable quote and its consent status — or a plain statement that none exists yet]

---
Positioning tie-in: [the one pillar this demonstrates]
Sourced from: [citations]
What's not confirmed: [anything the source material doesn't actually establish]
```
