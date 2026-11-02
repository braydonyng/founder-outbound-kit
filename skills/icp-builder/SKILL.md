---
name: icp-builder
description: Build or tighten the company's ICP from call transcripts, customer data and campaign results, then update ICP.md. Use when the founder says "build my ICP", "tighten the ICP", "what did we learn from these calls", or after a batch of sales conversations or campaign results.
---

# ICP Builder

You turn evidence into an ICP the founder can bet on. Hunches are fine as a starting point. Your job is to replace them with patterns from real conversations and results, and to say plainly which parts are still guesses.

## Inputs

Read, in this order:
1. `CLAUDE.md` and `LESSONS.md`
2. The current `ICP.md`
3. Everything in `calls/` (transcripts and notes)
4. Customer list, closed-lost reasons and campaign results, if present

If there are fewer than five conversations to learn from, say so and recommend network-led conversations before cold outbound.

## Process

1. **Extract every conversation into a row:** company, size, industry, region, tech stack, title, how they found us, the trigger ("why now"), the exact words they used for the problem, the outcome, and why they said no if they did.
2. **Find the patterns.** Group by title, size band, industry, stack and trigger. For each group, count conversations, positive outcomes and objections.
3. **Separate evidence from hope.** Label each ICP attribute `proven` (5+ supporting conversations), `promising` (2-4), or `hunch` (0-1).
4. **Check the market size.** For each promising segment, estimate how many companies fit. If the answer is a few dozen, flag it: that's a hobby, not a market yet.
5. **Pull their language.** List the exact phrases buyers used for the problem. These become message hooks.
6. **Find the exclusions.** Who wasted time, who could never buy, who was the wrong size? Add them to "Who we don't sell to."
7. **Update the title-by-pain matrix** with what each title actually cared about.

## Output

1. A short summary for the founder:
   - What changed in the ICP and why
   - The strongest segment, with evidence counts
   - The biggest open question, and the test that would answer it
2. A proposed diff to `ICP.md`. **Show the diff and wait for the founder's approval before writing it.**
3. Any new lessons for `LESSONS.md`.

## Rules

- Never invent conversations, customers or numbers.
- Don't narrow the ICP to the first few customers without checking market size.
- Keep conviction and evidence separate: the founder can choose to bet on a hunch, but it stays labeled as one.
