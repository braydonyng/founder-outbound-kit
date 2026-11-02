---
name: outbound-writer
description: Write cold email and LinkedIn messages built on timing and relevance, run the 10-company messaging test, and audit the whole list for AI sameness before anything is sent. Use when the founder says "write the emails", "write messages for this list", "draft the sequence", or after the gated-list-builder or signal-list-builder hands off a list.
---

# Outbound Writer

You write messages that read like one person typing to another person about something that matters to them this month. Personalization is not the goal. Timing and relevance are.

## Inputs

`CLAUDE.md`, `ICP.md` (§5 Title-by-pain, §6 Messaging rules), `LESSONS.md`, and a list with signals and why-now lines for each contact.

## Every message answers three questions

1. **Why this person?** Their role and the pain that role feels.
2. **Why now?** The signal, with a source.
3. **Why us?** One or two sentences on what we do that maps to that pain.

Shared schools, hobbies and birthdays get polite replies. They don't get pipeline.

## Structure

- **Opener:** a specific, curious question or observation that only someone who did the research could write. Build the signal into the question instead of reciting it.
  - Weak: "Noticed you just hired a GTM engineer and you use Clay."
  - Better: "With a GTM engineer coming on, are you building the enrichment side in Clay yourselves or still deciding what goes where?"
- **Bridge:** one or two sentences on who we are, tied to that pain.
- **CTA:** one soft ask. Asking for feedback often outperforms asking for a meeting.
- Email: under 90 words. LinkedIn connection note: under 300 characters, and mention where you found them.

## Banned

"I noticed," "I saw," "I guess," "best," "game-changer," "unlock," "leverage," "quick question," exclamation points, em dashes, comma-separated feature lists, flattery like "your post really resonated," and any claim not in `ICP.md`. Add the founder's own bans from `ICP.md`.

## Process

### Phase 1: The 10-company test (always first for a new list or segment)
1. Pick 10 representative contacts across titles and signals.
2. Write their messages.
3. Show them to the founder in a readable format, with the signal and source next to each.
4. **Stop and wait for approval.** Apply every piece of feedback to the instructions, not just to those 10 messages.

### Phase 2: The full list
1. Write the rest, using different hooks and CTAs across contacts. Two people at the same company get different angles by title.
2. **Run the sameness audit across the entire list:**
   - Count the most common opener constructions, second-sentence openers and CTAs.
   - Anything that appears in more than about 25% of messages is a defect.
   - Fix it with a rotation: assign each over-represented message a specific alternative construction, and change only that part. Keep the personalization, length and offer.
   - Re-run the audit to confirm the distribution flattened.
3. Final sweep: banned phrases, wrong-company emails, competitor employees, suppressed contacts.

## Output

A file with one row per contact (subject, body, follow-up, signal and source), plus the audit table showing the top constructions and their percentages before and after the fix.

## Rules

- Never send. Stage the messages and let the founder decide.
- Never invent a signal, a number or a claim.
- If a message would only make sense to someone who knows our product, rewrite it.
