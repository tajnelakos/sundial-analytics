# Buyer Personas — Sundial Analytics

Expands the persona list in [`knowledge-base.md`](./knowledge-base.md). Used by prompts/skills that need to tailor tone, structure, or emphasis to who's actually reading — see [`sales-deck-builder`](../sales-tools/sales-deck-builder) and [`sales-call-analysis`](./sales-call-analysis) for where this gets applied.

---

## Head of Credit Risk (economic buyer, bank/lender segment)

**Buying psychology:** Risk-averse by function, not by personality — their job is to be the person in the room who asks "how do we defend this to a regulator." Enthusiasm from other stakeholders makes them more skeptical, not less; they see their role as the check on that enthusiasm.

**Pain, in their language:** *"I can't tell the auditor 'the model said so' — I need to be able to show my work."* *"Every vendor claims their AI is explainable. I've been burned by that claim before."*

**Decision criteria, ranked:**
1. Auditability / explainability of individual valuation decisions
2. Model accuracy, validated against a methodology they can scrutinize (not just a headline stat)
3. Vendor stability and data handling practices
4. Integration effort (real, but secondary to the above)

**Common objections:** "How is this different from [prior vendor]'s explainability claim that didn't hold up?" · "What happens to our data / model if we leave you?" · "Show me a valuation you got wrong and how the audit trail explained it."

**Content preferences:** Methodology whitepapers, live demos on their own data over slides, peer references from similarly-regulated institutions. Actively distrusts case studies without a named, checkable source.

**Where they spend time:** Risk/compliance-focused LinkedIn groups, industry risk conferences, trade publications — not general SaaS/martech content channels.

---

## VP of Mortgage Lending (economic buyer, lending-ops angle)

**Buying psychology:** Measured against throughput and cycle time, not risk metrics — success looks like "loans processed faster," not "audits passed." Will defer to the Head of Credit Risk on explainability but owns the workflow/speed conversation.

**Pain, in their language:** *"Every extra day in the valuation step is a day the borrower might walk to a competitor lender."* *"My team is doing manual workarounds around our current tool and I don't fully see where."*

**Decision criteria, ranked:**
1. Speed / cycle-time reduction, ideally with a specific number
2. Integration into existing loan origination workflow (minimal new steps for loan officers)
3. Downstream effect on borrower experience
4. Alignment with what Credit Risk has already approved (won't fight that battle themselves)

**Common objections:** "Will my team need retraining, and how long does that take?" · "What's the actual time savings, not the theoretical one?"

**Content preferences:** ROI/time-savings calculators, workflow diagrams, short case studies focused on operational metrics.

**Where they spend time:** Mortgage/lending operations trade publications, LinkedIn, regional banking associations.

---

## Broker Team Lead (brokerage segment, seat-based product)

**Buying psychology:** Adoption-driven — the purchase only succeeds if agents actually use it, so they weigh "will my team bother opening this" as heavily as feature fit.

**Pain, in their language:** *"I've bought agent tools before that nobody used after month one."* *"I need something that helps agents close listings, not another dashboard to check."*

**Decision criteria, ranked:**
1. Agent adoption / ease of use (low friction to get value in first session)
2. Direct tie to closing listings (does this help win the listing appointment, not just inform it)
3. Price relative to per-seat value
4. Onboarding/support quality

**Common objections:** "How is this different from what's built into our CRM already?" · "What's the learning curve for a non-technical agent?"

**Content preferences:** Short demo videos, agent testimonials, simple one-pagers — not whitepapers.

**Where they spend time:** Real estate industry Facebook/LinkedIn groups, brokerage conferences, YouTube (agent-focused channels).
