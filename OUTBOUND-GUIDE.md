# Outbound From Zero: A Founder's Guide

The week-by-week version of building outbound before your first sales hire. Times are typical for a seed-stage B2B company doing cold outbound. Your network can make every step faster.

---

## Week 0: Write down what you believe

Before you send anything, fill in `ICP.md`, even if half of it is a guess.

- **Who you think buys:** title, company size, industry, region, tech stack, and the mindset of someone who buys new tools early.
- **Why they'd buy now:** the event or pain that makes this quarter different from last year.
- **Who you won't sell to:** too small, too big, wrong industry, competitors, existing customers and open deals.
- **What you can honestly claim:** proof you can back up. Leave out "best."
- **Your first offer:** a demo, a free trial, an advisory spot, a free audit. Make it easy to say yes to.

If you can't fill a section, that's your first research question, not a reason to wait.

## Weeks 1-2: Network-led sequences

Start with people who already know you.

1. List 50 to 100 people from your network, past customers, investors' portfolios and events who might fit or know someone who does.
2. Write to them yourself. Ask for feedback and introductions, not a purchase.
3. **Run the advisory program.** Offer a few prospects a free 30-day spot as an advisor on an early tool in their space. The only ask is honest feedback. At day 30, make a generous offer (for example, 50% off the first three months on the way to an annual contract).
4. Take notes on every conversation:
   - Who they were and how they found you
   - What triggered the conversation
   - The exact words they used for the problem (this becomes your copy)
   - Why they said no, if they did
5. After each batch of calls, update `ICP.md`. The goalposts will move. Let them.

## Weeks 2-3: Build the machine

While network conversations run, set up cold infrastructure so it's warm by the time you need it.

- **Domains and inboxes:** buy secondary domains, set up SPF, DKIM and DMARC, and warm inboxes for 2 to 3 weeks before real volume. Keep daily sends per inbox low.
- **Sequencer:** one tool for email and one for LinkedIn.
- **CRM:** whatever you'll actually keep updated. Suppression should be pulled from it live before every send, never from an old export.
- **Context repo:** set up Claude Code with the templates in this kit.

## Weeks 3-6: First cold tests

**1. Pick signals tied directly to your problem.**
A signal only counts if it's about the problem you solve. "They're hiring" is noise. "They're hiring for the exact role your product supports" is a signal. Good starting signals:
- Hiring for the role your product supports or replaces
- Launching or announcing something that creates your problem
- Engaging with posts about your category, including competitors' posts
- Funding, expansion or leadership change in the team that buys
- Using, or publicly frustrated with, a tool you replace

**2. Build the list through the gates** (see the `gated-list-builder` skill):
1. Find companies
2. Research and qualify them, then drop everything that fails the ICP
3. Find contacts, at most two per company
4. Find and verify emails, sending only to verified ones
5. Write messages
6. Load sequences

**3. Run the 10-company messaging test.** Write messages for 10 representative accounts, read every one yourself, then send. If they don't land with ten, they won't land with a thousand.

**4. Pilot 100, then scale in chunks.** The pilot proves the whole workflow: sourcing, enrichment, verification, copy and nothing landing at the wrong company.

**5. Write for timing and relevance.** Every message should answer three questions: why this person, why now, why you. Shared hobbies and birthdays get polite replies, not pipeline.

**6. Test several niche sequences at once.** One ICP, one signal and one CTA per sequence. That's the only way to know which one worked.

## Weeks 4-8: First replies and doubling down

- Expect the first ten positive replies to take somewhere between 15 and 45 days of cold outbound, depending on domain warmth, channel and how much of the list came from your network.
- **After 5 to 10 positive replies,** double down on the winning sequence and open a second ICP with a similar problem.
- Track from day one: pipeline by source, conversion at every stage (contacted, replied, meeting, SQL, closed), cycle length and cost per channel.
- Run the sameness audit on every new batch of AI-written copy. If any opener, phrase or CTA shows up in more than about a quarter of the list, rewrite those messages.

## Ongoing: The daily signal loop

Once a motion works, automate the watching:

1. Every morning, an agent scans your target accounts for fresh signals.
2. It scores them and keeps only strong, recent ones.
3. It drops anyone suppressed or already contacted.
4. It finds the right person and the why-now angle.
5. It posts one card per account to Slack: company, what happened, why it matters now, who to contact.
6. A human decides whether to send.

## The ready-to-hire checklist

Make the first sales hire when all of these are true:

- [ ] At least one repeatable source of pipeline with known conversion rates
- [ ] More than a handful of positive replies from a defined ICP, beyond your network
- [ ] ICP, messaging, objection handling and stage definitions written down
- [ ] Your calendar, not the market, is the bottleneck
- [ ] Enough data to set a fair quota

Then hire to scale what works. Your first rep inherits a machine, not a blank page.
