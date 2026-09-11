# Competitive Landscape — Sundial Analytics

Full battlecard reference. The summary table in [`knowledge-base.md`](./knowledge-base.md) is the quick version; this is what [`competitor-monitoring`](../sales-tools/competitor-monitoring), [`battlecard`](../sales-tools/battlecard), and [`win-loss-analysis`](./win-loss-analysis) draw on for deeper context.

**Last full refresh:** September 2026, following a [`staleness-detection`](./staleness-detection) sweep against the July–August bi-monthly competitor report and the trailing-12-month win-loss deep dive — see [`sweep-2026-09.md`](./staleness-detection/sweep-2026-09.md) for exactly what changed and why. Per-competitor "Last verified" dates below track individual sections.

## Executive summary

Three real competitors in the bank/lender segment, none with a decisive product edge — deals are won or lost in the risk conversation, not the demo. Bricklane is the highest-frequency threat (price-led, weak on explainability); ValuAI is the fastest-moving one — its audit trail shipped in July 2026 and it's now competing on price too, though we're 8-for-8 against it this period (small sample, closing gap, not a reason for confidence); Estemate is fading but still wins on relationship tenure and on-prem support — and still beats us more often than any other named competitor (72.7% win rate for them when faced, per the [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html)), which is worth remembering before assuming the flashier competitor is the bigger threat. Our two live vulnerabilities are price and the on-prem gap — see [Known gap working against us](#known-gap-working-against-us).

## Company profiles

| Competitor | Founded | Size | Funding | Target market | Core value prop |
|---|---|---|---|---|---|
| Bricklane Data | 2021 | ~80 employees | Series A (~$15M) | Mid-market lenders, EU-wide | Fastest, cheapest valuations |
| Estemate | 2005 | ~450 employees | Private, no disclosed VC | Large + regional banks, France/Benelux | Two decades of trusted valuation data |
| ValuAI | 2022 | ~120 employees | Series B (~$60M) | Forward-leaning banks/lenders, EU-wide | AI-native valuations built for what's next |
| PropIQ | 2019 | ~40 employees | Bootstrapped/seed | Independent brokerages | Valuation insight that helps agents close listings |

*(Source: general market knowledge, not independently verified — reconfirm before citing a specific figure to a prospect.)*

## Quick reference — read this before a call

| Competitor | Threat level | Segment | Win angle | Landmine — don't say |
|---|---|---|---|---|
| [Bricklane Data](#bricklane-data) | 🔴 High — most frequent competitor in losses (13 of 35 lost deals, Q1) | Bank/lender | Reframe price → cost of an indefensible decision | Don't price-match — it concedes the frame that this is a commodity |
| [ValuAI](#valuai) | 🟠 Medium-High — GA'd their audit trail in Jul 2026; 0-for-8 against us since, but that's a small sample and the gap is closing, not a reason for confidence | Bank/lender | Ask for proof at scale (named reference, live test on their data) — existence of the feature is no longer the wedge | Don't call it "still in beta" — it shipped; don't assume our current win rate against them will hold |
| [Estemate](#estemate) | 🟠 Medium-High — revised up: wins 72.7% of deals it contests (n=11), despite the least exciting product story of the three | Bank/lender (Benelux-heavy) | Modern UX + faster implementation, once a frustrated stakeholder is in the room | Don't attack the relationship tenure — it's their strongest card, and it's working better than this document previously credited |
| [PropIQ](#propiq) | ⚪ Low — different segment | Brokerage | N/A — rarely a head-to-head bank/lender deal | N/A |

## Capability comparison

Illustrative — not a substitute for a live demo comparison.

| | Sundial | Bricklane Data | Estemate | ValuAI |
|---|---|---|---|---|
| Comparable-level audit trail | ✅ Yes | ❌ Confidence score only | ⚠️ Partial, dated format | ⚠️ GA since Jul 2026, but reportedly weaker on commercial/mixed-use than residential (see [`call-09-ironbridge-bank.md`](./sales-call-analysis/call-09-ironbridge-bank.md)) |
| Accuracy methodology disclosed | ✅ Yes | ❌ Not published | ✅ Yes, established track record | ❌ Claimed, not disclosed |
| On-prem deployment | ❌ No — current gap, see [win-loss data](./win-loss-analysis/win-loss-infographic.svg) | ❌ Cloud only | ✅ Yes (legacy architecture) | ❌ Cloud only |
| Implementation timeline | Weeks | Fastest — self-serve | Slowest — legacy integration | Medium |
| Pricing model | Usage-based (per-call) | Usage-based, ~15% below Sundial | Enterprise/negotiated, typically higher | Not publicly disclosed; averaged ~9% below our deal size in Q3 head-to-heads (n=8, see [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html)) |

The on-prem gap is real, not a competitor's weakness — flag it early with a prospect that requires it rather than letting it surface late in the deal.

## Pricing & packaging

| Competitor | Model | Notes |
|---|---|---|
| Sundial | Usage-based (per-call API), seat-based for brokerage app | No self-serve tier for the bank/lender product — sales-assisted only |
| Bricklane Data | Usage-based, ~15% below Sundial | Self-serve signup, no enterprise tier disclosed — built for fast adoption without procurement |
| Estemate | Enterprise/negotiated only | Multi-year contracts typical, no self-serve option |
| ValuAI | Not publicly disclosed | Sales-assisted only. The "premium-priced" assumption didn't hold up in Q3 head-to-heads — their average quote came in below our average deal size (see [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html)); price is now part of their play, not just capability |
| PropIQ | Seat-based, tiered by team size | Freemium single-seat trial available |

## Marketing & positioning

| Competitor | Primary channel | Core message | Persona emphasis |
|---|---|---|---|
| Bricklane Data | Paid search, self-serve signup funnel | Speed + price | Procurement/ops buyers |
| Estemate | Direct sales, industry conferences | Trust and tenure | Risk-averse senior stakeholders |
| ValuAI | Content marketing, conference sponsorships, aggressive LinkedIn presence | "AI-native," technology leadership | Innovation-minded buyers — sometimes reaches the buyer before the risk function does |
| PropIQ | Real estate industry communities, webinars | Agent productivity | Broker team leads |

## Customer sentiment

| Competitor | Rating | Praise | Complaint |
|---|---|---|---|
| Bricklane Data | ~4.3/5 (G2, ~40 reviews) | Speed, easy self-serve setup | Support "felt automated"; accuracy questioned in edge cases |
| Estemate | ~3.6/5 (G2, ~90 reviews) | Data depth, reliability | Slow support response, dated UI *(confirmed — see [competitor-monitoring/example](../sales-tools/competitor-monitoring/weekly-brief-example.md))* |
| ValuAI | ~4.1/5 (G2, ~25 reviews — newer product) | Modern UI, strong demo experience | A few reviews mention promised features not yet available |
| PropIQ | ~4.5/5 (Capterra) | Easy agent adoption | Limited to brokerage use case, not built for lenders |

*(Source: illustrative review patterns, not pulled from a live G2/Capterra feed — treat ratings as directional, not exact.)*

---

## Bricklane Data

**Quick facts:** Threat level 🔴 High · Bank/lender segment · 13 of 35 Q1 losses · Last verified: March 2026 (per [win-loss-analysis](./win-loss-analysis/win-loss-infographic.svg))

**Positioning:** Speed and price. Their pitch is "valuations in seconds, at the lowest per-call cost in the market."

**Strengths:** Genuinely fast, aggressive pricing, easy self-serve API onboarding — appeals to buyers who haven't yet hit an audit-defensibility problem. *(Source: 3 lost-deal notes, Q1)*

**Weaknesses:** Explainability is thin — confidence score with no comparable-level breakdown. No dedicated compliance/audit-log feature. *(Source: product comparison, unconfirmed independently — worth a live demo comparison before repeating as certain)*

**How we win:** Reframe the conversation from price-per-call to cost-of-an-indefensible-decision. Works best once the Head of Credit Risk (not just procurement) is in the room — see [`personas.md`](./personas.md).

**How we lose:** Deals that stay procurement-led and never reach a real risk conversation; deals where price sensitivity dominates because the institution hasn't yet had an audit incident.

**Objection handling:** "Bricklane is 15% cheaper" → don't price-match; quantify the audit/rework cost of an unexplainable valuation instead, and offer a side-by-side audit trail comparison.

**Landmines — don't say:** Don't claim Bricklane's valuations are "inaccurate" — no evidence supports that, and an overclaim here is the kind of thing that gets fact-checked and costs credibility. The honest gap is explainability, not accuracy.

**Trigger signals it's in the deal:** Prospect asks about per-call pricing early, before asking about methodology.

---

## Estemate

**Quick facts:** Threat level 🟠 **Medium-High (revised up from Medium)** · Bank/lender segment, Benelux-heavy · Last verified: September 2026, via [`staleness-detection`](./staleness-detection) sweep (see [`sweep-2026-09.md`](./staleness-detection/sweep-2026-09.md))

**Why the threat level moved:** Win-loss data shows a 27.3% win rate *for us* when Estemate is the named competitor (n=11) — meaning Estemate wins nearly three-quarters of the deals it contests, the worst of any named competitor in this book, despite being the one with the least exciting product story. See the [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html). The lesson isn't that Estemate got stronger this period — it's that this document was previously rating threat by how compelling a competitor's pitch sounds, not by how often they actually win.

**Positioning:** Legacy incumbent, especially entrenched in France/Benelux. Sells on relationship tenure and breadth of historical data.

**Strengths:** Long-standing customer relationships, large historical dataset, strong brand recognition in Benelux specifically. On-prem deployment available, which we currently can't match. *(Source: general market knowledge — worth reconfirming against a specific deal)*

**Weaknesses:** Dated UI, slow release cadence, publicly documented support responsiveness issues. *(Source: 2 public G2 reviews, confirmed — see [competitor-monitoring/example](../sales-tools/competitor-monitoring/weekly-brief-example.md))*

**How we win:** Modern integration experience and faster implementation timeline; strongest against Estemate when the buying committee includes someone frustrated with the current tool's UX or support.

**How we lose:** Deeply entrenched relationships where switching cost (real or perceived) outweighs product gaps; risk-averse buyers who default to "nobody gets fired for choosing the incumbent"; any deal requiring on-prem deployment.

**Objection handling:** "We've used Estemate for 10 years" → don't attack the relationship; focus on a specific, current pain point (support responsiveness, release velocity) rather than a general pitch to switch.

**Landmines — don't say:** Don't lead with "Estemate is outdated" as a blanket claim — it reads as disrespecting the buyer's own long-standing choice. Let a specific, named pain point (support ticket age, missing feature) do the work instead.

**Trigger signals it's in the deal:** Prospect is Benelux-based; prospect mentions a slow support ticket or a feature request that's been open a long time; prospect states an on-prem requirement.

---

## ValuAI

**Quick facts:** Threat level 🟠 Medium-High · Bank/lender segment · Last verified: **September 2026**, via [`staleness-detection`](./staleness-detection) sweep (see [`sweep-2026-09.md`](./staleness-detection/sweep-2026-09.md)) — next recheck due October 2026, since this is still the fastest-moving section in this document.

**Positioning:** "AI-native" challenger, well-funded, leads with technology-forward messaging — as of this period, also reaching for "regulatory-ready" language (see [`competitor-monitoring`](../sales-tools/competitor-monitoring)'s bi-monthly report).

**Strengths:** Strong initial sales narrative, modern-feeling product demo, aggressive marketing presence, and — as of July 2026 — a shipped, GA audit-trail feature. *(Source: market observation; [bi-monthly-report-2026-07-08.md](../sales-tools/competitor-monitoring/bi-monthly-report-2026-07-08.md))*

**Weaknesses:** No longer "the feature doesn't exist" — it shipped. The current, more precise weakness: adoption evidence is thin (one named enterprise reference customer, no independent validation at scale) and it reportedly performs worse on commercial/mixed-use properties than residential. *(Source: [`call-09-ironbridge-bank.md`](./sales-call-analysis/call-09-ironbridge-bank.md); see [`battlecard/valuai.html`](../sales-tools/battlecard/valuai.html) for the fully updated talk track)*

**How we win:** Our clearest differentiation lane has moved from *existence* to *proof at scale* — offer a live audit trail on the buyer's own data, and ask ValuAI to do the same. This is working: **0 of 8 head-to-head deals against ValuAI were won by them this period** (see [win-loss deep dive](./win-loss-analysis/win-loss-detailed-analysis.html)). Don't read that as settled, though — 8 deals is a small sample, and their capability gap is closing, not widening.

**How we lose:** Early-stage deals where the buyer hasn't yet pressure-tested ValuAI's claims and is still impressed by the demo — and, newly, deals where their now-lower quoted price is the deciding factor rather than capability at all.

**Objection handling:** "ValuAI says they're explainable too" → don't dispute it, it's true now. Invite direct comparison instead ("ask them to show the actual comparable-level audit trail on a real valuation, then ask us the same") and, if the property type is commercial or mixed-use, that comparison favors us more specifically than it used to.

**Landmines — don't say:** Don't say the audit-trail feature "doesn't exist" or is "still in beta" — it shipped in July 2026, and repeating the old claim is exactly the kind of thing that gets fact-checked and costs credibility. Don't over-rely on the current 0-for-8 win-loss record either — it's real, but it's recent and small, not a permanent advantage.

**Trigger signals it's in the deal:** Buyer uses the word "AI-native," references a recent ValuAI demo, or brings up their audit trail feature by name — worth asking directly whether they've seen it live on their own data or only in a demo.

---

## PropIQ

**Quick facts:** Threat level ⚪ Low · Brokerage segment · Last verified: March 2026

**Positioning:** Brokerage-focused, doesn't meaningfully compete in the bank/lender segment.

**Relevance:** Comes up mainly in brokerage deals or occasionally when a bank buyer also has a brokerage arm evaluating tools separately. Not a primary battlecard priority outside the brokerage segment — deprioritize deepening this section unless brokerage-segment deal volume increases.

---

## Positioning gaps to exploit

1. **No competitor has a credible, specific answer to "show me the audit trail on a real valuation, not a demo one"** — this is the single highest-leverage moment in a competitive deal (see [`positioning.md`](./positioning.md)).
2. **Support responsiveness is a live, public weakness for Estemate** — usable in Benelux-specific battlecards without needing to fabricate anything, since it's evidenced in public reviews.
3. **Bricklane's price-led positioning has no answer to a risk-framed objection** — reframing the conversation away from price is more effective than matching it.

## Known gap working against us

**On-prem deployment** is not currently offered and was the #2 reason for lost deals in Q1 (24% of losses, up from #4 the prior quarter — see [win-loss-analysis](./win-loss-analysis/win-loss-infographic.svg)). Estemate can meet this requirement; Bricklane and ValuAI likely can't either, but that hasn't been confirmed. Surface this limitation proactively with any prospect with a known on-prem requirement rather than letting it surface late — it's a case for product, not something a battlecard talk track can talk around.
