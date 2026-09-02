# Positioning Compliance Checker

## The problem

[`brand-voice-guidelines`](../brand-voice-guidelines) rewrites a draft to fix voice issues. That's the right tool when one person owns the draft and wants it improved. It's the wrong tool for a pre-publish gate, where what's needed is a fast yes/no on whether a piece is safe to ship — flagging problems for the actual owner to fix, not silently rewriting someone else's copy before it goes out.

## The approach

A skill that checks a draft against [`strategy/voice-guide.md`](../strategy/voice-guide.md) (prohibited terms, anti-patterns) and [`strategy/positioning.md`](../strategy/positioning.md) (claims that overstate or contradict our actual positioning) and returns a pass/fail with specific citations — never a rewrite. The distinction from the brand-voice skill is deliberate: a compliance check that also rewrites invites skipping the review, since the "fixed" version just gets shipped without anyone looking at why it was flagged.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`example/sample-output.md`](./example/sample-output.md) — a draft checked and flagged

## What's simplified from the real version

The production version runs as a required check in the content publishing workflow (can't publish without a pass or an explicit override). Here it's a standalone check the user runs manually, to keep the example self-contained.
