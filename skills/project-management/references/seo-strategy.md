# Organic traffic strategy & guidelines

> These guidelines apply to all content intended for organic search. Reference this document whenever writing or optimizing web content.
> Last updated: April 2026. Updated to reflect April 2026 site performance data, B2B/AI strategic pivot, MOFU/BOFU content priority, course landing page audit SOP, and comparison against the December 2025 SEO agency plan. Second pass: reviewed against transcripts from AEO/GEO live courses (Steve Toth, Oct 2025) and Content Strategy for LLM Visibility live courses (Alex Birkett, Dec 2025). Key additions: off-page AEO strategy (Section 8b), query fanout implications (Section 1), truth alignment SOP (Section 8c), AI Info Page, passage-level optimization (Section 2), deal breaker content type (Section 9).

---

## Core SEO Philosophy

We optimize for search intent first, keyword density second. A piece of content that fully satisfies what a searcher actually needs will outperform content stuffed with keywords but lacking substance. Our goal is to be the best answer to the question, not just a page that contains the question.

We also optimize for AI-generated answers. As LLMs (ChatGPT, Perplexity, Gemini, Claude) become primary discovery channels for B2B marketers, CXL content needs to be structured and cited in ways that surface in AI responses, not just in the Google 10-blue-links format. This is the AEO/GEO objective described in Section 8.

Both objectives compound: content that is well-structured for humans tends to also be easier for AI to summarize and cite.

**Strategic direction from April 2026:** CXL is repositioning toward B2B marketing and AI in marketing. This changes the SEO priority order. We are no longer optimizing primarily for traffic volume. We are optimizing for qualified traffic from B2B practitioners who are evaluating training for themselves or their teams. MOFU and BOFU content now takes priority over TOFU blog expansion. New content briefs should default to MOFU or BOFU unless there is a specific TOFU gap with strong traffic potential and clear pipeline connection.

---

## Current State: Site Performance (April 2026)

Data sourced from Ahrefs and GSC pull, April 2026. Use these baselines when evaluating content priorities and setting targets.

### Organic overview

| Metric | Value |
|---|---|
| Organic keywords | 8,691 |
| Keywords in positions 1–3 | 2,055 |
| Estimated monthly organic traffic | ~69,000 visits |
| Pages with 1K+ monthly organic traffic | 75 |
| Pages with 5K+ monthly organic traffic | 10 |
| Pages with 10K+ monthly organic traffic | 3 |

### Top pages by clicks (GSC, Jan–Apr 2026)

| Page | Clicks | Impressions | CTR | Notes |
|---|---|---|---|---|
| Homepage | 11,138 | 1,345,112 | 0.83% | Branded |
| Institute hub | 2,381 | 185,874 | 1.28% | Mixed branded/non-branded |
| A/B test calculator | 1,312 | 54,346 | 2.41% | Tool page; strong CTR |
| AEO guide (original) | 1,035 | 294,429 | 0.35% | CTR problem — see note |
| USP examples | 991 | 195,666 | 0.51% | CTR problem |
| Value proposition | 750 | 248,295 | 0.30% | CTR problem |
| Growth marketing program | 669 | 58,493 | 1.14% | Course page performing |
| AEO guide (2025 version) | 613 | 161,947 | 0.38% | Self-cannibalization — see note |
| CRO minidegree | 611 | 177,128 | 0.34% | CTR problem |
| CTR benchmarks | 587 | 341,809 | 0.17% | Severe CTR problem |
| Differentiation strategy | 563 | 69,535 | 0.81% | |
| Cialdini principles | 532 | 141,997 | 0.37% | CTR problem |
| Meta ads course | 429 | 29,384 | 1.46% | Transactional; good CTR |
| AI SEO courses (blog) | 381 | 52,219 | 0.73% | AI content traction |
| AI marketing courses (blog) | 349 | 44,127 | 0.79% | AI content traction |

**CTR alert:** Six pages with 50K+ impressions each are sitting below 0.8% CTR. These pages already rank. The problem is the title or meta description. Fixing these is the highest-leverage quick win on the site — more clicks without any new content or link building.

**Cannibalization alert:** Two versions of the AEO guide are both ranking and splitting traffic. `/blog/answer-engine-optimization-aeo-the-comprehensive-guide/` (1,035 clicks) and `/blog/answer-engine-optimization-aeo-the-comprehensive-guide-for-2025/` (613 clicks) are competing for the same keyword cluster. These need to be consolidated. See Section 12 for the audit SOP.

### What the December 2025 performance data showed

- US organic sessions down 13.8% Dec vs Nov; organic revenue up 139.9%
- Blog traffic down 28–29%; course page traffic up 17.7%
- AI in B2B marketing minidegree was the top course page by traffic
- ChatGPT referrals down 29%; Gemini up 49%
- Course keywords on page 1: increased to 168 (from 153); B2B keywords on page 1: decreased to 123 (from 127)

**The right read on this data:** Sessions falling while revenue rises is not a problem — it is a signal that traffic is getting more qualified. The TOFU blog content that was generating sessions is less relevant to who CXL is now. The right response is not to recover blog traffic. It is to build content that brings in the people who buy, not just the people who read.

---

## 1. Keyword Research and Targeting

### Primary keyword

- Every page or article targets one primary keyword.
- The primary keyword must have clear search intent alignment (informational, navigational, commercial investigation, or transactional).
- Include the primary keyword in: title/H1, first 100 words, at least one H2, meta description, and URL slug.

### Secondary keywords

- Include 2–5 semantically related secondary keywords naturally within the body.
- Do not force secondary keywords. If a sentence sounds unnatural, remove the keyword.

### Keyword difficulty targets

Based on current site authority, CXL can rank for competitive terms (KD up to 78, e.g., "value proposition"). Use these ranges as a starting framework. Adjust based on SERP quality for each term.

| Content type | Target KD | Target monthly search volume |
|---|---|---|
| Competitive pillar content | 40–70 | 3,000+ |
| Supporting cluster articles | 15–40 | 500–5,000 |
| Long-tail / quick wins | 0–20 | 100–1,000 |
| Team/agency/B2B conversion content | 0–35 | 20–200 (low volume, high CPC signals intent) |

