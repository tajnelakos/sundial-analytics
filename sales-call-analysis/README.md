# Sales Call Analysis

## The problem

Discovery and demo calls generate the most honest competitive and product feedback a company gets — and most of it evaporates the moment the call ends, because nobody has time to relisten and extract it systematically. Call recording tools transcribe; they don't tell you which objection is becoming a pattern.

## The approach

A skill that takes a single call transcript and extracts four things, every time, in the same structure — so that running it across many calls produces comparable output instead of freeform notes:

1. **Objections raised**, verbatim where possible, tagged by type (price, product gap, timing, competitor, internal politics).
2. **Competitor mentions**, with the context they came up in (prospect brought it up unprompted vs. rep asked).
3. **Buying signals**, distinguished from politeness — "that's helpful" is not a buying signal; a question about implementation timeline is.
4. **One coachable moment** for the rep — something they could have handled better, framed constructively, not a performance score.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`gpt.md`](./gpt.md) — ChatGPT custom GPT version
- [`example.md`](./example.md) — run against a discovery call transcript

## Current limitations

Right now this takes one pasted transcript and returns one analysis. Feeding transcripts directly from the call recording tool's API and writing structured output into a shared tracker — so objection/competitor frequency can be tallied automatically across weeks — is next.
