---
name: seo-data-analysis
description: Analyze SEO performance data to identify ranking opportunities, CTR issues, declining pages, and content gaps using sources like Google Search Console, GA4, Ahrefs, and related SEO datasets. Use this skill whenever the user wants to audit blog or page performance, find SEO opportunities, prioritize what to update, interpret GSC or GA4 data, understand why pages are underperforming, or decide what content to create or refresh based on search performance.
---

# SEO Data Analysis

A skill for turning SEO performance data into clear, prioritized actions.

Use this skill when the task is not just to read data, but to interpret it and decide what matters most. The goal is to find pages and queries with meaningful growth potential and translate the data into specific SEO actions.

## What this skill does

This skill helps you:

- analyze SEO performance data from Google Search Console, GA4, Ahrefs, and similar sources
- identify high-potential opportunities such as:
  - high impressions + low CTR
  - rankings in positions 5–20
  - declining clicks or impressions
  - pages with traffic but weak engagement or conversion signals
- distinguish between different opportunity types:
  - CTR improvement
  - ranking improvement
  - content refresh
  - net-new content opportunity
- prioritize actions based on likely impact, not just surface-level metrics

## When to use this skill

Use this skill when the user wants to:

- audit blog or landing page SEO performance
- understand what to update first
- identify pages in striking distance
- find pages with strong impressions but weak CTR
- interpret Google Search Console or GA4 data
- compare performance across pages, queries, or time periods
- identify declining content performance
- decide whether to refresh, expand, merge, or create content
- turn SEO data into a prioritized action plan

This skill should also trigger when the user shares spreadsheets, tables, exports, CSVs, or screenshots related to SEO performance and asks what stands out, what to fix, or where the opportunities are.

## Core principles

- Use real data. Do not guess when metrics are available.
- Prioritize impact over activity. Focus on what can move traffic, rankings, or conversions.
- Avoid generic SEO advice. Every recommendation should be tied to observed data.
- Treat SEO analysis as decision-making, not reporting.
- A metric only matters if it leads to a clear interpretation and action.

## Inputs

Typical inputs include:

- Google Search Console exports
  - query
  - page
  - clicks
  - impressions
  - CTR
  - average position
- GA4 exports
  - sessions
  - engagement rate
  - conversions
  - bounce-related indicators
  - landing page performance
- Ahrefs or keyword tools
  - keyword difficulty
  - SERP overview
  - backlinks
  - competing pages
- scraped or structured SEO datasets from workflows
- user-provided thresholds or business context

If the input is incomplete, work with what is available and clearly state the limits.

## How to think about the analysis

Do not just summarize metrics. Look for patterns that imply opportunity.

### 1. CTR opportunity
Look for pages or queries with:

- high impressions
- lower-than-expected CTR
- rankings already near page one or mid-page one

Interpretation:
- the page is being seen but not chosen often enough
- the issue may be title, meta description, SERP positioning, intent mismatch, or weak framing

Typical action:
- improve title and meta angle
- align copy more tightly with search intent
- strengthen the promise or differentiation in the snippet and intro

### 2. Ranking opportunity
Look for:

- average positions between 5 and 20
- meaningful impressions
- signs the page is already relevant but not yet competitive enough

Interpretation:
- the page has earned relevance but needs improvement to move higher

Typical action:
- refresh or expand content
- improve structure and topical coverage
- strengthen internal linking
- improve clarity, examples, or depth

### 3. Declining performance
Look for:

- clicks or impressions trending down
- formerly strong pages losing visibility
- drops across important queries

Interpretation:
- competitors may be overtaking the page
- content may be aging, losing relevance, or missing newer expectations

Typical action:
- refresh content
- re-evaluate search intent fit
- compare against current top-ranking competitors

### 4. Content gap opportunity
Look for:

- queries appearing in GSC that are only weakly addressed
- pages ranking for adjacent terms without dedicated coverage
- strong topical demand without a strong matching asset

Interpretation:
- the site may need a new section, subtopic, or net-new article

Typical action:
- expand the existing page if intent is close
- create a new page if intent is distinct

### 5. Conversion or engagement mismatch
Look for:

- pages with strong search visibility but weak downstream behavior
- traffic that does not engage, convert, or continue deeper into the site

Interpretation:
- the traffic may be low quality, or the page may satisfy search partially but fail as an experience

Typical action:
- improve page structure, messaging, CTAs, or next-step clarity
- check whether the query intent matches the page’s actual purpose

## Prioritization framework

When multiple opportunities exist, prioritize based on this order:

### High priority
- high impressions
- positions 5–20
- low CTR on important queries
- strong business relevance
- pages already close to winning

### Medium priority
- moderate impressions with clear upside
- declining pages that were previously valuable
- pages with visible intent mismatch but fixable structure

### Lower priority
- very low-impression opportunities
- pages with weak relevance and little evidence of upside
- pages requiring major rebuilds with uncertain value

When possible, weigh:

1. traffic potential
2. likelihood of improvement
3. business value
4. effort required

## Decision framework

Use this logic when recommending next actions:

### Recommend CTR optimization when:
- impressions are high
- rankings are already fairly strong
- the main issue is under-clicking rather than invisibility

### Recommend content refresh when:
- the page ranks but not strongly enough
- competitors likely offer better depth, structure, or freshness
- impressions show meaningful demand

### Recommend net-new content when:
- the topic has demand
- the current page only partially addresses the query
- search intent deserves its own dedicated asset

### Recommend deeper review when:
- metrics conflict
- performance changed sharply
- the cause is not obvious from the available dataset

## Output guidelines

Your output should help the user decide what to do next.

Prefer structured outputs such as:

- prioritized opportunity tables
- grouped findings by opportunity type
- concise action plans
- JSON when the surrounding workflow requires it

Keep the output specific. Tie every recommendation to evidence in the data.

## Recommended output structure

When the user asks for opportunity analysis, use a structure like this:

### Summary
- what stands out overall
- where the biggest upside is
- what should be prioritized first

### Opportunities
For each opportunity include:

- page URL
- query or keyword
- clicks
- impressions
- CTR
- average position
- opportunity type
- why it matters
- recommended action

### Prioritized next steps
List the top actions in order of likely impact.

## Example opportunity labels

Use labels like:

- CTR improvement
- Ranking improvement
- Content refresh
- Content gap
- New content opportunity
- Intent mismatch
- Declining page

## Analysis quality bar

A strong analysis does all of the following:

- identifies real opportunities, not just interesting metrics
- explains why the opportunity exists
- distinguishes visibility issues from click issues
- distinguishes ranking issues from content coverage issues
- recommends actions that fit the evidence
- helps the user prioritize confidently

A weak analysis:

- repeats the data without interpretation
- gives generic SEO advice
- treats every page as equally important
- recommends changes without linking them to metrics

## Boundaries

This skill is for SEO data interpretation and prioritization.

It is not the place to do deep competitor teardown, full article rewriting, or final copy refinement unless the user explicitly combines those tasks. In those cases, this skill should still do the performance diagnosis first, then hand off conceptually to the relevant agent or skill.

## Working style

Be concise, analytical, and practical.

Do not overwhelm the user with every possible observation. Surface the highest-value patterns first. A useful SEO analysis should reduce noise and increase clarity.