### B2B and AI marketing keyword landscape (April 2026)

These are the strategic keyword targets for the B2B/AI pivot. Volumes are modest but CPCs confirm commercial intent. The traffic potential of adjacent and related terms is the more useful metric here.

| Keyword | Volume (US) | Difficulty | Traffic potential | CPC | Priority |
|---|---|---|---|---|---|
| ai marketing course | 600 | 51 | 2,500 | $3 | High — already showing traction |
| ai marketing training | 300 | 48 | 2,800 | — | High — best TP in this set |
| ai for b2b marketing | 250 | 42 | 200 | — | Medium — informational, use as cluster |
| b2b marketing training | 100 | 30 | 450 | $8 | High — highest CPC = strongest buying intent |
| b2b marketing certification | 90 | 20 | 150 | $5 | Medium — lower TP but low difficulty |
| b2b marketing course | 100 | 19 | 70 | $5 | Medium — low TP, use as secondary |
| marketing team training | 20 | 27 | 200 | $4 | Medium — feeds team plan pages |
| marketing agency training | 100 | 7 | 150 | — | Easy win — very low difficulty |
| n8n marketing automation | 100 | — | — | — | Strategic — own this term early |

**How to use this table:** Do not chase volume here. The search volumes are low by blog standards. The play is to own these terms before demand peaks, build topical authority, and use these pages as conversion surfaces for B2B team buyers who search with high intent at low volume.

### Priority action list: quick wins (April 2026)

Organized by action type, not keyword volume.

**Category 1: CTR fixes (existing rankings, title and meta only — no content rewrite needed)**

| Page | Impressions (90d) | Current CTR | Action |
|---|---|---|---|
| AEO guide (original) | 294,429 | 0.35% | Rewrite title and meta — test benefit-led vs question-led |
| CTR benchmarks | 341,809 | 0.17% | Severe underperformance; title test priority |
| Value proposition | 248,295 | 0.30% | Update title to front-load keyword; sharpen meta hook |
| Cialdini principles | 141,997 | 0.37% | Title may be too academic; test practitioner framing |
| CRO minidegree | 177,128 | 0.34% | Course page CTR should be 1%+; meta needs outcome framing |
| USP examples | 195,666 | 0.51% | Title test: lead with use case, not definition |

**Category 2: MOFU/BOFU content gaps (net new or major rewrites)**

| Content piece | Target keyword | Funnel stage | Feeds to |
|---|---|---|---|
| AI marketing training hub | ai marketing training | MOFU | AI courses, team plan |
| B2B marketing training guide | b2b marketing training | MOFU | for-team, for-growing-teams |
| Marketing training for agencies | marketing agency training | MOFU | for-agencies |
| How to upskill your B2B marketing team | marketing team training | MOFU | for-growing-teams |
| CXL for teams vs individual plans | — (navigational) | BOFU | Pricing, team pages |

**Category 3: AEO cannibalization fix**

Consolidate the two AEO guide URLs into one authoritative page. Redirect the lower-authority version. This recovers split link equity and unifies ranking signals. See Section 12 for audit SOP.

**Category 4: Transactional page optimization**

| Page | Impressions (90d) | Current CTR | Gap |
|---|---|---|---|
| Meta ads course | 29,384 | 1.46% | Position 6 — title/meta + schema push to top 3 |
| Growth marketing program | 58,493 | 1.14% | Title optimization + keyword expansion |

### Query fanout and zero-volume opportunities

When a user enters a query into an AI platform, the system generates dozens of synthetic sub-queries behind the scenes (called "query fanout"). Research shows 95% of these sub-queries have zero traditional search volume — they do not appear in Ahrefs or GSC. This means keyword tools undercount the actual opportunity for content that is structured to be retrieved by AI systems.

Implication: do not disqualify content topics solely because keyword tools show low or zero volume. Topics with genuine buyer signal but low search volume may have significant AI fanout opportunity. Use voice-of-customer data (sales call themes, support tickets, Reddit, G2 reviews) alongside keyword volume to validate topics. A question that appears repeatedly in customer conversations but has zero Ahrefs volume is still worth producing content for.

### Tools we use

- **Ahrefs** (connected via Claude.ai): keyword research, competitor gap analysis, backlink monitoring, organic traffic analysis
- **Google Search Console** (MCP-connected): impression and CTR data, query mining, indexing status
- **Google Analytics 4** (MCP-connected): traffic, engagement, conversion by page and channel
- **Peec AI**: LLM visibility tracking — monitors whether CXL appears in AI-generated answers for target queries
- **Peak AI or Profound**: citation source mapping — identifies which domains and URLs AI systems cite when answering category queries. Use before any off-page AEO outreach campaign. (See Section 8b.)

Always pull live data before finalizing keyword strategy for any brief. Do not estimate metrics.

---

## 2. On-Page Optimisation Checklist

Use this checklist for every piece of SEO content before publishing.

### Title and meta

- [ ] Title tag: Primary keyword near the front; under 60 characters; compelling for clicks.
- [ ] Meta description: Primary keyword included; clear benefit or hook; under 155 characters.
- [ ] URL slug: Short, lowercase, hyphen-separated; includes primary keyword; no stop words.

### Content structure

- [ ] H1 matches or closely mirrors the target keyword.
- [ ] H2s cover the main subtopics searchers expect (check SERP "People also ask" boxes).
- [ ] Primary keyword appears in the first 100 words.
- [ ] Content length is competitive for the target keyword (check top 3 ranking pages).
- [ ] TL;DR or key takeaway box at the top for articles over 1,000 words (required for AEO).
- [ ] Answer-first structure: lead with the direct answer before elaborating.
- [ ] Passage-level optimization: each major section should be self-contained enough that it makes sense if extracted and quoted without surrounding context. AI systems retrieve chunks, not full pages.
- [ ] Semantic overlap: key concepts are rephrased at least once using different wording. This broadens the range of sub-queries the content matches in AI retrieval. Do not keyword-stuff; rephrase naturally within the prose.

### Internal linking

