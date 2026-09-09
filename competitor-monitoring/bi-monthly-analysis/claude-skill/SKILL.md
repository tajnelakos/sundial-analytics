---
name: bi-monthly-competitive-intelligence
description: Produces a recurring bi-monthly competitive intelligence report tracking named competitors' public developments, partnerships, and positioning shifts, each claim dated and sourced, in a fixed structure so reports are comparable period over period. Use for the deeper periodic report — distinct from competitor-monitoring's weekly brief, which is faster and lower-ceremony.
---

# Bi-Monthly Competitive Intelligence Report

## Purpose

Produce a structured, sourced, comparable-over-time report of what named competitors are publicly doing — company developments, partnerships, and positioning shifts — for a fixed two-month period. Unlike the weekly brief, this report is built to hold up as a reference document: every claim about a competitor is dated, sourced, and neutral.

## Scope and period

- Track the competitors defined in `competitive-landscape.md`. Region-agnostic by default — track globally unless a specific deal or segment calls for a regional cut.
- Cover a fixed two-month window (e.g. July–August). State the window explicitly at the top of the report.
- If nothing verifiable is found for a competitor in the period, write "No significant developments found in this period" rather than reaching back to older news or padding with unrelated content.

## Instructions

1. **Verify before writing.** Every bullet describing an actual development gets a source. Do not present something as a development if it can't be sourced.
2. **Keep the vendor-tracking sections neutral and descriptive.** No comparative language ("better than," "weaker than"), no impact/threat/opportunity language, and don't mention Sundial Analytics by name inside these sections. State competitors' own claimed figures as their claims, not as verified fact.
3. **Structure each competitor identically**, in this order:
   - **Recent Developments** — funding, acquisitions, expansion, product/feature launches, notable hires, governance changes. Not general content marketing or thought-leadership posts unless they announce an actual company-level change.
   - **Partnerships and Ecosystem Moves** — integrations, data partnerships, distribution deals.
   - **Messaging and Positioning** — only include this section if messaging has visibly changed from the start of the current half-year. Don't restate stable, unchanged positioning just to fill the section.
4. **Source every developmental claim** with a short label, not a raw URL (e.g. "Company press release," "Official blog," "Industry news"). If two sources support one claim, include both.
5. **After the neutral per-competitor sections, add two sections the real-world version of this report deliberately excludes** (see note below):
   - **Market Patterns** — cross-competitor observations only when a genuine pattern spans multiple competitors (e.g. two competitors shifting messaging toward the same claim in the same period). Skip this section entirely if nothing crosses competitor lines this period — a single-competitor observation belongs in that competitor's own section, not here.
   - **Strategic Signals for Sundial Analytics** — the implications, tied to specific developments above, including what to do next (e.g. flag a stale battlecard claim, revisit a positioning angle). This is the one place recommendations belong.
6. **No conclusion, no forced recommendation, no filler.** If a section has nothing, say so plainly rather than manufacturing content.

## A deliberate departure from the real-world version

A real competitive intelligence report circulated inside a company is usually kept strictly neutral — descriptive only, no strategic framing — so the intelligence function stays trusted as an unbiased source and doesn't get read as one analyst's opinion dressed up as fact. This version intentionally adds the Market Patterns and Strategic Signals sections on top of that neutral base, to demonstrate the synthesis step a product marketer would do with the report afterward. In production, that synthesis would usually happen in a separate follow-up, not inside the report of record itself.

## Output format

Two deliverables: the structured write-up (Markdown, for the record) and, given the report's actual audience, a designed one-page HTML version meant to be opened and skimmed rather than read as a document — see [`example/`](../example) for both.
