---
name: blog-post-builder
description: Drafts a blog post built around one specific, real point of view or finding — one of positioning.md's points of view, or a real result from competitor-monitoring, win-loss-analysis, staleness-detection, or sales-call-analysis — not a generic "how-to" SEO topic with no real argument behind it. Use when the user wants a blog post and can name (or accept) a specific claim it should make.
---

# Blog Post Builder

## Purpose

Most B2B blog content is generic SEO-bait dressed as thought leadership — a "how-to" post built to rank, not to argue anything. This skill requires a real, specific seed (an actual point of view from `positioning.md`, or an actual finding from this repo's data) before it drafts anything, the same discipline [`personalized-outbound`](../personalized-outbound) applies to a trigger signal and [`case-study-builder`](../case-study-builder) applies to a customer result.

## Instructions

1. **Require a specific seed.** One of [`positioning.md`](../../knowledge-base/positioning.md)'s three "Points of view that ladder to this," or a real, sourced finding from [`competitor-monitoring`](../../sales-tools/competitor-monitoring), [`win-loss-analysis`](../../knowledge-base/win-loss-analysis), [`staleness-detection`](../../knowledge-base/staleness-detection), or [`sales-call-analysis`](../../knowledge-base/sales-call-analysis). If the user just says "write a blog post about X" with no specific claim, offer `positioning.md`'s three POVs as starting options rather than free-associating a generic angle.
2. **Structure:** headline that leads with the claim (no scene-setting opener — `branding-guideline`'s anti-pattern rule already bans this), an intro that states the claim directly, 2-4 body sections each developing one part of the argument with a real, checkable illustration, a conclusion, one CTA.
3. **Any statistic or example used to illustrate the argument must be sourced from this repo's actual data** — the same rule [`positioning-compliance`](../positioning-compliance) and `case-study-builder` already enforce. Don't invent an anecdote because a real one isn't dramatic enough.
4. **Generalize competitive intelligence before it goes public.** A specific finding from a named prospect's sales call (e.g. `sales-call-analysis`) or a specific competitor's name (freely used internally in `competitive-landscape.md`/battlecards) needs to be anonymized for a public blog post — "a recent competitive evaluation" and "a well-funded AI-native entrant," not the account's or competitor's actual name. Internal naming conventions don't transfer to public content automatically; flag any draft that names a real prospect or competitor for legal/marketing-lead review before it publishes.
5. **SEO mechanics apply once the argument is real, not before:** primary keyword in the headline, first paragraph, one subheading, meta description, and URL slug; 2-3 secondary keywords used naturally in body copy; title tag under 60 characters; meta description under 160 characters that compels a click; one H1, descriptive H2/H3s. Write for the persona reading this first — don't keyword-stuff at the expense of the actual point.
6. **Match the target persona's actual content preferences and channels** from [`personas.md`](../../knowledge-base/personas.md) — e.g. the Head of Credit Risk persona reads risk/compliance trade publications and methodology whitepapers, not general SaaS/martech blogs, which should shape tone and depth, not just distribution choice.
7. **Follow [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s full voice rules.**
8. **Run the finished draft through [`positioning-compliance`](../positioning-compliance) before publishing.**

## What to avoid

- Don't write a generic explainer with no real argument in it just because it would rank.
- Don't invent an illustrative anecdote or stat that isn't traceable to this repo's actual data.
- Don't name a specific real (fictional-in-this-repo) prospect account or competitor in the public-facing draft without flagging it for review first.
- Don't optimize for keyword density at the expense of the actual claim.

## Output format

```
## Blog Post — [working title]

**Seed:** [the specific POV or finding this is built around, with internal source]
**Target persona / audience:** [...]
**Primary keyword:** [...] · **Secondary keywords:** [...]

**Title tag:** [...]
**Meta description:** [...]
**URL slug:** [...]

[Headline]

[Body, with H2s]

[CTA]

---
Sourced from: [internal citations for any stat/example used]
Named account or competitor in draft: yes/no — [if yes, flagged for review]
```
