# Positioning Compliance Checker

## The problem

[`branding-guideline`](../../knowledge-base/branding-guideline) rewrites a draft to fix voice issues. That's the right tool when one person owns the draft and wants it improved. It's the wrong tool for a pre-publish gate, where what's needed is a fast yes/no on whether a piece is safe to ship — flagging problems for the actual owner to fix, not silently rewriting someone else's copy before it goes out.

## The approach

A skill that checks a draft against [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules (prohibited terms, anti-patterns), [`positioning.md`](../../knowledge-base/positioning.md) (claims that overstate or contradict our actual positioning), and [`competitive-landscape.md`](../../knowledge-base/competitive-landscape.md) (named-competitor claims that have gone stale since they were written) — and returns a pass/fail with specific citations, never a rewrite. The distinction from the brand-voice skill is deliberate: a compliance check that also rewrites invites skipping the review, since the "fixed" version just gets shipped without anyone looking at why it was flagged.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`compliance-rules-reference.md`](./compliance-rules-reference.md) — a fast-lookup checklist consolidating the checkable rules from all three source docs, so a reviewer isn't re-deriving them on every pass

### Worked examples — one per outcome

- [`example.md`](./example.md) — a draft with hard fails (prohibited term, unverifiable claim, positioning overclaim)
- [`example-pass.md`](./example-pass.md) — a clean pass, nothing found in either category
- [`example-soft-flags-only.md`](./example-soft-flags-only.md) — passes (no hard fails), but a real stylistic anti-pattern still gets named
- [`example-stale-competitive-claim.md`](./example-stale-competitive-claim.md) — a claim that was accurate when written and is false now, because a named competitor (ValuAI) shipped the feature the claim said they lacked

### Tracked data

- [`compliance-check-log.csv`](./compliance-check-log.csv) — 20 logged checks, Jul–Sep 2026, across 8 content types
- [`compliance-trends-analysis.html`](./compliance-trends-analysis.html) — the computed analysis ([view live ↗](https://tajnelakos.github.io/sundial-analytics/marketing-assets/positioning-compliance/compliance-trends-analysis.html)). Headline finding: pass rate collapsed to 12.5% the month after ValuAI's audit trail feature went GA (writers were still using the "we're the only one" claim), then recovered to 71.4% right after the [`staleness-detection`](../../knowledge-base/staleness-detection) sweep corrected the source docs — direct evidence that this check and that sweep are catching the same underlying drift from two different angles.

## Current limitations

Right now this is a standalone check run manually, and the tracked log is a one-time fictional snapshot rather than a live feed from an actual content-review queue — the same limitation [`win-loss-analysis`](../../knowledge-base/win-loss-analysis) has with its CRM export. Wiring this in as a required check in the content publishing workflow (can't publish without a pass or an explicit override), and specifically as a required step in the [`battlecard`](../../sales-tools/battlecard) refresh cycle given how the trends data shows battlecards behaving, is next.
