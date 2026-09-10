---
name: brand-voice-rewrite
description: Rewrites a marketing draft to match a documented brand voice, and explains the reasoning behind each significant change rather than returning a silent rewrite. Use when the user has a draft (blog post, email, one-pager, social copy) and wants it brought in line with brand voice.
---

# Brand Voice Rewrite — Sundial Analytics

## Rules

This skill applies [`voice-guide.md`](../voice-guide.md) — tone, style standards, anti-patterns, prohibited terms, and approved substitutions all live there once, not restated here. Read it before running this skill; this file covers only how to apply those rules as a rewrite pass, which is genuinely distinct from the rules themselves.

## Instructions

1. Read the full draft before editing anything — voice fixes made line-by-line without context tend to fix words and miss structural issues (e.g. a weak opening paragraph).
2. Rewrite applying the rules above.
3. For every substantive change (not minor wording), add a brief inline note explaining which rule motivated it. Don't annotate trivial word swaps.
4. If the draft contains a claim that can't be verified from context (a specific stat, a comparison), flag it rather than silently keeping or removing it — the writer needs to confirm it, not the rewrite tool.
5. Preserve the author's structure and intent where it isn't in conflict with a voice rule — this is a voice pass, not a full rewrite from scratch.

## Output format

Return the rewritten draft, followed by a short "Changes and why" list covering only the substantive edits.
