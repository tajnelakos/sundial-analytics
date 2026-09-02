# Sales Deck Builder

## The problem

Reps customize decks for big deals by copy-pasting slides from old decks and hoping the story still holds together. The result is usually a Frankenstein deck: right individual slides, wrong order, no throughline tailored to who's actually in the room.

## The approach

A skill that takes minimal deal context (who's buying, what they care about, what stage the deal is at) and outputs a **slide-by-slide outline**, not full slide copy — headline, purpose, and key point per slide, tailored to the specific buyer persona. This is deliberately an outline generator, not a full deck generator: the outline is fast to sanity-check and hand to design/the rep, while a fully-written deck is harder to critique and more likely to ship something subtly off.

The core judgment call it makes every time: **order and emphasis change based on buyer persona**, even when the underlying product facts don't. A credit-risk buyer and a mortgage-ops buyer should not get the same deck structure just because they're buying the same product.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`custom-gpt/INSTRUCTIONS.md`](./custom-gpt/INSTRUCTIONS.md) — ChatGPT custom GPT version
- [`example/sample-deck-outline.md`](./example/sample-deck-outline.md) — outline generated for a fictional Sundial Analytics deal

## What's simplified from the real version

The production version pulls approved slide inventory from a shared deck library so the outline references actual existing slides where possible, rather than describing slides from scratch. Here it generates a from-scratch outline to keep the example self-contained.