- [ ] At least 2 internal links to relevant existing content.
- [ ] At least 1 internal link from an existing page pointing to this new content (after publishing).
- [ ] Anchor text is descriptive, not "click here" or "read more."
- [ ] If the content belongs to a cluster, it links to its pillar page (see Section 10).
- [ ] If the content is MOFU or BOFU, it links to the relevant course or team landing page.

### Images and media

- [ ] All images have descriptive alt text (primary keyword used naturally in at least one).
- [ ] Images are compressed and optimized for web.
- [ ] Image file names use hyphens and describe the content.

### Technical

- [ ] Page loads quickly on mobile (test with PageSpeed Insights).
- [ ] Schema markup applied where relevant (Article, FAQ, HowTo, Course).
- [ ] No broken links on the page.
- [ ] Canonical tag is set if content is adapted from another source.

---

## 3. Search Intent and Funnel Framework

### Intent types

| Intent | What the searcher wants | Our content approach |
|---|---|---|
| **Informational** | To learn or understand something | Comprehensive, evidence-led; prioritize depth and accuracy over breadth |
| **Navigational** | To find a specific CXL page or resource | Brand/product pages; clear navigation to destination |
| **Commercial investigation** | To evaluate options before buying | Comparison content, case studies, outcome-led proof |
| **Transactional** | To take an action (sign up, enroll, buy) | Course landing pages with clear offer and single CTA above fold |

### Funnel stage framework

Every piece of content should be assigned a funnel stage before briefing. The stage determines the format, CTA, and internal link destination.

**TOFU (top of funnel) — awareness**
- Searcher is learning; not ready to buy
- Format: definitional, how-to, benchmark, listicle
- CTA: newsletter signup, free resource download
- Internal link to: pillar page on the topic
- Examples: "what is answer engine optimization," "B2B marketing strategy guide," "differentiation strategy examples"
- Current CXL TOFU estate: strong (legacy CRO content), but declining in relevance to current ICP

**MOFU (middle of funnel) — evaluation**
- Searcher knows the problem; evaluating solutions and approaches
- Format: comparison, "how we do X," outcome-led how-to, skills guide, case study
- CTA: team plan trial, webinar signup, course enrollment
- Internal link to: relevant course landing page or team plan page
- Examples: "how to train your B2B marketing team on AI," "marketing attribution tools compared," "b2b demand gen playbook"
- Current CXL MOFU estate: thin — this is the primary content gap

**BOFU (bottom of funnel) — decision**
- Searcher is ready to act; evaluating CXL specifically
- Format: pricing page, team landing page, course landing page, testimonial-led page
- CTA: single conversion action (enroll, start trial, contact sales)
- Internal link to: pricing, related courses
- Examples: team plan pages (for-team, for-agencies, for-growing-teams), course enrollment pages, pricing page
- Current CXL BOFU estate: exists (course pages, pricing, team pages) but under-optimized for SEO and CTR

**Default rule for new content:** Unless there is a specific, data-confirmed TOFU gap with strong traffic potential and clear pipeline connection, new content briefs default to MOFU. The current TOFU estate is already large relative to MOFU. Adding more TOFU without connecting it to conversion is generating sessions that do not become customers.

---

## 4. Content Freshness

- Review high-traffic pages every 6 months to update stats, examples, and links.
- Pages with outdated citations (pre-2022 studies, old screenshots, old brand references) are priority refresh candidates.
- Add a "Last updated: [month year]" note at the top of any article that is refreshed.
- Redirect or consolidate pages with overlapping keyword targets.
- Sunset content that cannot be meaningfully updated and has no inbound links.
- Do not use relative time references in new content ("recently," "last year," "a few months ago"). Use actual dates or ranges. This prevents freshness decay.

**Current refresh priority:** AEO guide consolidation (two URLs competing), plus the five high-impression/low-CTR pages listed in Section 1. Title and meta updates count as a refresh and trigger a date update.

**Old brand references to fix:** The blog style guide still references `conversionxl.com` in its internal search example. All internal search examples should use `cxl.com`.

---

## 5. Link Building

**Approved tactics:**
- Original research and data reports (Wynter panels, internal survey data). These earn editorial links.
- Guest contributions on vetted B2B marketing publications
- Digital PR: outreach around data-led stories and original research findings
- Resource page link placements on marketing and martech sites
- Building tools and calculators (e.g., A/B test calculator) that earn passive links

**Prohibited tactics:**
- Paid links (violates Google guidelines)
- Link exchanges
- Low-quality directory submissions
- Comment spam

---

## 6. Key Metrics to Track

| Metric | Tool | Current baseline (Apr 2026) | Target | Review frequency |
|---|---|---|---|---|
| Organic sessions | GA4 | ~69K/month | Protect quality; volume secondary | Weekly |
| Keywords in positions 1–3 | Ahrefs | 2,055 | +20% YoY | Monthly |
| CTR on non-branded pages | Search Console | 0.17–0.81% for top 10 TOFU pages | 1%+ across top 10 | Monthly |
| "Answer engine optimization" position | Ahrefs | ~3–4 | Top 2 | Monthly |
| AI marketing training keyword position | Ahrefs | Not yet ranking | Page 1 | Monthly |
| LLM citation rate | Peec AI | Baseline TBD | Month-on-month growth | Monthly |
| ChatGPT referrals | GA4 | Declining (Dec: -29%) | Stabilize, then grow | Monthly |
| Course page organic revenue | GA4 | Up 139.9% Dec vs Nov | Sustain growth | Monthly |
| Backlinks (new/lost) | Ahrefs | Monitor | Net positive | Monthly |
| Core Web Vitals | PageSpeed Insights | Monitor | All green | Quarterly |

**Note on sessions vs. revenue:** Organic sessions falling while course page revenue rises is a positive signal, not a problem. The metric that matters is qualified traffic converting. Do not optimize to recover sessions from TOFU blog content if that content does not convert.

---

## 7. Local SEO

Not applicable. CXL is a global digital product. No local SEO component.

---

## 8. AEO / GEO: Answer Engine and Generative Engine Optimisation

This is a dual objective alongside traditional SEO. From the CXL vision: "Stabilize organic and own LLM search. Get CXL cited in more results from LLMs and continue to build on early traction in this channel."

### What it means

