# Lessons: Rules Learned the Hard Way

Every time the AI (or a human) gets something wrong, the fix isn't just correcting the output. Write the rule here so it never happens again. The AI reads this file before any GTM task.

Format for each lesson:

```
## [Short rule]
**What happened:** [the mistake, with numbers if you have them]
**Rule:** [what to do from now on]
**Applies to:** [list building / enrichment / messaging / sending / reporting]
```

---

## Starter lessons (from my own builds)

## Disqualify before you spend
**What happened:** Paid enrichment ran on a full list before the ICP filters, and a large share of the paid emails were thrown away immediately.
**Rule:** Run every filter that can disqualify a company or contact before any paid step.
**Applies to:** list building, enrichment

## Count phrases across the whole list
**What happened:** Several AI writers each varied their own batches, but across the full list nearly two-thirds of messages opened the same way.
**Rule:** After merging batches, count opener, phrase and CTA frequency across the whole list. Anything over about 25% gets rewritten.
**Applies to:** messaging

## Check what your scraper is actually returning
**What happened:** A post-engagement scraper silently capped at about 100 comments per post. A different tool returned about eight times as many people.
**Rule:** Spot-check scraper output against what's visible on the post before trusting the counts.
**Applies to:** list building

## Dedupe on the person, not the URL
**What happened:** People who both commented and reacted came back with two different profile URLs and were nearly messaged twice by two senders.
**Rule:** Dedupe on normalized name plus headline or company, then pick one row per person.
**Applies to:** list building, sending

## Only signals about our problem count
**What happened:** A broad signal (general hiring in a nearby function) looked relevant and produced almost no interest.
**Rule:** Keep only signals tied directly to the problem we solve.
**Applies to:** signals, scoring

## Drop job-changers
**What happened:** Enrichment returned work emails at a contact's new company while the message referenced their old one.
**Rule:** If the email domain doesn't match the company in the message, drop the lead.
**Applies to:** enrichment, sending
