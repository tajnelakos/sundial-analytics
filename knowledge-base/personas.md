# Buyer Personas — Sundial Analytics

Expands the persona list in [`knowledge-base.md`](./knowledge-base.md). Where [`icp.md`](./icp.md) names *which roles* sit on a buying committee and what's generally at stake for each, this document is what those roles actually think, say, and respond to — used by prompts/skills that need to tailor tone, structure, or emphasis to who's actually reading, not just confirm they exist. See [`sales-deck-builder`](../sales-tools/sales-deck-builder), [`persona-email-sequence`](../marketing-assets/persona-email-sequence), [`abm-account-brief`](../sales-tools/abm-account-brief), and [`sales-call-analysis`](./sales-call-analysis) for where this gets applied.

## How this maps to the buying committee

[`icp.md`](./icp.md)'s buying committee table names six roles. The three below with the deepest, most decision-shaping psychology get full persona treatment; the other three get a shorter entry, since their behavior is more procedural than psychological — the content that would actually change a rep's approach is thinner.

| Buying committee role (per `icp.md`) | Persona below | Depth |
|---|---|---|
| Economic buyer | [Head of Credit Risk](#head-of-credit-risk-economic-buyer-banklender-segment) | Full |
| Economic buyer (lending-ops) | [VP of Mortgage Lending](#vp-of-mortgage-lending-economic-buyer-lending-ops-angle) | Full |
| End user / brokerage buyer | [Broker Team Lead](#broker-team-lead-brokerage-segment-seat-based-product) | Full |
| Technical evaluator | [Credit Risk Analyst / Data Lead](#credit-risk-analyst--data-lead-technical-evaluator) | Full |
| IT/security reviewer | [IT Security Lead](#it-security-lead-infrastructure-gatekeeper) | Full |
| Procurement / compliance | [Vendor Risk & Compliance Reviewer](#vendor-risk--compliance-reviewer) | Shorter — mostly procedural |

## Persona interaction map

A deal rarely has one persona in the room — it has several, often with real tension between them, not just different priorities in parallel:

- **Head of Credit Risk vs. VP of Mortgage Lending** is the most common live tension: risk wants rigor, lending-ops wants speed, and neither will say the other's priority doesn't matter. The rep's job is to show the two aren't actually in conflict (a defensible valuation *is* a fast valuation once the audit-trail step is automated), not to pick a side. See the [Meridian Savings call](../knowledge-base/sales-call-analysis/call-02-meridian-savings.md) for this playing out directly.
- **Credit Risk Analyst / Data Lead is usually an ally, not a gatekeeper**, if engaged early — they want to be the one who validated the tool properly, and a rep who treats them as a rubber stamp loses that alliance. See the [Meadowbrook Financial call](../knowledge-base/sales-call-analysis/call-13-meadowbrook-financial.md), where the analyst's own evaluation rigor became the rep's strongest lever.
- **IT Security Lead answers to a different, often invisible-until-late master**: a specific regulator or internal data-governance policy, not the deal's momentum. They are the one persona here who can end a deal that every other stakeholder wants to close — see the [Solvane Lending Group call](../knowledge-base/sales-call-analysis/call-10-solvane-lending-group.md).
- **Vendor Risk & Compliance moves on its own clock**, largely deaf to sales urgency, and reacts badly to being chased directly rather than through the internal champion — see the [Thornfield Mutual call](../knowledge-base/sales-call-analysis/call-14-thornfield-mutual.md).

---

## Head of Credit Risk (economic buyer, bank/lender segment)

**Buying psychology:** Risk-averse by function, not by personality — their job is to be the person in the room who asks "how do we defend this to a regulator." Enthusiasm from other stakeholders makes them more skeptical, not less; they see their role as the check on that enthusiasm.

**Measured on:** Audit outcomes, exam findings (or absence of them), and — increasingly — how defensible the institution's automated decisions are under regulatory scrutiny. Not measured on loan volume or speed; a fast process that produces an indefensible decision is a mark against them, not a win.

**Pain, in their language:** *"I can't tell the auditor 'the model said so' — I need to be able to show my work."* *"Every vendor claims their AI is explainable. I've been burned by that claim before."* *"I don't need the best model. I need the one I can defend two years from now, after whoever ran it has left."*

**Decision criteria, ranked:**
1. Auditability / explainability of individual valuation decisions
2. Model accuracy, validated against a methodology they can scrutinize (not just a headline stat)
3. Vendor stability and data handling practices
4. Integration effort (real, but secondary to the above)

**Common objections:** "How is this different from [prior vendor]'s explainability claim that didn't hold up?" · "What happens to our data / model if we leave you?" · "Show me a valuation you got wrong and how the audit trail explained it."

**Trust triggers:** A vendor who volunteers a live demo on the buyer's own real data, unprompted. A vendor who says "we don't know, let me find out" rather than an immediate confident answer. A specific, named methodology detail rather than a general claim.

**Trust breakers:** Any claim that sounds identical to a prior vendor's claim that didn't hold up — this persona has usually been burned once already and pattern-matches hard against repeat offenses. Overclaiming accuracy without a disclosed methodology. Being asked to just "trust the model."

**Content preferences:** Methodology whitepapers, live demos on their own data over slides, peer references from similarly-regulated institutions. Actively distrusts case studies without a named, checkable source.

**Where they spend time:** Risk/compliance-focused LinkedIn groups, industry risk conferences, trade publications — not general SaaS/martech content channels.

**Seen in this repo:** [Nordkredit](../knowledge-base/sales-call-analysis/call-01-nordkredit.md) (Lena Virtanen — the clean, textbook version of this persona's mandate), [Court Street Lending](../knowledge-base/sales-call-analysis/call-03-court-street-lending.md) (David Okafor — the same psychology under a formal competitive bake-off), [Crestview Capital Bank](../knowledge-base/sales-call-analysis/call-11-crestview-capital-bank.md) (Ingrid Solberg — a regulatory-certification variant of the same core need for defensibility).

---

## VP of Mortgage Lending (economic buyer, lending-ops angle)

**Buying psychology:** Measured against throughput and cycle time, not risk metrics — success looks like "loans processed faster," not "audits passed." Will defer to the Head of Credit Risk on explainability but owns the workflow/speed conversation.

**Measured on:** Loan cycle time, borrower drop-off/abandonment rate, and team productivity. A tool that's more defensible but slower is, from this persona's KPIs alone, a regression — which is exactly why the tension with Head of Credit Risk (see the interaction map above) is real, not manufactured.

**Pain, in their language:** *"Every extra day in the valuation step is a day the borrower might walk to a competitor lender."* *"My team is doing manual workarounds around our current tool and I don't fully see where."* *"I need my risk team on board, but I'm not going to sell this internally for them."*

**Decision criteria, ranked:**
1. Speed / cycle-time reduction, ideally with a specific number
2. Integration into existing loan origination workflow (minimal new steps for loan officers)
3. Downstream effect on borrower experience
4. Alignment with what Credit Risk has already approved (won't fight that battle themselves)

**Common objections:** "Will my team need retraining, and how long does that take?" · "What's the actual time savings, not the theoretical one?"

**Trust triggers:** A specific, credible implementation timeline broken into real steps, not a marketing "instant" claim. A rep who separates "the tool goes live" from "my team actually adopts it" — this persona has been burned by vendors conflating the two.

**Trust breakers:** Being told competitor timelines are "instant" or "seamless" without qualification — this persona knows enough about their own workflow to smell an oversimplified claim. Being asked to advocate internally for the risk/compliance case themselves.

**Content preferences:** ROI/time-savings calculators, workflow diagrams, short case studies focused on operational metrics.

**Where they spend time:** Mortgage/lending operations trade publications, LinkedIn, regional banking associations.

**Seen in this repo:** [Meridian Savings](../knowledge-base/sales-call-analysis/call-02-meridian-savings.md) (Julia Hoffmann — the split-committee dynamic with Credit Risk, explicitly acknowledged mid-call), [Delta Mortgage Partners](../knowledge-base/sales-call-analysis/call-07-delta-mortgage-partners.md) (Sophie Larsen — the "instant vs. actually adopted" distinction surfacing directly against a Bricklane claim).

---

## Broker Team Lead (brokerage segment, seat-based product)

**Buying psychology:** Adoption-driven — the purchase only succeeds if agents actually use it, so they weigh "will my team bother opening this" as heavily as feature fit.

**Measured on:** Listing win rate, agent productivity, and — quietly — whether their last few tool purchases actually got used. A Broker Team Lead who's been burned by low adoption before will interrogate onboarding harder than price.

**Pain, in their language:** *"I've bought agent tools before that nobody used after month one."* *"I need something that helps agents close listings, not another dashboard to check."* *"Half my team barely uses the advanced features of what we already have."*

**Decision criteria, ranked:**
1. Agent adoption / ease of use (low friction to get value in first session)
2. Direct tie to closing listings (does this help win the listing appointment, not just inform it)
3. Price relative to per-seat value
4. Onboarding/support quality

**Common objections:** "How is this different from what's built into our CRM already?" · "What's the learning curve for a non-technical agent?"

**Trust triggers:** A rep who asks about the team's actual tech-comfort spread rather than assuming uniform ease of adoption. A referral from another brokerage with a specific, credible outcome (not a generic testimonial).

**Trust breakers:** A rep pushing a full-team rollout before adoption risk has been addressed. Feature-first pitches that don't address who on the team will actually open the tool.

**Content preferences:** Short demo videos, agent testimonials, simple one-pagers — not whitepapers.

**Where they spend time:** Real estate industry Facebook/LinkedIn groups, brokerage conferences, YouTube (agent-focused channels).

**Seen in this repo:** [Riverton Brokers](../knowledge-base/sales-call-analysis/call-04-riverton-brokers.md) (Tomas Reyes — adoption risk correctly identified as the real question, not the mobile feature gap itself), [Harborlight Brokerages](../knowledge-base/sales-call-analysis/call-12-harborlight-brokerages.md) (Dana Whitfield — a case where the rep correctly talked *out of* a low-value deal), [Copperfield Estates](../knowledge-base/sales-call-analysis/call-15-copperfield-estates.md) (Owen Marsh — a warm-referral case where adoption risk was already resolved by someone else's track record).

---

## Credit Risk Analyst / Data Lead (technical evaluator)

**Buying psychology:** Wants to be the one who validated the tool properly — treating this persona as a rubber-stamp step rather than a real technical reviewer is the single most common way a rep loses their support. They are usually not the final decision-maker, but a deal without their early buy-in tends to stall later at the procurement gate even if the economic buyer is enthusiastic (see [`icp.md`](./icp.md)).

**Pain, in their language:** *"I don't want to be the person who signed off on something that fell apart in front of an examiner."* *"Every vendor's demo looks clean. I want to see it break, or at least try to."*

**Decision criteria, ranked:**
1. Whether the audit trail holds up under a live test on real data they select, not a prepared demo
2. Disclosed accuracy methodology they can actually scrutinize
3. Integration feasibility with the specific systems they maintain
4. Whether the vendor treats their scrutiny as legitimate rather than an obstacle

**Common objections:** "Can we run this on a property we pick, not one you've prepared?" · "What's the actual methodology, not the confidence score?"

**Trust triggers:** A rep who invites a harder test than the one being requested. Being asked what evidence bar *they* think is fair, rather than being told what the evidence is.

**Trust breakers:** A rep who only offers prepared demo material when asked for something live. Any hint that their technical questions are an inconvenience.

**Seen in this repo:** [Meadowbrook Financial](../knowledge-base/sales-call-analysis/call-13-meadowbrook-financial.md) — the data/risk analyst whose own evaluation rigor (noting their team hadn't tested any vendor's audit trail live yet) became the strongest argument in the room, once invited rather than resisted.

---

## IT Security Lead (infrastructure gatekeeper)

**Buying psychology:** Not swayed by product enthusiasm from other stakeholders — answers to a data-governance policy or regulator, not the deal's momentum. Genuinely willing to end a deal everyone else wants, and doesn't experience that as a loss.

**Pain, in their language:** *"That's not a small gap for us — it's a hard requirement, not a nice-to-have."* *"I've had vendors dodge this question before, so directness helps."*

**Decision criteria, ranked:**
1. Data residency and processing location, against a specific regulatory requirement
2. Access control and audit-logging architecture
3. Whether the vendor gives a direct yes/no rather than a deflection

**Common objections:** "Does this support on-premises deployment?" · "Where specifically is data processed and stored?"

**Trust triggers:** An immediate, honest "no, we don't have that" when true, followed by a concrete next step (e.g. a compliance/infrastructure technical call) rather than a soft pivot.

**Trust breakers:** Any vendor response that reframes a hard requirement as a soft preference. A generic "we take security seriously" non-answer.

**Seen in this repo:** [Solvane Lending Group](../knowledge-base/sales-call-analysis/call-10-solvane-lending-group.md) (Erik Voss — a hard on-prem requirement stated plainly, handled honestly by the rep rather than talked around; see [`competitive-landscape.md`](./competitive-landscape.md)'s "Known gap working against us").

---

## Vendor Risk & Compliance Reviewer

**Buying psychology:** Operates on an internal review clock that has nothing to do with sales urgency — typically a queue-based process with its own timeline, largely independent of how convinced the economic buyer already is.

**Pain, in their language:** *"New vendor approvals move slowly here — I don't have much ability to expedite it."*

**Decision criteria, ranked:**
1. Standard security/compliance documentation completeness
2. Precedent — has a similar vendor been approved before
3. Absence of direct pressure from the vendor (a vendor reaching out directly can read as pressure, not helpfulness)

**Common objections:** Rarely objects directly — more often simply doesn't move, which reads as an objection if misdiagnosed as one.

**What actually helps:** Pre-prepared standard documentation handed to the internal champion, not this reviewer directly. Patience calibrated to their actual stated timeline, not repeated check-ins.

**Seen in this repo:** [Thornfield Mutual](../knowledge-base/sales-call-analysis/call-14-thornfield-mutual.md) — the champion (Grace Almeida) explicitly asked the rep not to contact compliance directly, and the deal's only open variable was this internal queue, not a product objection.

---

## Using personas together on one deal

Most real deals engage two or three of these personas at once, not one at a time — the practical skill is knowing which one is actually blocking progress at a given moment, since the answer changes across a deal's lifecycle: Credit Risk Analyst / Data Lead early (technical validation), Head of Credit Risk and VP of Mortgage Lending in the middle (the substantive decision, often in tension with each other), then IT Security and Vendor Risk & Compliance late (gates that can kill an otherwise-won deal). Treating a late-stage IT Security objection as if it were a Head of Credit Risk objection — i.e., trying to win it on explainability — is a common, avoidable mismatch.