AEO (Answer Engine Optimisation) targets featured snippets and AI overviews in Google Search. GEO (Generative Engine Optimisation) targets citation in AI-generated responses from ChatGPT, Perplexity, Claude, and Gemini.

CXL already has early traction: "answer engine optimization" ranks position 3–4 with 294K GSC impressions in 90 days. ChatGPT referrals fell 29% in December — this is a gap to close, not ignore. Peec AI tracking should be set up to monitor CXL's presence in LLM responses for priority queries.

### Content requirements for AEO/GEO

Every long-form article should include:
- **TL;DR box at the top:** 3–5 bullets that summarize the article's answers. This is the most impactful AEO signal.
- **Answer-first structure:** Open each major section with the direct answer, then elaborate. Do not bury the answer.
- **Definitions for key terms:** When introducing a concept, define it in 1–2 sentences. AI systems pull clean definitions.
- **Consistent entity naming:** Use the full term consistently (e.g., "answer engine optimization" not "AEO" throughout body copy). AI systems match on entity names.
- **Schema markup:** Article and FAQ schema help both Google AI overviews and third-party LLMs.
- **Authoritative sourcing:** Cite primary sources (studies, data) rather than second-hand summaries. LLMs favor well-sourced content.

### Which content types benefit most from AEO/GEO optimization

1. Definitional and how-to content (e.g., "what is answer engine optimization")
2. Benchmark and data content (e.g., "average CTR by industry")
3. Comparison content (e.g., "n8n vs Zapier for marketing automation") — see note on hyper-targeted comparisons below
4. Course descriptions and curriculum overviews (positions CXL as a cited source for AI marketing training)
5. Deal breaker content: pages that explicitly address why buyers might reject CXL (pricing, team seat minimums, course format, certification value). LLMs surface these objections when users ask for recommendations. Having credible, transparent content on these questions means LLMs cite CXL rather than a competitor or a forum.

**Hyper-targeted comparison pages:** Generic "A vs B" pages are not enough. Effective AI-cited comparison content is specific: "CXL vs [competitor] for B2B demand gen teams," "live courses vs on-demand training for marketing managers." Structure these pages as self-contained arguments, not feature checklists. The specificity of ICP and use case is what makes AI systems retrieve them for long-tail, high-intent sub-queries.

### LLM visibility tracking

Use Peec AI to monitor whether CXL appears in AI-generated answers for target queries. When Peec AI flags a gap (CXL not cited for a term we should own), that signals either a content gap or a structured data gap. Cross-reference with Ahrefs and GSC before deciding which it is.

Priority queries to monitor (build this list in Peec AI):
- "best AI marketing courses"
- "b2b marketing training platform"
- "answer engine optimization guide"
- "how to use n8n for marketing"
- "marketing training for B2B teams"

### 8b. Off-page AEO/GEO strategy

**This is the most underinvested area in CXL's current SEO/AEO approach.** Research across multiple AI visibility platforms shows approximately 95% of the URLs that AI systems cite as sources are earned, off-page media — not owned content. On-page optimization is necessary but is not sufficient for LLM visibility.

The on-page content gets CXL indexed and ranked in Google. The off-page presence gets CXL cited in AI-generated answers. Both require attention.

**Citation source mapping (do this before outreach)**

Use an AI visibility platform (Peak AI or Profound) to identify which domains and URLs most frequently appear as citation sources when AI tools answer queries in CXL's target category. Filter for:
- Editorial listicles and roundups ("best B2B marketing courses")
- Review aggregators (G2, Capterra, Clutch)
- Community platforms (Reddit, LinkedIn communities)
- YouTube and podcast content in the category
- Competitor pages that appear as "alternatives" sources

Score each opportunity by: citation frequency, feasibility of inclusion, and strategic fit. Prioritize outreach based on contact availability and how often the source is cited across multiple AI platforms.

**Tactical approaches by citation channel**

| Channel | Tactic | Notes |
|---|---|---|
| Editorial listicles | Outreach for inclusion in "best X" roundups; offer reciprocal link or affiliate arrangement | Build relationships before asking; cold outreach rarely works without an existing connection or incentive |
| G2 / Clutch / Capterra | Create or update CXL listings; run customer NPS campaigns to drive reviews | Review volume and recency affect AI citation frequency; treat this as ongoing customer marketing |
| Reddit | Build credibility through genuine participation, not promotion; employee advocacy in relevant subreddits | Reddit functions as a mirror of brand awareness, not a direct outreach channel; forced promotion backfires |
| YouTube | Original content, instructor guest appearances, affiliate/partner UGC | YouTube increasingly appears in AI-generated answers; instructor-led content from course experts is the fastest path |
| LinkedIn | Publish original research; instructor thought leadership; encourage employee advocacy | LinkedIn citation in AI outputs is growing; team-level posting amplifies reach beyond a single brand account |

**The Matthew Effect:** Early momentum in AI search compounds. Brands that accumulate citations first gain higher citation frequency, which generates further visibility. This favors moving now rather than waiting.

**Off-page AEO is cross-functional:** sustainable off-page presence requires alignment between SEO, PR, product marketing, and customer experience. Each function shapes what people say about CXL across the web. Co-ordinate citation-building efforts rather than treating them as an SEO-only task.

### 8c. Truth Alignment: auditing how AI represents CXL

LLMs do not always represent CXL accurately. They may attribute courses to the wrong instructors, describe our audience incorrectly, or omit key differentiators. Left unmanaged, inaccurate AI representations reduce conversion even when CXL does get cited.

**Truth Alignment SOP**

1. **Create a truth notebook.** A concise, factual document covering: what CXL is, who it is for, what makes it different, key course topics, instructor credentials, pricing model, and common misconceptions. Keep it under 1,000 words. Update when anything material changes.

2. **Run probe prompts.** Monthly, ask ChatGPT, Perplexity, Gemini, and Claude: "What is CXL?", "Who is CXL for?", "What courses does CXL offer?", "How does CXL compare to [competitor]?" Save the responses.

3. **Grade accuracy.** Compare responses against the truth notebook. Flag: missing information, factual errors, outdated references, and competitor advantages that go unchallenged.

4. **Fix the source material.** Inaccurate LLM output usually traces to a gap in the sources LLMs use (Wikipedia absence, outdated press coverage, missing G2 reviews, thin course descriptions). Fix the source, not the LLM output directly.

