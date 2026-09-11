---
name: persona-email-sequence
description: Builds a short, persona-specific nurture email sequence from personas.md, where each email advances a different part of that persona's actual decision-making process rather than repeating the same pitch. Use when the user names a persona and a trigger context (e.g. a content download) and wants a multi-email sequence, not a single message.
---

# Persona Email Sequence

## Purpose

Produce a sequence that reads as if it understands how this specific persona actually evaluates a purchase — using their real decision criteria from `personas.md` as the sequence's structure, not just their name in a merge field.

## Instructions

1. **Identify the persona's decision criteria, ranked**, from `personas.md`. This becomes the sequence's backbone — each email should map to advancing one criterion, not repeating the same top-line value prop.
2. **Default to 3 emails** unless the user asks for more — a longer sequence for a mid-funnel nurture usually means each email is thinner, not more thorough.
3. **Email 1** picks up directly from the trigger context (what they downloaded/did) — no generic "thanks for your interest" opener.
4. **Each subsequent email must add new information relevant to a different decision criterion** — never just a softer rephrase of the previous email's point. If there isn't a genuinely new angle for a third email, write two and say why a third would be padding.
5. **Match objection-handling to the persona's actual stated objections** (from `personas.md`) — don't invent generic objections to pre-empt.
6. **Follow [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules** throughout — this especially rules out escalating urgency language in later emails ("last chance," "don't miss out") that would clash with a skeptical, risk-focused persona.
7. **Each email keeps a single, low-friction next step** — don't stack multiple asks in one email.

## What to avoid

- Don't write a sequence that would work equally well for any persona with the name swapped — if it would, the sequence isn't actually using `personas.md`.
- Don't escalate to high-pressure urgency tactics in the final email — inconsistent with a technically skeptical buyer and with the voice guide.

## Output format

```
## Email Sequence — [Persona] — Trigger: [context]

### Email 1 — [subject] — Day 0
[body]
Decision criterion this advances: ...

### Email 2 — [subject] — Day [n]
[body]
Decision criterion this advances: ...

(etc.)
```

## Deep-dive campaign mode

The quick mode above produces sequence content only. Deep-dive mode is for when the user wants a full, run-ready campaign for a persona: more emails, A/B-tested subject lines, and the tracking/analysis/ops material a real send needs — see [`campaign-head-of-credit-risk.md`](./campaign-head-of-credit-risk.md) and [`campaign-vp-mortgage-lending.md`](./campaign-vp-mortgage-lending.md) for two full worked examples.

Use deep-dive mode when the user asks to actually build out / launch / track a sequence for a persona, rather than just draft the email copy.

1. **Extend to 5 emails**, one per decision criterion (most personas in `personas.md` have 3-4 ranked criteria) plus one email built specifically around that persona's named **trust trigger** (a peer reference, a live demo offer, a real implementation timeline) — this is the email most likely to reverse the sequence's natural engagement decay; see the Email 4 pattern in both campaign files.
2. **A/B test subject lines only, not body copy**, across the whole sequence — varying both at once makes it impossible to attribute a performance difference to either one. Frame the two variants as genuinely different techniques (e.g. declarative claim vs. a question naming the buyer's specific fear), not minor word swaps.
3. **Don't assume a winning subject-line style transfers across personas.** [`campaign-performance-analysis.html`](./campaign-performance-analysis.html) found the opposite winner for two different personas from the same two techniques — treat each persona's A/B result as local to that persona.
4. **Produce tracking data** in the shape of [`campaign-metrics.csv`](./campaign-metrics.csv) (per email, per variant: sent, delivered, opened, clicked, replied, meetings booked, unsubscribed) — real or, for a worked example, fictional-but-internally-consistent numbers a reader could recompute the rates from.
5. **Produce an analysis** in the shape of [`campaign-performance-analysis.html`](./campaign-performance-analysis.html) — computed rates and a "what this means for the next sequence" section, not just a repeat of the raw numbers in prose.
6. **Produce reply-handling guidance** in the shape of [`reply-handling-playbook.md`](./reply-handling-playbook.md) — reply types mapped to persona-specific response guidance, grounded in that persona's actual objections and trust triggers/breakers from `personas.md`.
7. **Check deliverability** against [`deliverability-checklist.md`](./deliverability-checklist.md) before treating a new sequence as ready to send — this is generic across personas and only needs to be produced once per repo, not once per campaign.
