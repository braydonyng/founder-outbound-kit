---
name: signal-list-builder
description: Build a prospect list from buying signals and from people engaging with LinkedIn or X posts in our category, then research each person and company. Use when the founder says "find people engaging with posts about X", "build a signal list", "who's showing intent", or "scrape the commenters on these posts".
---

# Signal and Engager List Builder

You find people who are raising their hands, then research them well enough that the message can be timely and relevant.

## Inputs

1. `CLAUDE.md`, `ICP.md` (especially §7 Buying signals and §8 Suppression) and `LESSONS.md`
2. Either a list of post URLs, or a topic to search for high-engagement posts
3. The scraping and enrichment tools available (for example Apify, Clay or Deepline)

## Process

### 1. Find the posts
- Search for posts in our category with strong engagement, especially "comment X and I'll send you the guide" posts and launch posts from companies in our space.
- Prefer posts from the last 90 days.
- Show the founder the post list with engagement counts before scraping.

### 2. Preview cost, then scrape
- Estimate rows and cost. **Show the estimate and cap the run before starting.**
- Collect commenters and reactors. Save raw output to disk immediately.
- **Spot-check the counts** against what's visible on the post. If the scraper returned far fewer people than the post shows, it's capping silently. Switch tools.
- Drop the post author's own replies.
- Drop profiles with blank or placeholder headlines. They're usually bots or brand-new fake accounts.

### 3. Dedupe on the person
Dedupe on normalized name plus headline, not on profile URL. The same person can appear with two different URLs (for example once as a commenter and once as a reactor). Keep one row per person, preferring the commenter row, and keep their comment text.

### 4. Score against the ICP
For each person: title fit, company fit (size, industry, region, stack) and engagement type (a substantive comment outranks a reaction). Drop anyone who fails the ICP, works at a competitor, or is suppressed.

### 5. Research the survivors
For each remaining person and company, collect:
- Company headcount, industry, region and tech stack
- What they actually said in their comment
- Signals tied to our problem: hiring for the role we support, launches, funding, leadership changes, tool changes
- A source URL for every signal

A signal only counts if it's tied directly to the problem we solve.

### 6. Write the "why now" line
For each person, one sentence: why this person, why now and why us, built from their signal. This is input for the outbound-writer skill, not the message itself.

## Output

A table saved to `lists/[date]-[name]/` with: name, title, company, domain, profile URL, source post, engagement type, comment text, signals with URLs, ICP score and the why-now line. Then report how many were scraped, removed at each step and why, and how many survived.

## Rules

- Verified data only. No invented signals.
- At most two people per company.
- Never mention the source post's author or a competitor in outreach unless the founder approves it.
