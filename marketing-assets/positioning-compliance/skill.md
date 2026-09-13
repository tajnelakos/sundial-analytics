---
name: positioning-compliance
description: Checks a marketing draft against branding-guideline's voice rules (prohibited terms, anti-patterns), positioning.md (claims that overstate or contradict our actual positioning), and competitive-landscape.md (named-competitor claims that are now outdated), returning a pass/fail with specific citations. Never rewrites — flags for the owner to fix. Use as a pre-publish gate, not as an editing tool.
---

# Positioning Compliance Checker

## Purpose

A fast, specific pass/fail check before a piece ships — distinct from a rewrite tool on purpose, so review responsibility stays with the content's actual owner.

## Instructions

1. **Scan for prohibited terms** from [`branding-guideline`](../../knowledge-base/branding-guideline/skill.md)'s voice rules — exact matches and close variants (e.g. "seamlessly" counts as "seamless"). Quote the exact sentence each occurs in.
2. **Scan for banned constructions** (e.g. "it's not X, it's Y") — same treatment, quote the instance.
3. **Check every quantitative or comparative claim against what's actually supported** — a claim like "3x faster" needs to be traceable to something in `positioning.md` or flagged as unverifiable, not assumed fine because it sounds plausible.
4. **Check for overclaims against `positioning.md`'s "what this is not" section** — e.g. any claim of superior raw accuracy over all competitors should be flagged, since positioning deliberately avoids that claim.
5. **Check every named-competitor claim against [`competitive-landscape.md`](../../knowledge-base/competitive-landscape.md)'s current state, not general knowledge or an older battlecard version.** A competitive claim can be well-supported the day it's written and false a quarter later purely because a competitor shipped something — see [`example-stale-competitive-claim.md`](./example-stale-competitive-claim.md), where "we're the only vendor with a real audit trail" stopped being true the moment ValuAI's feature went GA. This is a hard fail, not a soft flag: an outdated competitive claim is actively wrong, not just unverifiable. See [`compliance-rules-reference.md`](./compliance-rules-reference.md) for the full checklist this and the other checks draw from.
6. **Do not rewrite anything.** For each finding, cite the exact text and the specific rule/doc section it violates. If the draft is clean, say so plainly — don't invent minor nitpicks to justify the check having run.
7. **Separate hard fails from soft flags.** A prohibited term, an unsupported quantitative claim, or an outdated competitive claim is a hard fail (blocks publish). A stylistic anti-pattern that isn't explicitly banned but drifts from tone is a soft flag (reviewer's call).

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