5. **Add an AI Info Page.** Create a dedicated, machine-readable page ("About CXL for AI systems" or "Learn about CXL") in markdown format, linked from the site footer. This page should contain the truth notebook content in clean, parseable text. LLMs index and retrieve these pages when forming brand descriptions. This is a low-effort, high-leverage tactic that should be built once and maintained alongside the truth notebook.

6. **Repeat monthly.** Track whether accuracy improves after source material changes. Peec AI monitoring (Section 8 above) shows whether CXL is cited; truth alignment work ensures the citation is accurate.

---

## 9. Content-Type SEO: Rules by Format

Apply the checklist in Section 2 to all SEO content, then layer on the format-specific rules below.

### Blog and long-form articles

**Intent target:** Informational (TOFU) or commercial investigation (MOFU).

**Before writing:**
- Confirm which funnel stage this serves (TOFU or MOFU). If TOFU, confirm there is a clear pipeline connection — which course or team page does this lead to?
- Confirm which ICP this is written for. The intro framing, examples, and language should match that persona's context. Do not write for both ICPs in the same post.
- Pull Ahrefs and GSC data for the target keyword before starting. Do not brief without data.

**Structure:**
- Lead with the direct answer before elaborating (answer-first structure).
- TL;DR box at the top is required for articles over 1,000 words. This is also the primary AEO signal.
- Each H2 section opens with a 1–2 sentence direct answer before supporting detail.
- Content length should match the competitive average for the target keyword. Check the top 3 ranking pages.

**Internal linking:**
- Minimum 2 internal links; at least 1 inbound internal link from an existing page after publishing.
- TOFU posts link to their pillar page and at least one MOFU article on the same topic.
- MOFU posts link to the relevant course or team landing page.

**AEO/GEO requirements apply in full** (see Section 8): definitions, entity consistency, FAQ schema.

**CTAs:**
- TOFU: newsletter signup or free resource download.
- MOFU: course enrollment, team plan trial, or webinar.
- Every blog post ends with a CTA block. The CTA must connect to the article's topic. Generic "explore our courses" CTAs are not acceptable.

**Freshness rules:**
- No relative time references ("recently," "last year," "a few months ago"). Use actual dates or ranges.
- Stats-heavy posts should note the data source date and flag for review when that source updates.

**Style guide alignment:**
- No em dashes. Restructure with a comma, colon, or full stop.
- Titles are title case; all headings below H1 are sentence case.
- Numbers: spell out one through nine; use numerals for 10 and above.
- Images: descriptive alt text, hyphened file names, compressed for web.
- Internal links: use `cxl.com` not `conversionxl.com` in any site search references.

### Course landing pages

**Intent target:** Transactional (BOFU). The searcher is evaluating whether to enroll. Do not write for informational queries on landing pages.

**Before creating a new course page — mandatory pre-check:**
Run the cannibalization check in Section 12 before creating any new course landing page. If an existing page (including archived pages) already ranks for the target keyword, update or reuse that page. Do not create a second page targeting the same term.

**Keyword targeting:**
- Primary keyword: the course topic phrase a practitioner would search when actively looking for training (e.g., "n8n marketing automation course," "answer engine optimization training").
- Use Ahrefs to confirm search volume and difficulty. Prefer keywords in the 200–2,000 monthly search volume range for course-specific terms.
- Use GSC to check if CXL already ranks for the term. If an existing page ranks for the same keyword, flag cannibalization before proceeding.
- See Section 1 for B2B/AI keyword targets by priority.

**Title and H1:**
- SEO title format: `[Primary Keyword Phrase] | CXL` — 60-character max.
- H1 (the large red-highlighted headline on the page): must include the primary keyword or a close variant. Keep under 70 characters. No forced line breaks.
- Do not optimize the functional title ("Live Course: [Name]") for search. It is a label, not a headline.

**Meta description:**
- Include the primary keyword naturally.
- Lead with the outcome or result, not the format.
- 135-character max.
- Avoid repeating the SEO title word-for-word.

**On-page structure:**
- The hero section is the primary conversion zone. One CTA above the fold.
- Outcome bullets in the hero (max 5) must not restate the H1 or excerpt.
- Schema: apply `Course` schema to all course landing pages.
- Do not add a TL;DR box. Landing pages are not articles; the hero section serves this function.

**Cannibalization check:**
- Before finalizing the keyword, run Ahrefs to confirm no other CXL page already targets the same primary keyword with higher authority. If a conflict exists, note it and flag to the user before proceeding.
- Check archived and redirected pages in addition to live pages. See Section 12.

---

## 10. Pillar and Cluster Architecture

CXL content should be organized into topic clusters. Each cluster has one pillar page (comprehensive, high-authority, often ranking for a high-volume keyword) and multiple cluster articles (narrower, feeding traffic and link equity back to the pillar). Every piece of new content should be placed into a cluster before it is briefed.

### Current clusters

**Cluster 1: CRO and conversion (existing strength — maintenance mode)**
- Pillar: Conversion rate optimization guide (`/conversion-rate-optimization/`)
- Cluster articles: landing page conversion, A/B testing, CTA optimization, statistical power, social proof
- Action: CTR fixes on existing pages. No new content needed unless there is a specific gap confirmed by GSC data.

**Cluster 2: AI in B2B marketing (emerging — active build)**
- Pillar: To be created — "AI marketing training" as the hub
- Cluster articles: ai marketing course roundup (exists), ai seo course roundup (exists), ai for b2b marketing, n8n marketing automation, answer engine optimization
- Action: Pillar page needed. Connect existing cluster articles to it with internal links. Extend to MOFU with training/team use cases.

**Cluster 3: B2B marketing skills (new — to build)**
- Pillar: "B2B marketing training" or "B2B marketing skills" — to be created
- Cluster articles: demand gen training, marketing attribution, marketing ops, marketing team upskilling, b2b marketing certification
- Action: Plan cluster before briefing individual posts. Each article should feed the pillar and link to a relevant course or team page.

