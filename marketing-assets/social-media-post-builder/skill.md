---
name: social-media-post-builder
description: Drafts a social media post (LinkedIn by default, given this ICP) built around one real, cited proof point — a win-loss-analysis stat, a competitor-monitoring finding, a case study result, or a positioning.md point of view — not a generic "check out our product" post. Use when the user wants a social post and can point to (or accept) a specific real finding as its seed.
---

# Social Media Post Builder

## Purpose

A social post with no real finding behind it is just an ad with a hashtag. This skill requires the same real seed [`blog-post-builder`](../blog-post-builder) does, compressed to platform length and mechanics.

## Instructions

1. **Require a specific seed** — a real, sourced stat or finding from this repo's data ([`win-loss-analysis`](../../knowledge-base/win-loss-analysis), [`competitor-monitoring`](../../sales-tools/competitor-monitoring), [`sales-call-analysis`](../../knowledge-base/sales-call-analysis), a [`case-study-builder`](../case-study-builder) result) or one of [`positioning.md`](../../knowledge-base/positioning.md)'s points of view. Reject "write a post about our product" with nothing to hook it to — ask for a finding, or suggest one from recent data.
2. **Structure:** hook (first line states the finding directly — no rhetorical question, per `branding-guideline`'s anti-pattern rule), body (2-4 short lines expanding it), one CTA (comment, click, follow — never stacked).
3. **Default to LinkedIn** given this ICP — [`personas.md`](../../knowledge-base/personas.md) places both the Head of Credit Risk and VP of Mortgage Lending personas there specifically ("risk/compliance-focused LinkedIn groups," "regional banking associations"). Professional but direct tone, paragraph breaks rather than a wall of text, comfortably under LinkedIn's ~1,300-character pre-"see more" cutoff.
4. **Generalize competitive intelligence before it goes public** — the same rule as `blog-post-builder`. A specific competitor or named prospect account used freely internally (`competitive-landscape.md`, battlecards) needs to be anonymized in public social copy, and any draft that does name one gets flagged for legal/marketing-lead review before it posts.
5. **Any stat used must be traceable to this repo's actual data** — don't round a number up to make the hook land harder.
6. **Follow [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules** — social copy is the most likely place a rhetorical-question hook or manufactured urgency creeps back in, so check this explicitly rather than assuming platform norms override brand voice.
7. **Run the finished draft through [`positioning-compliance`](../positioning-compliance) before publishing.**

## What to avoid

- Don't write a generic engagement-bait hook that isn't actually connected to the finding underneath it.
- Don't stack more than one CTA.
- Don't name a specific real competitor or prospect account without flagging it for review.

## Output format

```
## Social Post — [Platform] — [seed finding, one line]

[Hook]

[Body]

[CTA]

#hashtag #hashtag #hashtag

---
Sourced from: [internal citation]
Competitor or account named: yes/no — [if yes, flagged for review]
```
