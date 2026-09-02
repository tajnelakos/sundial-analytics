---
name: personalized-outbound
description: Drafts one outbound email or LinkedIn message from an account brief, referencing the account's actual trigger signal and positioning angle, following the brand voice guide. Use when the user has an account brief (from abm-account-brief or similar) and wants an outreach draft — not a generic template with the account name inserted.
---

# Personalized Outbound

## Purpose

Turn an account-specific brief into one outbound message that could only have been sent to this account — not a template that happens to mention their name.

## Instructions

1. **Require the trigger/signal to be referenced specifically**, not generically. "I saw you're growing" is not this; "I saw you recently brought on a new Head of Credit Risk and are migrating valuation tooling" is.
2. **Lead with the account's situation, not our product.** The first line should establish that this message is about them specifically — the product enters after that, as the response to their situation, not the subject of the message.
3. **Use the positioning angle already selected in the brief** — don't default to a generic pitch if the brief specifies a particular angle (e.g. defensibility over speed).
4. **One clear, low-friction ask.** Not "let's set up a call to discuss our platform" — something specific and small enough to say yes to (e.g. "worth a 15-minute conversation about how you're thinking about explainability requirements for the new tooling?").
5. **Follow `voice-guide.md`** — no hype language, no banned terms, second person and direct.
6. **Keep it short.** Cold/warm outbound that requires scrolling doesn't get read; aim for under 120 words for email, shorter for LinkedIn.
7. **If the input brief doesn't contain a specific enough trigger to personalize against, say so** rather than producing generic outbound dressed up as personalized — a message with no real hook shouldn't ship under this skill's output.

## What to avoid

- Don't invent a trigger or detail not present in the account brief.
- Don't lead with company boilerplate ("At Sundial, we believe...") — this reads as a template regardless of what follows it.
- Don't ask for a demo in the first message unless the brief indicates the account is already late-stage aware of the product.

## Output format

```
## Outbound Draft — [Account name] — [channel: Email / LinkedIn]

Subject: [if email]

[message body]

---
Personalization used: [the specific trigger/detail this message depends on]
```
