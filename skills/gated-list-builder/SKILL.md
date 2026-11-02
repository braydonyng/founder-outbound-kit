---
name: gated-list-builder
description: Build a cold outbound list through fixed gates so disqualified companies and contacts are removed before any money is spent on enrichment. Use when the founder says "build a list", "find companies like X", "source accounts for this segment", or before any paid enrichment run.
---

# Gated List Builder

You build lists in a fixed order. Every filter that can disqualify a company or a person runs before the step that costs money. Don't reorder the stages and don't skip a gate.

## Inputs

`CLAUDE.md`, `ICP.md`, `LESSONS.md`, the target segment, and the enrichment tools available.

## The six stages

### 1. Find companies
Source the account universe for the segment from company databases, curated lists, directories or signal lists. Dedupe on domain. Prefer free sources first.

### 2. Research and qualify, then GATE
For each company confirm: what they actually do, headcount, region, and the ICP-specific attributes. **Drop every company that fails here**: wrong industry, outside the size band, acquired or defunct, competitor, suppressed, current customer or open deal. Report the drop counts by reason.

### 3. Find contacts, then GATE
Only at surviving companies. Pick titles from the title-by-pain matrix. Under 50 employees, the founder is a fine target. At 50 or more, pick the functional owner. **Cap at two people per company before any per-contact spend.**

### 4. Find and verify emails
Only for the capped, qualified contacts. Verify every address and keep only verified ones. Run the **wrong-company check**: if the email domain belongs to a different company than the one the message will reference, drop the lead.

### 5. Write messages
Hand off to the outbound-writer skill. A new list or segment always starts with the 10-company test.

### 6. Load sequences
Only after the founder approves the test. One sequence per niche: one ICP, one signal and one CTA.

## Cost control

- Before every paid step, show the founder: rows, cost per row, total, and the cap. Wait for approval.
- Run new lists as a 100-row pilot through all six stages before running 1,000.
- Save paid output to disk immediately after each call. Never re-buy data you already paid for.

## Output

A folder in `lists/[date]-[segment]/` with one file per stage, plus a summary: counts in and out at each stage, drop reasons, total cost and cost per final lead.
