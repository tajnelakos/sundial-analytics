---
name: abm-account-brief
description: Builds a one-page account brief for a named target account by applying the shared ICP, persona, positioning, and competitive-landscape reference docs to that account's specific situation. Use when the user names a target account (with whatever's known about it — firmographics, a buying signal, prior contact) and wants a synthesized brief, not a generic pitch.
---

# ABM Account Brief

## Purpose

Apply the general knowledge base (`icp.md`, `personas.md`, `positioning.md`, `competitive-landscape.md`) to one specific account, so the output is account-specific reasoning, not a restatement of the generic docs with the account's name inserted.

## Instructions

1. **Place the account in the ICP tiering** (`icp.md`) using whatever firmographic detail is given. State the tier and why — this determines expected sales cycle length and how much procurement friction to expect.
2. **Infer the likely buying committee** for this account from the standard committee structure in `icp.md`, adjusted for anything account-specific that's known (e.g. a named hire fills a specific role).
3. **Select the 1-2 most relevant personas** (`personas.md`) based on what's actually known about this account, not all three by default — a brief that tries to speak to every persona equally speaks to none of them well.
4. **Pick the positioning angle** (`positioning.md`) that best matches this account's apparent situation, not the general pitch — if a specific pain or trigger signal is known, lead with the value proposition that maps to it.
5. **Assess competitive risk** using `competitive-landscape.md` — is there a specific competitor likely to already be in this deal (based on account profile, geography, or a known evaluation), and what's the specific play against them for this account.
6. **If a buying signal is provided** (e.g. from `icp-buying-signal-monitor`), the brief must reference it directly as the reason for the account's current priority and timing — don't produce a generic brief that ignores why this account is being looked at right now.
7. **Keep it to one page.** This is meant to be read before a call, not studied — cut detail that doesn't change what the rep would say or do differently.

## What to avoid

- Don't restate the full contents of any one reference doc — pull only what applies to this account.
- Don't invent account-specific facts that weren't given or reasonably inferable from what was given.
- Don't recommend a generic "schedule a demo" close — the next step should be specific to what's known about the account's situation.

## Output format

```
## Account Brief — [Account name]

**Tier:** [tier] — [why]
**Likely committee:** [roles, with names/titles if known]
**Lead persona for this brief:** [persona] — [why this one, this account]
**Positioning angle:** [angle] — [why it fits this account specifically]
**Competitive risk:** [competitor, if any] — [the specific play]
**Why now:** [the buying signal or trigger, if known]
**Recommended next step:** [specific action]
```
