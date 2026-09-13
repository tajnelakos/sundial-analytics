# Case Study Builder

## The problem

Case studies are usually the most fabricated piece of B2B content in the building — assembled from a rep's memory of how a deal went, a testimonial quote nobody actually said out loud, and a result quietly rounded up because the real number wasn't impressive enough. The fix isn't a better case-study template; it's requiring the same real-source discipline this repo's other tools already apply ([`personalized-outbound`](../personalized-outbound), [`positioning-compliance`](../positioning-compliance)), so a case study says only what its actual CRM record and call transcript support.

## The approach

Takes a closed-won account's real CRM record and/or call transcript — not a rep's plausible-sounding summary of how the deal went — and produces a Challenge/Solution/Results case study, citing which specific artifact backs each claim. Explicitly separates "this happened, and we have proof" from "this would be a nice claim to make," including the often-skipped step of flagging that a quote pulled from a sales call transcript needs the customer's own consent before it can run as a public testimonial.

## Files

- [`skill.md`](./skill.md) — the Claude Skill definition
- [`example.md`](./example.md) — Nordkredit, built from the actual win-loss CRM record and sales-call-analysis transcript already in this repo

## Why this account specifically

Nordkredit isn't a fresh example invented for this folder — it's the same account [`icp-buying-signal-monitor`](../../sales-tools/icp-buying-signal-monitor) flagged as a cold signal, [`abm-account-brief`](../../sales-tools/abm-account-brief) briefed, and [`personalized-outbound`](../personalized-outbound) drafted outreach to. [`sales-call-analysis/call-01-nordkredit.md`](../../knowledge-base/sales-call-analysis/call-01-nordkredit.md) is the resulting discovery call, and [`win-loss-analysis/win-loss-crm-export.csv`](../../knowledge-base/win-loss-analysis/win-loss-crm-export.csv) (OPP-1001) shows it closed won. This folder is that pipeline's actual ending, not a new, disconnected example.

## Current limitations

The customer sign-off this skill flags as a prerequisite is a real business step it can identify the need for but can't execute — getting Nordkredit's actual permission to quote Lena Virtanen and use the company's name publicly is a human process outside this repo's scope.
