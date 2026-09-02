# Persona Email Sequence

## The problem

Nurture sequences are usually written once for "the buyer" in general, then sent to everyone regardless of role — so a credit-risk-focused email lands on an operations buyer who doesn't care about audit trails, and vice versa. The fix isn't more emails, it's sequences actually built around what a specific persona's decision-making process looks like, using [`personas.md`](../personas.md) instead of a single generic buyer.

This is distinct from [`personalized-outbound`](../personalized-outbound): that skill drafts one 1:1 message for a specific named account with a specific trigger. This one builds a reusable multi-email sequence for a persona segment — for marketing automation, not 1:1 sales outreach.

## The approach

A skill that takes a persona (from `personas.md`) and a starting context (e.g. "downloaded the audit-trail whitepaper") and produces a short sequence — each email escalating naturally through that persona's actual decision criteria, not just increasing urgency. The sequence explicitly avoids restating the same value proposition three ways; each email should earn its place by advancing a different part of that persona's evaluation.

## Files

- [`claude-skill/SKILL.md`](./claude-skill/SKILL.md) — the Claude Skill definition
- [`example/sample-output.md`](./example/sample-output.md) — a 3-email sequence for the Head of Credit Risk persona

## What's simplified from the real version

The production version is tied into the marketing automation platform's trigger/branch logic (e.g. stop the sequence if the contact books a call). Here it outputs the email content only, to keep the example self-contained.
