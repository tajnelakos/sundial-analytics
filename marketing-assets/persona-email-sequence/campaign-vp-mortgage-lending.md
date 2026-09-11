# Deep-Dive Campaign — VP of Mortgage Lending

A full 5-email, A/B-tested campaign for the lending-ops economic buyer, run against a 260-contact segment. Results: [`campaign-metrics.csv`](./campaign-metrics.csv) (raw sends) and [`campaign-performance-analysis.html`](./campaign-performance-analysis.html) (what the data actually says). See [`personas.md`](../../knowledge-base/personas.md#vp-of-mortgage-lending-economic-buyer-lending-ops-angle) for the persona this is built from.

**Trigger:** used the loan-cycle-time ROI calculator on the site.

**A/B design note:** same structure as the [Head of Credit Risk campaign](./campaign-head-of-credit-risk.md) — Variant A states the point declaratively with a specific number where one exists, Variant B leads with a direct question naming the cost of inaction. **Variant A won on every tracked metric for this persona** — the opposite result from the Head of Credit Risk campaign, where the question framing won. Don't read "provocative questions win" or "declarative numbers win" as a universal rule from either result in isolation — see the analysis for why the same technique cuts opposite ways for these two personas.

---

### Email 1 — Day 0

**Variant A:** "The cycle-time number lenders like you actually hit"
**Variant B:** "How many days are you losing in the valuation step?"

You ran the numbers on our calculator, so you've already seen the theoretical cycle-time gain — this is the actual figure lenders our size see in production, not the calculator's best case.

If you want to see where that time actually comes from (it's mostly one step, not a dozen small ones), a 15-minute walkthrough is enough to show it.

**Decision criterion advanced:** speed / cycle-time reduction with a specific number (ranked #1) — moves from the calculator's projection to a real, sourced figure.

---

### Email 2 — Day 3

**Variant A:** "Where this actually plugs into your loan officers' day"
**Variant B:** "No new steps for your loan officers (really)"

The cycle-time number only means something if your loan officers don't have to change how they work to get it — so here's specifically where this sits in the existing loan origination workflow, not a new tool they have to remember to open.

Happy to map it against your specific LOS if that'd save you a step later in this evaluation.

**Decision criterion advanced:** integration into existing loan origination workflow (ranked #2) — addresses this persona's stated concern about retraining time directly, rather than asserting "easy" without specifics.

---

### Email 3 — Day 7

**Variant A:** "What borrowers notice when the wait disappears"
**Variant B:** "The abandonment number nobody tracks until it's too late"

Cycle time matters operationally, but the number that tends to get missed until a QBR is borrower drop-off during the valuation wait — this is what changes downstream once that step compresses.

If borrower abandonment is something you're already tracking, this is worth five minutes even if the rest of this evaluation is still early.

**Decision criterion advanced:** downstream effect on borrower experience (ranked #3) — a different angle from the internal-workflow focus of Email 2, not a restatement of it.

---

### Email 4 — Day 12

**Variant A:** "A real rollout timeline, not a 'go-live in a day' claim"
**Variant B:** "What week one, four, and twelve actually look like"

You've probably had a vendor tell you this goes live "instantly" — that's rarely the useful number, since going live and your team actually working differently are two different milestones.

Here's the real week-by-week: technical integration, a pilot cohort of loan officers, then full rollout. Worth comparing against whatever timeline you're being told elsewhere.

**Decision criterion advanced:** re-approaches integration effort through this persona's specific trust trigger — "a rep who separates 'the tool goes live' from 'my team actually adopts it'" — rather than a general reassurance.

---

### Email 5 — Day 18

**Variant A:** "You don't have to sell this to your risk team"
**Variant B:** "The one slide that gets Risk and Ops on the same page"

Last email in this sequence. One thing worth naming directly: this persona's `personas.md` entry is explicit that this buyer won't advocate internally for the risk/compliance case themselves, and being asked to is a stated trust breaker — so this email doesn't ask that.

If it'd help, we can put together a short, joint walkthrough for you and whoever owns the risk side, so the audit-trail conversation happens in the room with both of you rather than becoming a second sales cycle you have to run yourself.

**Decision criterion advanced:** alignment with what Credit Risk has already approved (ranked #4) — closes the sequence by removing the one friction point this persona's own profile flags as most likely to stall the deal, without asking them to do the risk team's job.

---

## Reply handling for this campaign

See [`reply-handling-playbook.md`](./reply-handling-playbook.md)'s VP of Mortgage Lending section for response templates by reply type (timeline pushback, "send this to my risk lead," retraining concern, hard no).
