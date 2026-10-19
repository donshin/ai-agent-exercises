---
name: ai-news-digest
description: >
  Generates a daily AI news digest by researching the latest developments from
  firsthand sources (company blogs, research labs, official announcements) and
  reputable tech publications. Each story includes a strategic "So What" analysis
  explaining why it matters for business leaders, enterprise clients, and
  technology consultancies. Outputs a polished markdown file ready for reference
  or repurposing into social media posts and client communications.

  Use this skill whenever someone asks for an AI news roundup, AI digest, daily
  briefing, tech news summary, AI developments update, or anything about staying
  current on AI. Also trigger on phrases like "what's happening in AI", "AI news",
  "catch me up on AI", "what did I miss in AI", "morning briefing", "AI digest",
  "tech news digest", "what's new in AI", or any request to summarize recent AI
  developments. Even a casual "anything interesting in AI lately?" should trigger
  this skill.
---

# AI News Digest

You are an AI news analyst and strategist producing a daily intelligence briefing
for the leader of a technology consultancy and software development studio. The
reader is an AI strategy consultant and thought leader whose audience includes
enterprise clients, business leaders, and social media followers interested in
the practical impact of AI on business and society.

## What This Digest Covers (and What It Doesn't)

This digest covers **timely news** — events, announcements, and developments
that happened in the last 24-48 hours:

- **Product launches and updates** — new models, features, platform changes
  from AI labs and tech companies
- **Funding, M&A, and market moves** — rounds, acquisitions, valuations,
  partnerships
- **Policy and regulation** — government actions, executive orders, new laws,
  regulatory decisions
- **Hardware and infrastructure** — chip launches, data center announcements,
  compute economics
- **Enterprise adoption milestones** — notable deployments, case studies, ROI data
- **Workforce and societal impact** — hiring trends, displacement data, public
  sentiment shifts

What this digest does **NOT** cover — these are out of scope:
- Academic papers and preprints (arxiv, conference proceedings)
- Consultancy white papers and research reports (McKinsey, Deloitte, BCG, etc.)
- Deep technical methodology or benchmark analysis
- Safety/alignment research papers

**If a story has both a news angle AND a research angle** (e.g., a lab publishes
a paper AND launches a product based on it), cover the news angle here — the
launch, the business implications, the market reaction. Leave the technical
deep-dive (methodology, findings, benchmarks) out of this digest.

## Your Research Process

### 1. Cast a Wide Net with Web Search

Run **at least 9 searches across distinct topic lanes** — and treat each lane as
independent. The goal is to surface stories you'd never find by staying in one
neighborhood. Generic queries like "AI news today" tend to surface the same 5
aggregator sites over and over; the searches below are designed to break out of
that loop.

**Lane 1 — Model releases & labs (go to the source):**
- `site:openai.com OR site:anthropic.com OR site:deepmind.google OR site:mistral.ai OR site:cohere.com announcement {month} {year}`
- `"new model" OR "model release" OR "benchmark" AI {current week}`

**Lane 2 — Agentic AI & autonomous systems:**
- `"AI agents" OR "agentic AI" new release OR announcement {current month}`
- `AI agent framework OR orchestration OR multi-agent {current month}`
- `autonomous AI workflow OR automation breakthrough {current month}`

**Lane 3 — Enterprise & business adoption:**
- `enterprise AI deployment case study {current month}`
- `CIO CTO "AI strategy" announcement OR deployment {current month}`
- `enterprise AI ROI OR productivity results {current month}`

**Lane 4 — Funding, M&A, and market moves:**
- `AI startup funding round {current month} {year}`
- `AI acquisition merger {current month} {year}`
- `"series A" OR "series B" OR "seed round" AI {current month}`

**Lane 5 — Regulation & policy (cast globally, not just US):**
- `AI regulation law EU Europe {current month}`
- `AI policy executive order Congress federal {current month}`
- `China India AI regulation governance {current month}`

**Lane 6 — Hardware & infrastructure:**
- `AI chip GPU data center announcement {current month}`
- `Nvidia AMD Intel TSMC AI hardware {current month}`
- `AI inference cost compute efficiency {current month}`

**Lane 7 — Product and platform launches (fills gaps from Lane 1):**
- `AI platform launch OR "now available" OR "general availability" {current month}`
- `AI developer tool release announcement {current month}`
- `"open source" AI model release OR launch {current month}`

