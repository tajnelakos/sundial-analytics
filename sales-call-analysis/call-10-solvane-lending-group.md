# Call Transcript — Solvane Lending Group

**Date:** July 2026 · **Duration:** ~18 minutes · **Call type:** Third call, technical validation
**Rep:** Marcus Webb (Sundial Analytics) · **Prospect:** Karin Lindqvist, VP of Mortgage Lending, Solvane Lending Group (national lender); joined by Erik Voss, IT Security Lead

---

**Marcus:** Karin, Erik, thanks for both joining. Last time we covered the product fit — my understanding is this call is more about technical and security requirements. Is that right?

**Erik:** Correct. Product side is sold, mostly. My job today is to make sure this actually fits our infrastructure requirements before this goes further.

**Marcus:** Understood, go ahead.

**Erik:** Our data governance policy requires on-premises deployment for any system that touches customer-identifiable financial data. That's not a preference, it's a compliance requirement from our board. Does Sundial support on-prem?

**Marcus:** I want to answer this directly rather than soften it: no, we don't currently offer on-premises deployment. We're a cloud-hosted platform.

**Erik:** That's a problem. That's not a small gap for us — it's a hard requirement, not a nice-to-have.

**Marcus:** I understand, and I'd rather you hear that clearly now than have it surface after more of your time is invested. Can I ask — is the on-prem requirement about data residency specifically, or about not trusting cloud infrastructure generally, or something else? I ask because the underlying concern sometimes has more than one possible solution.

**Erik:** Mostly data residency and control — our regulator has specific expectations about where and how customer financial data is processed and stored.

**Marcus:** Okay. I don't have an on-prem product to offer you, so I'm not going to pretend there's a workaround that doesn't exist. What I can do is connect you with our compliance team to understand exactly how our cloud infrastructure handles data residency and processing controls — some regulators accept a well-documented cloud architecture with the right certifications, others don't. I don't know which category yours falls into, and I'd rather find that out accurately than guess.

**Karin:** Erik, is that worth exploring, or is this a hard no regardless of the specifics?

**Erik:** Depends on the details, honestly. If their cloud architecture has strong enough residency and access controls, our regulator might accept it — we've had that conversation before with other cloud vendors, it's not automatically disqualifying. But if it doesn't, this is a dead end for us.

**Marcus:** That's a fair distinction, and I'd rather get you a precise, honest answer than keep this conversation alive on false hope. I'll set up a call between you and our compliance/infrastructure team specifically to go through data residency and access controls in detail — and if the answer is genuinely "this doesn't meet your requirement," I'll tell you that directly rather than stringing this out.

**Erik:** I'd appreciate that. I've had vendors dodge this question before, so directness helps.

**Karin:** If it doesn't work out, for what it's worth, I'd want to stay in touch for possible future fit — we're still not thrilled with Estemate, on-prem or not.

**Marcus:** Understood, and I'll treat that separately regardless of how the infrastructure conversation goes. I'll get the technical call scheduled this week.

---

## Internal notes (rep-logged)

- **Hard, confirmed blocker**: on-premises deployment requirement, tied to a board-level data governance policy, not a soft preference — matches the exact gap already documented in `competitive-landscape.md`'s "Known gap working against us." This is a real, live instance of that documented risk materializing, not a hypothetical.
- Correctly did not oversell or imply a workaround that doesn't exist — directly acknowledged the gap and proposed a real, bounded next step (compliance/infrastructure technical call) rather than stringing the deal along.
- Genuinely uncertain outcome: depends on whether Solvane's regulator accepts a well-documented cloud architecture — this is a fair test case for whether the on-prem gap is truly disqualifying everywhere, or only where cloud isn't independently justifiable. Worth tracking the outcome specifically to update `competitive-landscape.md`'s framing (currently states the gap "is a case for product, not something a battlecard talk track can talk around" — this call is a real test of that).
- Estemate is the incumbent here too, and the prospect signaled openness to switching regardless of this deal's outcome — worth a separate, lower-pressure follow-up track independent of the on-prem resolution.
- Escalate to product/leadership: this is now the second documented account (see also implied volume in `competitive-landscape.md`) where on-prem is a literal deal-blocker, not just a stated preference — worth prioritizing for a real roadmap conversation rather than continuing to treat it as a known-but-deprioritized gap.
