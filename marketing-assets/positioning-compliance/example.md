# Sample output

A fictional draft going through the compliance checker — flags rather than fixes.

---

## Input

> In today's fast-changing real estate lending landscape, financial institutions are increasingly turning to advanced technology solutions to streamline their valuation processes. Our platform is powered by cutting-edge AI algorithms that deliver significantly faster results than traditional methods, helping users eliminate lending risk and transform their credit operations. Users receive a valuation output within a short timeframe, backed by industry-leading accuracy.

## Output

```
## Compliance Check — Draft, untitled (valuation product intro paragraph)

**Result:** FAIL

### Hard fails (block publish)
- "cutting-edge AI algorithms" — violates: branding-guideline prohibited terms list ("cutting-edge," and this phrasing matches the explicitly banned "powered by advanced AI" / "powered by cutting-edge algorithms" pattern)
- "significantly faster" — violates: branding-guideline style rule (numbers over adjectives) — no figure or comparison is given to support this, and none is traceable to positioning.md
- "helping users eliminate lending risk" — violates: positioning.md — this is a stronger claim than our positioning supports; the doc explicitly notes we reduce manual review time and provide a documented basis, not that we eliminate lending risk
- "industry-leading accuracy" — violates: positioning.md "what this is not" — positioning deliberately avoids an unqualified accuracy superiority claim; this is exactly the claim it warns against

### Soft flags (reviewer's call)
- "In today's fast-changing real estate lending landscape..." — drifts from: branding-guideline style guidance to lead with the claim, not a scene-setting opener. Not a banned phrase outright, but reads as filler.
```