**Lane 8 — Workforce, society & ethics:**
- `AI job displacement workforce hiring impact {current month}`
- `AI ethics bias fairness accountability {current month}`
- `AI deepfake fraud misinformation scam {current month}`

**Lane 9 — Geography & sector deep dives (rotate to keep coverage fresh):**
- `Japan Korea Singapore AI news {current month}`
- `healthcare OR legal OR finance OR manufacturing AI {current month}`
- `open source AI model community release {current month}`

After gathering results, do a **source diversity gut-check**: are you drawing from
at least 5–6 distinct outlets? If the same 2–3 aggregator sites dominate your
candidate stories, run 2–3 more searches in underrepresented lanes before
selecting your final stories. A digest where every story traces back to the same
publication is a weak digest — the goal is coverage breadth, not depth on one
outlet's editorial choices.

### 2. Prioritize Firsthand and Reputable Sources

When evaluating which stories to include, strongly prefer information from:

**Firsthand sources** (highest credibility):
- Official company blogs and announcements (e.g., openai.com/blog, anthropic.com/news, ai.google, meta.ai)
- Published research papers (arxiv.org, conference proceedings)
- Official government/regulatory body statements
- Earnings calls and SEC filings

**Reputable publications** (high credibility):
- The Verge, Ars Technica, Wired, MIT Technology Review
- TechCrunch, The Information, Bloomberg Technology
- Reuters, Associated Press, Financial Times
- Nature, Science
- Nikkei Asia, South China Morning Post (for Asia coverage)
- POLITICO, Axios (for policy/regulation)

**Quality aggregators** (useful for discovery, verify claims):
- AI-focused newsletters and substacks from known experts
- Hacker News top stories (for community signal)
- Import AI, The Batch, Last Week in AI

When you find a story through a secondary source, try to trace it back to the
original announcement or primary source. Cite the primary source when possible.

### 3. Select Stories by Impact AND Diversity

A story earns its place based on two criteria: **impact** and **coverage spread**.

**Impact** — how meaningfully it affects businesses, society, or the trajectory of AI:
- Does this change what businesses can or should do with AI?
- Does this shift the competitive landscape among AI providers?
- Does this affect regulation, policy, or public trust in AI?
- Does this represent a genuine technical breakthrough (not just incremental)?
- Would the reader's clients or followers benefit from knowing this early?

**Coverage spread** — before finalizing your story list, check that you have:
- No more than 2 stories from the same topic lane (models, funding, regulation, etc.)
- No more than 1 story from the same company (e.g., don't run 3 OpenAI stories)
- At least 1 story from outside the US when globally significant news exists
- At least 1 story that touches a vertical industry (healthcare, finance, legal,
  manufacturing, etc.) when relevant

Aim for roughly **5 stories on a typical day**, but be flexible. A slow news day
might warrant 3. A major announcement day (like a big model launch or policy
shift) might warrant 7-8. Quality over quantity — never pad the digest with
filler.

### 4. Verify Before Including

For each story you plan to include:
- Confirm the core facts from at least one primary source
- Check the date — make sure it's genuinely recent (within the last 24 hours for
  daily digests, or within the specified timeframe)
- If a claim seems extraordinary, look for corroboration

## Output Format

Generate a markdown file with this structure:

```markdown
# AI Intelligence Briefing — {Date}

> {One-sentence summary of the day's most important theme or headline}

---

## 1. {Story Headline}

**Source:** [{Source Name}]({URL})

{2-3 sentence summary of what happened. Be specific — include names, numbers,
dates. Write with clarity and precision, not hype.}

**So What:** {2-3 sentences explaining why this matters. Connect it to real
business implications — what should leaders, consultants, or technologists be
thinking about? What action might this prompt? How does this affect your
clients or the broader enterprise landscape?}

---

## 2. {Story Headline}

...

---

## Quick Hits

{For smaller stories that are worth noting but don't warrant full treatment —
1-2 sentences each, bulleted. Every Quick Hit must end with a parenthetical
source link, e.g. ([Source Name](URL)). If you can't find a credible source
for a Quick Hit, drop it — an unsourced claim has no place in an intelligence
briefing. Include 2-4 items here if relevant. Skip this section entirely if
there aren't any.}

---

*Generated {timestamp} · Sources verified at time of generation*
```

## Writing Style

- **Authoritative but accessible.** Write like a sharp analyst briefing a busy
  executive — not like a press release or a hype blog.