**Cluster 4: Marketing team training (new — feeds team plan pages)**
- Pillar: "Marketing training for teams" or "upskilling your marketing team" — to be created
- Cluster articles: for-agencies content, for-growing-teams content, marketing training ROI, team plan comparison
- Action: MOFU content cluster. Each article links to the relevant team landing page (for-team, for-agencies, for-growing-teams). See Section 11.

### Internal linking rules

- Every cluster article links to its pillar page.
- Every MOFU cluster article links to at least one course or team landing page.
- Pillar pages link to their cluster articles.
- No orphan content: every new page must have at least one inbound internal link from an existing page on the day it publishes.

---

## 11. Team Plan Content Cluster

CXL has three team-focused landing pages: `for-team`, `for-agencies`, `for-growing-teams`. These are BOFU conversion pages. The keyword research confirms there is no high-volume direct search demand for these pages. Organic traffic to them will come from MOFU content that builds trust and hands off to the page.

### MOFU content plan

| Content piece | Funnel stage | Target keyword | Volume | KD | Feeds to |
|---|---|---|---|---|---|
| How to upskill your B2B marketing team on AI in 2026 | MOFU | marketing team training | 20/mo | 27 | for-growing-teams |
| Marketing training for agencies: building AI skills across client teams | MOFU | marketing agency training | 100/mo | 7 | for-agencies |
| B2B marketing skills your team needs to fill pipeline in 2026 | MOFU | b2b marketing training | 100/mo | 30 | for-team |
| CXL for teams vs. individual plans: how to decide | BOFU | marketing training platform | — | — | Pricing, team pages |

### BOFU page optimization

Before driving traffic to the team pages, audit each one against the landing page rules in Section 9. Check:
- Does the SEO title and meta include a keyword with commercial intent?
- Is there one clear CTA above the fold?
- Does the page include `Course` or `Service` schema?
- Are outcome bullets specific enough to resonate with ICP 2 (Head of Marketing, Series A–C)?

### Success metrics for the team plan cluster

Volume is not the right metric here. The right metrics are:
- Team page conversion rate (from cluster article traffic)
- Demo or trial requests attributed to MOFU content
- Time-on-page for MOFU posts landing on team pages

---

## 12. Course Landing Page Audit and SOP

### The problem

CXL has accumulated course landing pages over time, some of which have been archived, redirected, or left as drafts. When new courses are released on related topics, two risks arise:

1. **Keyword cannibalization:** A new page targets the same keyword as an archived page that still has organic authority. Both pages rank weakly instead of one page ranking strongly.
2. **Wasted equity:** An archived page with strong backlinks or historical rankings is redirected to the homepage instead of being reused for a closely related new course. The accumulated authority is discarded.

The AEO guide duplication currently live on the site is an example of cannibalization in action: two URLs competing for the same 294K-impression keyword cluster.

### Pre-launch audit: before creating any new course landing page

Run this checklist before starting the `/buildlandingpage` workflow.

**Step 1: Keyword check**

Pull Ahrefs organic keywords for `cxl.com` filtered to the course topic. Also check GSC for queries the site is already receiving for the topic. Identify:
- Is any CXL page currently ranking (positions 1–50) for the target keyword or close variants?
- Is any CXL page receiving impressions (even at low position) for the target keyword?

If yes to either: go to Step 2 before creating a new page.

**Step 2: Existing page audit**

For each existing page found in Step 1:
- Is the page live, draft, archived, or redirected?
- What is the current URL and page ID? (Check Airtable WP pages table)
- Does the page's topic still match the new course closely enough to reuse?
- Does the page have inbound links? (Check Ahrefs backlinks for the specific URL)
- Does the page have a history of ranking for the target keyword?

**Decision matrix:**

| Existing page status | Keyword overlap | Inbound links | Decision |
|---|---|---|---|
| Live, same topic | High | Yes | Update existing page — do not create new |
| Live, same topic | High | No | Update existing page — do not create new |
| Live, adjacent topic | Moderate | Yes | Update existing; add new section for new course angle |
| Archived/draft, same topic | High | Yes | Restore and update — do not create new |
| Archived/draft, same topic | High | No | Restore and update if content is salvageable; otherwise create new |
| Redirected to homepage | High | Yes | Restore the redirect target; update for new course |
| Redirected to homepage | High | No | Create new page; set canonical; monitor |
| No existing page | — | — | Create new via `/buildlandingpage` |

**Step 3: Consolidation (if required)**

If two live pages are competing for the same keyword:
- Identify the stronger page (more backlinks, higher position, more GSC impressions).
- Redirect the weaker page to the stronger page (301).
- Migrate any unique content from the weaker page into the stronger page before redirecting.
- Update Airtable WP pages table for both pages.
- Add a note in the proposal file and campaign log.

### SOP: creating a new course landing page with SEO and AEO in mind

Use this sequence every time. This runs alongside (and before) the `/buildlandingpage` command.

**Phase 1: Research (before any writing)**

1. Pull Ahrefs data for the course topic: volume, difficulty, traffic potential for the primary keyword and 5 close variants.
2. Pull GSC data for the topic: existing impressions, CTR, and current ranking URLs.
3. Run the pre-launch audit above (Step 1–3).
4. Identify the primary keyword, one secondary keyword, and 2–3 supporting terms.
5. Confirm no existing CXL page should be updated instead of a new page being created.

**Phase 2: Keyword decisions (before writing)**

6. Set the primary keyword. It must be:
   - The most specific phrase a practitioner would search when actively looking for this training
   - In the 200–2,000 volume range (course-specific terms rarely exceed this)
   - Not already targeted by a stronger existing CXL page
7. Set the SEO title: `[Primary Keyword Phrase] | CXL` — 60-character max.
8. Draft the meta description: outcome-led, primary keyword included, 135-character max.
9. Confirm H1 includes the primary keyword or a close variant (under 70 characters).

**Phase 3: Page build (via `/buildlandingpage`)**

10. Follow the `/buildlandingpage` workflow for title, H1, excerpt, and WP creation.
11. Apply `Course` schema to the page (manual step in Yoast or via API if accessible).
12. Set the canonical URL to itself (not to a parent page or programme hub) unless this page is intentionally subordinate.

**Phase 4: AEO optimization (new step — add to every course page)**

