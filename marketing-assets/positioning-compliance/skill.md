---
name: positioning-compliance
description: Checks a marketing draft against branding-guideline's voice rules (prohibited terms, anti-patterns) and positioning.md (claims that overstate or contradict our actual positioning), returning a pass/fail with specific citations. Never rewrites — flags for the owner to fix. Use as a pre-publish gate, not as an editing tool.
---

# Positioning Compliance Checker

## Purpose

A fast, specific pass/fail check before a piece ships — distinct from a rewrite tool on purpose, so review responsibility stays with the content's actual owner.

## Instructions

1. **Scan for prohibited terms** from [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules — exact matches and close variants (e.g. "seamlessly" counts as "seamless"). Quote the exact sentence each occurs in.
2. **Scan for banned constructions** (e.g. "it's not X, it's Y") — same treatment, quote the instance.
3. **Check every quantitative or comparative claim against what's actually supported** — a claim like "3x faster" needs to be traceable to something in `positioning.md` or flagged as unverifiable, not assumed fine because it sounds plausible.
4. **Check for overclaims against `positioning.md`'s "what this is not" section** — e.g. any claim of superior raw accuracy over all competitors should be flagged, since positioning deliberately avoids that claim.
5. **Do not rewrite anything.** For each finding, cite the exact text and the specific rule/doc section it violates. If the draft is clean, say so plainly — don't invent minor nitpicks to justify the check having run.
6. **Separate hard fails from soft flags.** A prohibited term or an unsupported quantitative claim is a hard fail (blocks publish). A stylistic anti-pattern that isn't explicitly banned but drifts from tone is a soft flag (reviewer's call).

## What to avoid

- Don't suggest replacement copy — that's the brand-voice skill's job, not this one's. Keep the boundary clean so the check stays fast and the fix stays owned by the actual writer.
- Don't pass a draft with a caveat buried in the middle of a paragraph — hard fails go at the top of the output, not softened by a generally positive summary.

## Output format

```
## Compliance Check — [draft name/context]

**Result:** PASS / FAIL

### Hard fails (block publish)
- "[exact quoted text]" — violates: [specific rule/doc reference]

### Soft flags (reviewer's call)
- "[exact quoted text]" — drifts from: [guidance, not a hard rule]

(If none in a category, state "None found.")
```
