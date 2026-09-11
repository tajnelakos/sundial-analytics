# Reply-Handling Playbook

Nurture sequences generate replies that don't fit "book a meeting" or "unsubscribe" — a technical objection, a request to loop in someone else, a polite non-answer. This playbook maps reply types to response guidance, per persona, so a rep or SDR triaging a shared inbox doesn't have to improvise a tone match on every reply. Pairs with [`campaign-head-of-credit-risk.md`](./campaign-head-of-credit-risk.md) and [`campaign-vp-mortgage-lending.md`](./campaign-vp-mortgage-lending.md); the reply categories are the same across personas, the right response isn't.

## General rules, both personas

- **Reply within one business day.** A fast reply to an inbound response matters more than a polished one — see [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md) for tone, but don't let voice-polishing delay the reply itself.
- **Never send a templated reply that ignores what they actually wrote.** Every template below is a starting point to personalize against their specific wording, not a copy-paste.
- **Stop the sequence the moment someone replies**, regardless of reply type — a scheduled Email 3 landing on top of an unresolved objection reply reads as not having read their message.
- **A reply that raises an objection is a better outcome than no reply.** Route it to the rep, don't try to fully resolve a substantive objection inside the automated sequence's reply-handling step.

---

## Head of Credit Risk

This persona's `personas.md` entry: risk-averse by function, has usually been burned by a prior vendor's explainability claim, distrusts anything that reads as a soft answer.

### "Can you send me the methodology doc directly, not just describe it?"
**Read:** A genuine technical evaluation step, not stalling — this is exactly the behavior the persona profile predicts ("actively distrusts case studies without a named, checkable source").
**Response guidance:** Send the actual methodology documentation immediately, not a summary. If a live version doesn't exist yet, say so plainly and give a specific date it will, rather than a vague "I'll follow up." This persona's trust triggers explicitly reward "we don't know, let me find out" over a confident non-answer.

### "How is this different from [prior vendor]'s explainability claim that fell apart?"
**Read:** The single most predictable objection for this persona — `personas.md` names it directly as a common objection.
**Response guidance:** Don't get defensive or imply the prior vendor was simply wrong. Ask what specifically fell apart (methodology, a live audit, an exam finding) and answer that specific failure mode directly — a generic "we're different" answer pattern-matches as exactly the claim they're already skeptical of.

### "I've forwarded this to our data/risk analyst to take a look."
**Read:** A good sign, not a brush-off — per `personas.md`'s persona interaction map, the Credit Risk Analyst / Data Lead is usually an ally if engaged early, and this Head of Credit Risk is routing correctly rather than rubber-stamping.
**Response guidance:** Offer to loop in directly with the analyst rather than waiting for them to reach out — and treat the analyst's technical questions as legitimate scrutiny, not an obstacle, when they arrive.

### "Not the right time — we're mid-exam cycle / just renewed with our current vendor."
**Read:** Often a real, specific timing constraint for this persona, not a soft no — regulated institutions have exam calendars that genuinely gate vendor evaluation bandwidth.
**Response guidance:** Ask for (or infer, if given) a specific re-engagement point rather than a generic "circle back in Q_" — then actually wait for it. Re-approaching before the stated timing reads as exactly the pressure this persona's profile flags as a trust breaker.

### Hard no / unsubscribe
**Response guidance:** No reply needed beyond confirming the unsubscribe request is honored. Don't send a "sorry to see you go" retention email — this persona's profile suggests that reads as pressure, not warmth.

---

## VP of Mortgage Lending

This persona's `personas.md` entry: measured on cycle time and throughput, won't advocate internally for the risk/compliance case, wants a real implementation timeline rather than an "instant" claim.

### "What's the actual retraining time for my loan officers?"
**Read:** A direct hit on this persona's stated common objection — answer with the real number, not a range that sounds better than it is.
**Response guidance:** Give the honest figure, broken down by what's genuinely new versus what stays the same in the existing workflow. If the honest answer is "more than a day," say that — this persona's trust trigger is explicitly "a rep who separates 'the tool goes live' from 'my team actually adopts it.'"

### "What's the real time savings, not the marketing number?"
**Response guidance:** Point to a sourced, specific figure (the same one used in Email 1) rather than restating the calculator's theoretical output — and offer a reference call with an existing lending-ops customer if one exists, since this persona's content preferences skew toward operational-metric case studies over slides.

### "Can you send this to our risk lead / send a version for compliance?"
**Read:** This is the single most important reply type for this persona — `personas.md` states directly that this buyer "won't sell this internally for them" on the risk side, so a request to loop in risk is the sequence working as intended, not a detour.
**Response guidance:** Offer the joint walkthrough described in [`campaign-vp-mortgage-lending.md`](./campaign-vp-mortgage-lending.md)'s Email 5, and reach out to the risk contact directly rather than routing everything back through the VP — this removes exactly the internal-selling burden the persona profile flags as a trust breaker if left on them.

### "We're not prioritizing this right now — cycle times are fine."
**Read:** Possibly a genuine low-priority signal, but per `personas.md`'s pain language ("my team is doing manual workarounds ... and I don't fully see where"), this can also mean the pain is real but not yet visible to this specific person.
**Response guidance:** One light follow-up offering the borrower-abandonment data point (Email 3's angle) is reasonable if it wasn't already covered — a downstream metric this persona may not be tracking yet. Don't push past a second soft no.

### Hard no / unsubscribe
**Response guidance:** Same as Head of Credit Risk — honor immediately, no retention email.