13. Write a structured course description that includes:
    - A 2-sentence definition of what the skill/topic is (AI systems pull clean definitions)
    - A clear outcome statement: "After this course, you will be able to…"
    - Named tools, frameworks, or methods covered (entity signals for LLMs)
14. Ensure the curriculum/session outline uses full descriptive terms, not abbreviations (entity consistency for AEO).
15. Add FAQ schema covering: "What will I learn?", "Who is this course for?", "How long does it take?", "Is this live or on-demand?" These are the questions AI systems are asked when users query for course recommendations.

**Phase 5: Internal linking (before or immediately after publishing)**

16. Link from the relevant pillar page to this new course page.
17. Link from at least one MOFU blog post in the same topic cluster to this course page.
18. Link from the relevant team landing page (if applicable) to this course page.
19. Add an inbound link from the most closely related existing course or programme page.

**Phase 6: Post-launch tracking**

20. Add the page to the Airtable WP pages table with: page ID, slug, status, target keyword, SEO title, and date created.
21. Add the target keyword to the Ahrefs rank tracker for the CXL project.
22. Add the course topic to the Peec AI monitoring list for LLM citation tracking.
23. Set a 30-day review: check GSC for first impression data. If impressions are low and no ranking movement after 30 days, revisit the keyword choice and on-page optimization.

### Ongoing maintenance: quarterly course page audit

Every quarter, run this check across all live course and programme landing pages:

- Pull GSC data for each page: impressions, clicks, CTR, average position.
- Flag any page with 10K+ impressions and under 1% CTR — title/meta issue.
- Flag any page with zero GSC impressions after 60 days — indexing or crawl issue.
- Flag any two pages where the top GSC keywords overlap significantly — cannibalization risk.
- Check for archived or redirected pages still receiving inbound links (Ahrefs) — potential to restore.

---

## 13. Open Questions: Keyword Strategy

These questions need answers before we can fully define the keyword roadmap. Once answered, update the keyword targets in Section 1 and the content calendar.

1. **Core topic expansion:** CXL currently owns CRO and conversion content organically. Are we explicitly expanding into B2B marketing automation, AI in marketing, demand gen automation, and marketing ops as new topic clusters? (Current direction says yes — this should be confirmed and committed to.)

2. **AI/automation keywords to own:** Which specific keywords should CXL own in the AI marketing automation space? Candidates include: "n8n marketing automation," "B2B marketing automation," "AI marketing tools," "marketing workflow automation," "Claude for marketing." Which are priorities?

3. **Course-specific SEO:** Each AI summer course maps to a search term. Should course landing pages be optimized for organic search, or are they purely for paid and direct traffic? If organic, what are the target keywords per course?

4. **LLM citation targets:** Which queries should CXL appear in when B2B marketers ask AI tools? (e.g., "best AI courses for B2B marketers," "how to automate marketing with n8n") Building a target list here would shape both content and PR strategy.

5. **Content velocity:** How many new SEO-focused articles can be produced per month? This determines how aggressively we can expand into new topic clusters vs. refreshing existing high-traffic content.

6. **Geographic priority:** Is the US the primary market, or are there specific countries to prioritize in the keyword strategy (e.g., UK, Canada, Australia)?

7. **Conversion goal for organic traffic:** What's the primary conversion action for blog readers: newsletter signup, course enrollment, or free trial? This affects which CTA appears on organic pages and how we measure SEO ROI.

8. **Archived course pages:** Which archived course pages have the strongest backlink profiles or historical rankings? These should be audited before any new courses in those topics are launched. Pull from Ahrefs — filter by `cxl.com/institute` URLs returning 4xx or 3xx.

---

## 14. Previous SEO Plan Reference: December 2025

This section documents the December 2025 SEO plan from the external SEO retainer, the performance context it was written against, and a comparison to the strategy in this document. Retained here as reference for continuity and decision-making.

### December 2025 performance summary (from external plan)

