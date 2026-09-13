# Sample output — passes, but not nitpick-free

The middle case between [`example.md`](./example.md) (hard fails) and [`example-pass.md`](./example-pass.md) (nothing found at all): a draft with zero hard fails, so it's a PASS, but a real stylistic anti-pattern still gets named rather than waved through because "it passed."

---

## Input

> Wondering how your team would explain an automated valuation to an examiner? Sundial's audit trail shows the specific comparables used and their weighting for every valuation, so your team can walk through the reasoning afterward instead of just citing a confidence score. Our benchmarking methodology is documented and available for technical evaluators to review.

## Output

```
## Compliance Check — Draft, untitled (audit trail feature paragraph, v2)

**Result:** PASS

### Hard fails (block publish)
- None found.

### Soft flags (reviewer's call)
- "Wondering how your team would explain an automated valuation to an examiner?" — drifts from: branding-guideline's anti-pattern against rhetorical questions as openers ("reads as filler; open on the actual point instead"). Not a banned phrase outright — everything after this opening line is clean — so this doesn't block publish, but the writer should know it's there.
```

Why this is a PASS and not a FAIL: the rhetorical-question opener is listed in `branding-guideline` as an anti-pattern to avoid, but it isn't in the explicitly "banned outright" category the way the "it's not X, it's Y" construction is — see [`compliance-rules-reference.md`](./compliance-rules-reference.md)'s categories 2 and 3 for the distinction this check is drawing. Everything else in the draft (the methodology claim, the lack of any invented figure, no competitor named) matches [`example-pass.md`](./example-pass.md)'s clean version — this example exists specifically to show that "PASS" and "nothing worth mentioning" aren't the same result.
