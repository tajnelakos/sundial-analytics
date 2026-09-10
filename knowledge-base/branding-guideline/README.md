# Branding Guideline

## The problem

Brand guidelines are usually a PDF nobody rereads after onboarding — and most of them only cover half the picture: voice rules with no visual identity, or a logo file with no naming conventions, split across whatever tool made them easiest to produce at the time. In practice, brand consistency breaks down in the small, high-volume stuff — a support-team blog post, a sales one-pager written under deadline, a button component built without checking the type scale — not the flagship campaign that gets three rounds of review.

## The approach

Two things live here, deliberately not merged: a **skill** that applies the voice rules as an active rewrite pass (below), and the **fuller brand system** those rules are one part of — mission, values, tone by channel, logo, color, typography, and naming conventions, with the actual visual assets alongside it, not described in prose only.

## Files — the rewrite skill

- [`skill.md`](./skill.md) — the Claude Skill definition, including the voice rules it applies (tone, style standards, anti-patterns, prohibited terms, substitutions)
- [`before-after.md`](./before-after.md) — a sample rewrite for [Sundial Analytics](../knowledge-base.md), with the reasoning shown

## Files — the full brand system

- [`brand-guidelines.md`](./brand-guidelines.md) — mission, vision, brand values, tone-by-channel, logo rules, full color palette (HEX/RGB/CMYK), typography, UI/UX visual styles, naming conventions, image and icon style
- [`logo.svg`](./logo.svg) — primary logo, for light backgrounds
- [`logo-reversed.svg`](./logo-reversed.svg) — white version, for dark backgrounds
- [`logo-mark.svg`](./logo-mark.svg) — icon alone
- [`logo-usage.svg`](./logo-usage.svg) — clear space, minimum size, and misuse reference sheet
- [`color-palette.svg`](./color-palette.svg) — the palette swatch reference

## Current limitations

The rule set in `skill.md` is condensed to what generalizes across content types; a fuller internal terminology doc and a running library of examples pulled from top-performing published content are next to fold in. The logo files are hand-authored SVG with system-font fallbacks rather than production-ready files with text converted to outlines — the right next step before these ever left this repo for real print or app-icon use.
