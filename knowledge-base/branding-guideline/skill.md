---
name: brand-voice-rewrite
description: Rewrites a marketing draft to match a documented brand voice, and explains the reasoning behind each significant change rather than returning a silent rewrite. Use when the user has a draft (blog post, email, one-pager, social copy) and wants it brought in line with brand voice.
---

# Brand Voice Rewrite — Sundial Analytics

## Tone

Confident and specific, never hyped. This is a technically skeptical, regulator-adjacent audience (see [`../personas.md`](../personas.md)) — the tone that wins with them is the tone of someone who has nothing to overstate because the real claim is already strong enough.

## Style and editorial standards

- **Lead with the claim, not the setup.** No scene-setting openers ("In today's fast-changing landscape...").
- **Numbers over adjectives.** State the actual figure or comparison if one exists in the source material; if none exists, use a defensible qualitative claim instead of inventing a number.
- **Second person, active voice.** Contractions are fine — formality should come from precision, not stiffness.
- **One idea per paragraph.** This audience skims first, reads second.
- **State limitations plainly when relevant.** A claim that acknowledges what the product doesn't do reads as more credible to this audience than one that doesn't, not less.

## Anti-patterns

- **The "it's not X, it's Y" construction.** Banned outright — it's become a cliché that reads as trying too hard rather than landing a contrast. State the point directly instead.
- **Unexplained AI claims.** Never assert an AI capability without saying what it actually does or checks — this audience treats an unexplained AI claim as a yellow flag, not a selling point (see the Head of Credit Risk persona's explicit skepticism in [`../personas.md`](../personas.md)).
- **Rhetorical questions as openers.** ("Tired of unexplainable valuations?") Reads as filler; open on the actual point instead.
- **Manufactured urgency.** ("Don't get left behind," "the future is now") — doesn't match a buyer who is actively suspicious of hype.

## Prohibited terms

Words to avoid outright — they're either meaningless through overuse or specifically undercut this audience's trust:

`seamless` · `revolutionary` · `cutting-edge` · `game-changing` · `next-generation` · `unlock` (as in "unlock your potential") · `robust` (as a standalone descriptor with no specifics attached) · `powered by advanced AI` / `powered by cutting-edge algorithms` · `disrupt` / `disruptive`

## Approved substitutions

| Instead of | Use |
|---|---|
| "seamless integration" | name the actual integration point ("connects to your existing LOS via API") |
| "powered by advanced AI" | describe what the system actually does or checks |
| "significantly faster" | the actual figure, or "faster than manual review" if no figure is available |
| "revolutionary approach" | state the specific thing that's different, without the adjective |

## Instructions

1. Read the full draft before editing anything — voice fixes made line-by-line without context tend to fix words and miss structural issues (e.g. a weak opening paragraph).
2. Rewrite applying the rules above.
3. For every substantive change (not minor wording), add a brief inline note explaining which rule motivated it. Don't annotate trivial word swaps.
4. If the draft contains a claim that can't be verified from context (a specific stat, a comparison), flag it rather than silently keeping or removing it — the writer needs to confirm it, not the rewrite tool.
5. Preserve the author's structure and intent where it isn't in conflict with a voice rule — this is a voice pass, not a full rewrite from scratch.

## Output format

Return the rewritten draft, followed by a short "Changes and why" list covering only the substantive edits.
