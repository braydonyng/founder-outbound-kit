# [Company] GTM: Instructions for the AI

## Read this first, every time

Before any GTM work (list building, enrichment, messaging, campaign setup, scoring or automation), read `ICP.md` and `LESSONS.md` in this folder.

- `ICP.md` is the source of truth for who we sell to, who we don't, what we claim and how we message.
- If a task conflicts with `ICP.md`, stop and say so. Either the task is wrong or the file needs a deliberate update. Never silently do something different.
- `LESSONS.md` holds rules learned from past mistakes. They are not suggestions.

## Hard rules

1. **Disqualify before you spend.** Every filter that can disqualify a company or contact runs before any paid step.
2. **Two contacts per company, maximum.**
3. **Verified data only.** Never invent a person, email, signal or fact. Every signal needs a source URL.
4. **Wrong-company check.** If a contact's email domain belongs to a different company than the one named in the message, drop the lead.
5. **Suppression is live.** Pull suppression from the CRM right before any send. Never use an old export.
6. **Preview and cap costs.** Before any paid enrichment or scraping run, show the expected cost and cap it. Save paid output to disk immediately.
7. **Test before scale.** New messaging gets a 10-company test that the founder approves. New lists get a 100-row pilot before 1,000.
8. **The founder sends.** Draft and stage everything. Nothing goes to a prospect without the founder's explicit go-ahead.

## Messaging rules

- Lead with timing and relevance: why this person, why now, why us.
- Build the research into the question. Never open with "I noticed" or "I saw."
- One idea and one CTA per message.
- No claims we can't prove. Never say "best."
- Write like a person typing to one person.
- [Add your own banned phrases and tone notes here.]

## Folder map

- `ICP.md`: segments, exclusions, title-by-pain matrix, signals, suppression
- `LESSONS.md`: rules learned from mistakes
- `calls/`: call transcripts and notes
- `messaging/`: best and worst emails, approved templates
- `lists/`: list builds, one folder per run
- `.claude/skills/`: icp-builder, signal-list-builder, gated-list-builder, outbound-writer