**US (Dec vs Nov):**
- Organic sessions: -13.8%
- Organic revenue: +139.9%
- Blog traffic: -28%
- Course page traffic: +17.7%
- GSC clicks: -21.3%; impressions: +4.5%
- Top course pages: AI in B2B marketing minidegree (#1), Meta Ads, CRO minidegree, Growth Marketing

**Global (Oct vs Sep):**
- Organic sessions: -18.5%
- Organic revenue: +76.4%
- Blog sessions: -29%; course page sessions: -21.6%; course page revenue: +62.2%
- Top course pages: AI in B2B marketing minidegree (#1), CRO minidegree, Growth Marketing, Optimize pages for AI Search

**LLM referrals:**
- ChatGPT: -29%
- Perplexity: -15%
- Gemini: +49%
- Claude: -15%

**Keyword rankings (US):**
- Course keywords on page 1: 168 (up from 153)
- Certification keywords on page 1: 72 (up from 66)
- AI keywords on page 1: 10 (up from 9)
- B2B keywords on page 1: 123 (down from 127)

### January 2026 plan (external SEO retainer — $900/month + ad hoc)

**Scope included:**
- 4 course page SEO reviews/month: growth marketing, brand marketing, demand gen, GTM strategy
- 8 blog topic validations/month (topics supplied by content team)
- 2 existing blog page optimizations: AI search vs traditional SEO, content strategy for AI search
- Ad hoc: Looker Studio dashboard ($400), Peec AI LLM tracking setup ($150), AI + marketing keyword research ($250)
- Total: $1,700/month

### Comparison: what the external plan got right

| Area | Assessment |
|---|---|
| Course page optimization cadence (4/month) | Correct approach. The four pages selected (growth marketing, brand marketing, demand gen, GTM strategy) are all MOFU/BOFU with commercial intent and existing page-1 presence. Keep this cadence. |
| Peec AI LLM visibility tracking | Right tool. CXL needs to monitor LLM citation gaps. Pair with a target query list (see Section 8). |
| Blog tightening methodology | Correct approach: identify what GSC says users are actually querying, then close the gap. The two pages selected (AI search vs traditional SEO, content strategy for AI search) were well-chosen MOFU pieces. |
| Blog topic validation process | Useful process gate. Prevents content being written for terms with no demand. Worth keeping as a step, not as the ceiling of SEO contribution. |

### Comparison: what the external plan missed or got wrong

| Area | Gap | What this document does instead |
|---|---|---|
| CTR optimization | Not mentioned at all. Six pages with 50K–341K impressions each sit below 0.8% CTR. This is the highest-leverage quick win on the site. | Section 1 priority action list, Category 1 |
| Funnel framework | No distinction between TOFU, MOFU, and BOFU. All blog content treated equally. | Section 3: funnel framework with rules per stage |
| Team plan content strategy | No mention of for-team, for-agencies, or for-growing-teams pages. | Section 11: team plan content cluster |
| Pillar/cluster architecture | No cluster logic. Content validated in isolation, not connected to a hub page or internal linking strategy. | Section 10: pillar and cluster architecture |
| B2B repositioning | Plan optimizes existing pages without acknowledging the strategic shift toward B2B/AI. The course pages selected don't include AI in B2B marketing (the #1 course page by traffic). | Sections 1, 3, 10 reflect B2B/AI priority |
| Course landing page cannibalization | No mention of duplicate or competing pages (the two AEO guide URLs are a live example). | Section 12: audit SOP |
| Data framing | Sessions falling while revenue rising was treated as a problem. It is a signal of improving traffic quality. | Current State section reframes this correctly |
| Keyword research output | $250 ad hoc item produces a Google Sheet. Research without a next step has a high rate of not being actioned. | All keyword research should feed directly into content briefs or page updates with an assigned owner. |
| Reactive topic sourcing | Content team supplies topics; SEO validates them. For a strategic pivot, SEO should be sourcing topics, not reacting to them. | Section 10 cluster architecture is the brief-generation framework. |

### What to carry forward

From the external plan:
- 4 course page optimizations/month cadence (add AI in B2B marketing minidegree to the rotation)
- Peec AI setup and ongoing LLM monitoring
- The blog tightening methodology (GSC gap → brief → update)

From this document, in addition:
- CTR optimization sprint (5 pages, titles and metas only, immediate)
- AEO guide cannibalization fix (consolidate two URLs)
- MOFU content cluster build (Section 11)
- Course landing page audit SOP (Section 12) before any new course pages are created

---

## 15. To Do

- [ ] **Airtable tracker for blogs and landing pages.** Create a dedicated Airtable table (or extend the existing WP pages table) to track SEO state for both blog posts and course/programme landing pages. Fields to include: URL, page type (blog/landing page), funnel stage (TOFU/MOFU/BOFU), target keyword, SEO title, meta description, GSC impressions (last 90d), GSC CTR, current position, cluster, last reviewed date, and status (optimized, needs update, flagged for consolidation). This becomes the operational tracking layer for the quarterly audit in Section 12.

- [ ] **Scheduled agent to monitor SEO performance.** Set up a recurring Claude Code agent (via `/schedule`) to run monthly. Agent should: pull GSC page data for the project, flag any page with 10K+ impressions and under 1% CTR, flag any two pages where top keywords overlap significantly (cannibalization signal), flag pages with zero impressions after 60 days, and post a summary to Slack or write findings to a report file. This replaces the ad hoc Looker Studio dashboard proposed in the December external plan with an automated, actionable output.

- [ ] **Layer in Tarek's n8n workflows.** Review Tarek's existing n8n workflows and identify which can feed into or extend the Airtable tracker and scheduled agent above. Likely integration points: automated GSC/Ahrefs data pulls into Airtable on a set cadence, Slack alert routing when the monitoring agent flags an issue, and any existing content publishing or page-update workflows that should trigger an Airtable row update. Avoid rebuilding what already exists — map first, then extend.

- [ ] **Create orchestration diagram.** Once the Airtable tracker, scheduled agent, and n8n workflow integrations are mapped, create a diagram showing how data flows between systems: GSC/Ahrefs → n8n → Airtable tracker → Claude monitoring agent → Slack/report output → human action. Include the WordPress page lifecycle (create → track → audit → update/consolidate → retire) and how it connects to the content pipeline (proposal file → buildlandingpage → Airtable). Use Miro or FigJam (both connected via Claude.ai integrations). This diagram becomes the onboarding reference for anyone new touching SEO or content ops.

- [ ] **Include internal linking review and proposals. Refreshing with new content** 

- [ ] **Include footer review and optimization** 

- [ ] **include category page and description review.** 

- [x] **Reviewed against course transcripts from Eurekos.** Done April 2026. Transcripts sourced from: Content Strategy for LLM Visibility (Alex Birkett, Dec 2025, 2 sessions) and Optimize pages for AI Search with GEO/AEO (Steve Toth, Oct 2025, 2 sessions). Key additions documented in this revision: Sections 8b, 8c, query fanout note in Section 1, passage-level optimization in Section 2, deal breaker content type and hyper-targeted comparison pages in Section 8.
- [ ] **Build the truth notebook.** Draft a 500–1,000 word factual document covering what CXL is, who it is for, key differentiators, course topics, pricing model, and common misconceptions. This becomes the source document for the AI Info Page (Section 8c). Owner needed.
- [ ] **Create the AI Info Page.** Once the truth notebook is drafted, publish a machine-readable "Learn about CXL" page in markdown. Link from the site footer. See Section 8c for the full SOP.
- [ ] **Run citation source mapping.** Use Peak AI or Profound to identify which domains AI systems cite when answering "best B2B marketing courses" and adjacent queries. Use output to prioritize off-page outreach targets. See Section 8b.
- [ ] **First truth alignment probe.** Run the five probe prompts in Section 8c against ChatGPT, Perplexity, Gemini, and Claude. Grade against the brand facts in CLAUDE.md and the ICP profiles. Document gaps. Share findings with the team.
- [ ] **G2/Clutch/Capterra listings audit.** Check whether CXL has current, accurate listings on the main B2B review aggregators. These are high-value citation sources for AI systems. If listings exist, check recency of reviews. If not, create them and run a customer NPS campaign to seed reviews.
- [ ] **Review content types in this document.** Only the course landing page guidelines reflect fully up-to-date thinking. Blog guidelines need a review pass to confirm they match current B2B/AI focus and AEO requirements. Schedule as part of the next content ops review.