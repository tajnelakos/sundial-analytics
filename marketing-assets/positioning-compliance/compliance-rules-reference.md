# Compliance Rules Reference

A fast-lookup checklist for everything this skill actually checks a draft against. Not a replacement for [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md), [`positioning.md`](../../knowledge-base/positioning.md), or [`competitive-landscape.md`](../../knowledge-base/competitive-landscape.md) — each stays the source of truth, and a rule changes there, not here. This file exists so a reviewer (or the skill itself) doesn't have to re-derive the checkable list from three source docs on every pass.

## How to use this

Run a draft through the four categories in order. Categories 1-2 and 4 produce hard fails; category 3 is judgment-call territory (soft flags). See [`example.md`](./example.md), [`example-pass.md`](./example-pass.md), [`example-soft-flags-only.md`](./example-soft-flags-only.md), and [`example-stale-competitive-claim.md`](./example-stale-competitive-claim.md) for one worked case per outcome.

## 1. Prohibited terms (hard fail) — source: `branding-guideline`

Exact matches and close variants (a term still counts with a different suffix — "seamlessly," "disruption," "unlocking").

`seamless` · `revolutionary` · `cutting-edge` · `game-changing` · `next-generation` · `unlock` (as in "unlock your potential") · `robust` (standalone, no specifics attached) · `powered by advanced AI` / `powered by cutting-edge algorithms` · `disrupt` / `disruptive`

## 2. Banned constructions (hard fail) — source: `branding-guideline`

- **"It's not X, it's Y."** Banned outright, no exceptions — flag any instance regardless of how the specific X/Y is filled in.
- **An AI capability asserted without saying what it actually does or checks.** ("Powered by AI" with no mechanism named.) This audience treats an unexplained AI claim as a yellow flag, not a selling point — see the Head of Credit Risk persona's stated skepticism in [`personas.md`](../../knowledge-base/personas.md).

## 3. Style anti-patterns (soft flag, reviewer's call) — source: `branding-guideline`

These aren't outright banned, so they don't block publish on their own — but they're worth flagging every time, since they're the most common way a draft drifts from voice without tripping a hard rule.

- A scene-setting opener instead of leading with the claim ("In today's fast-changing landscape...").
- A rhetorical question as an opener ("Tired of unexplainable valuations?").
- Manufactured urgency language ("don't get left behind," "the future is now," "last chance").
- An adjective doing the work a number or a defensible qualitative claim should do, where the draft *could* have used one but didn't reach for it.

## 4. Positioning and competitive accuracy (hard fail) — source: `positioning.md`, `competitive-landscape.md`

- **Any claim of superior raw accuracy over every competitor in every scenario.** `positioning.md`'s "What this is not" section rules this out explicitly — the narrative wins on defensibility, not an accuracy race.
- **A quantitative or comparative claim with no traceable source.** "3x faster," "industry-leading accuracy" — if it doesn't map to something in `positioning.md` or a cited, checkable figure, it's a hard fail, not a stylistic nitpick.
- **A named-competitor claim that's gone stale.** Check every claim about what a specific competitor does or doesn't have against `competitive-landscape.md`'s *current* state, not general knowledge or a battlecard version from memory — competitors ship things. As of the September 2026 refresh: ValuAI has a GA audit trail feature (since July 2026), so any claim that ValuAI (or "every other AI-powered vendor," if that's meant to include ValuAI) lacks one is false, not merely unverifiable. See [`example-stale-competitive-claim.md`](./example-stale-competitive-claim.md).
- **A claim that assumes an old competitive threat level.** `competitive-landscape.md`'s Quick Reference table is the current read — e.g. Estemate is 🟠 Medium-High (72.7% win rate against us when faced), not the "boring incumbent, low threat" framing an older draft might still carry.

## Why this list itself can go stale

This reference is a snapshot of three source docs at the time it was written — the same problem [`staleness-detection`](../../knowledge-base/staleness-detection) exists to catch for the knowledge base generally. If `competitive-landscape.md` changes (a competitor ships or drops a feature, a threat level moves), category 4 here should be re-derived from it, not assumed still accurate. [`compliance-trends-analysis.html`](./compliance-trends-analysis.html) shows what happens when this drift isn't caught quickly: a spike in stale-competitive-claim hard fails in the month after ValuAI's GA launch, before `competitive-landscape.md` and the battlecards caught up.
