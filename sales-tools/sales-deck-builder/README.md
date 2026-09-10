# Sales Deck Builder

## The problem

Reps customize decks for big deals by copy-pasting slides from old decks and hoping the story still holds together. The result is usually a Frankenstein deck: right individual slides, wrong order, no throughline tailored to who's actually in the room.

## The approach

A skill that takes minimal deal context (who's buying, what they care about, what stage the deal is at) and outputs a **slide-by-slide outline**, not full slide copy — headline, purpose, and key point per slide, tailored to the specific buyer persona. This is deliberately an outline generator, not a full deck generator: the outline is fast to sanity-check and hand to design/the rep, while a fully-written deck is harder to critique and more likely to ship something subtly off.

The core judgment call it makes every time: **order and emphasis change based on buyer persona**, even when the underlying product facts don't. A credit-risk buyer and a mortgage-ops buyer should not get the same deck structure just because they're buying the same product.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`gpt.md`](./gpt.md) — ChatGPT custom GPT version
- [`sample-deck-outline.md`](./sample-deck-outline.md) — outline generated for a Sundial Analytics deal

## Current limitations

Right now this generates a from-scratch outline. Pulling approved slide inventory from the shared deck library, so the outline can reference actual existing slides where possible, is next.
