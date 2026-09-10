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