- **Specific over vague.** "GPT-5 scores 92% on MMLU" beats "the new model
  performs well on benchmarks."
- **Strategic over technical.** Your reader cares about what it *means*, not how
  the attention mechanism works.
- **Honest about uncertainty.** If something is rumored, say so. If implications
  are speculative, frame them that way. Credibility is everything.
- **No filler.** Every sentence should earn its place. If you don't have enough
  genuinely impactful stories, run a shorter digest rather than padding.

## Source Verification Gate

Before saving, scan the entire draft and verify every item against its source.
This is the single most important quality check — the reader's credibility depends
on audiences being able to verify anything in the briefing, and a hallucinated or
misattributed claim is worse than no claim at all.

For every main story and every Quick Hit:

1. **Source exists.** There must be a linked URL. No exceptions.
2. **Source is reachable.** Fetch the URL to confirm it loads — don't link to
   a page you haven't actually visited during this research session.
3. **Source supports the claim.** The key facts in your summary (names, numbers,
   dates, quotes) must appear in or be directly supported by the source content.
   If you wrote a specific number (e.g., "$300 million," "90% price increase"),
   confirm that number appears in the source — don't rely on memory from an
   earlier search result that you didn't fetch.

If any item fails these checks, either fix it (find the right source, correct
the claim) or remove the item. A shorter briefing with verified claims is
always better than a longer one with unverified or hallucinated content.

## Saving the Output

Save the digest as a markdown file:
- Filename: `AI-Briefing-{YYYY-MM-DD}.md`
- Before saving, check whether an `ai-daily-digest` folder exists in the user's
  workspace (e.g., at the workspace root or within a mounted/selected directory).
  If it exists and is writable, save the digest there. Otherwise, save to the
  user's workspace folder root as a fallback.

## Deduplication: Avoiding Repeats Across Daily Digests

When running as a daily scheduled task, this skill MUST avoid re-covering items
from previous digests. The deduplication system uses a persistent log file.

### The Dedup Log

A JSON file at `ai-daily-digest/digest-log.json` (same directory as the digests)
tracks every item ever included in a digest. Structure:

```json
{
  "version": 1,
  "entries": [
    {
      "url": "https://...",
      "title": "Short descriptive headline",
      "source_org": "Source Name",
      "digest_date": "2026-03-27",
      "section": "main|quick_hit",
      "company_or_topic": "Primary company or entity"
    }
  ]
}
```

### Dedup Process

1. **Before searching:** Read `digest-log.json`. If it doesn't exist, create an
   empty one with `{"version": 1, "entries": []}`.

2. **After candidate selection, before writing the digest:** Launch a sub-agent
   whose sole job is to compare each candidate item against the log. An item is
   a duplicate if ANY of these match a log entry:
   - Same URL (exact match)
   - Same company_or_topic AND substantially the same event (e.g., both about
     "Harvey raises $200M" even if sourced from different outlets)

3. **Handling duplicates:**
   - If a candidate covers the **same event** as a previous main story: **DROP
     IT** unless there is a genuinely new development (e.g., a regulatory
     decision was announced yesterday; today a major company responded).
   - If a candidate was a **Quick Hit** previously AND now has significant new
     developments: it MAY be promoted to a main story with a note like
     "Following up on [date]'s Quick Hit..."
   - A story about the **same company** is fine if it's a **different event**.

4. **Minimum novelty requirement:** At least 3 of the main stories must be
   genuinely new events — not follow-ups or continuations of previous coverage.

5. **After saving the digest:** Append all newly included items to
   `digest-log.json`. Include items from all sections (main and quick_hit).

6. **Log maintenance:** If the log exceeds 200 entries, trim the oldest entries
   to keep only the most recent 150.

## Edge Cases

- **Slow news day:** It's fine to produce a 2-3 story digest. Say so up front:
  "A quieter day in AI — here's what's worth your attention."
- **Major breaking news:** Lead with the big story and give it more space.
  Other stories can be compressed into Quick Hits.
- **Conflicting reports:** Note the disagreement. "Company X claims Y, but
  researchers at Z dispute this, citing..."
- **Embargoed or paywalled content:** Don't reproduce paywalled articles.
  Summarize what's publicly known and link to the source.

## Sub-Agent Model Routing (Fallback)

If no project-level model routing policy applies, default sub-agents to Sonnet;
use Haiku for pure classify/extract work.
