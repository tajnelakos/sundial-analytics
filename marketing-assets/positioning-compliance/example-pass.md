# Sample output — a clean pass

Shows the checker when a draft actually clears every rule — the check shouldn't invent minor nitpicks just to look like it did something. Contrast with [`example.md`](./example.md) (hard fails) and [`example-soft-flags-only.md`](./example-soft-flags-only.md) (passes, but not nitpick-free).

---

## Input

> You can see every comparable used in a Sundial valuation, and how each one was weighted — not just a confidence score. That's the difference when an examiner asks how a number was reached. Our benchmarking methodology is documented and available to technical evaluators on request, so your team can scrutinize it before relying on it in production.

## Output

```
## Compliance Check — Draft, untitled (audit trail feature paragraph)

**Result:** PASS

### Hard fails (block publish)
- None found.

### Soft flags (reviewer's call)
- None found.
```

Notes on why this passes clean, not just "why it wasn't flagged":

- Leads with the claim ("you can see every comparable...") — no scene-setting opener.
- The AI/methodology claim names what's actually checkable (comparables, weighting, a documented methodology) rather than asserting a capability with no mechanism — this is the opposite of the banned "powered by advanced AI" pattern in [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md).
- No quantitative claim is made at all, so there's nothing to trace or flag as unverifiable — "documented and available to technical evaluators on request" is the defensible qualitative claim [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md) recommends reaching for when no hard figure exists, used correctly rather than as a workaround.
- No competitor named, so no risk of a stale competitive claim.
- No accuracy-superiority claim — the draft never reaches for "best" or "most accurate," consistent with [`positioning.md`](../../knowledge-base/positioning.md)'s "what this is not."
