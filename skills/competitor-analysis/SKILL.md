---
name: competitor-analysis
description: Analyze top-ranking competitors to identify SERP patterns, content gaps, and optimization opportunities. Use this skill when the user wants to improve existing content, generate SEO briefs, or understand why competitors rank higher.
---

# Competitor Analysis

Analyze competitors to understand why they rank and how to outperform them.

---

## What this skill does

Use this skill to:

- analyze top-ranking pages
- identify SERP patterns
- compare competitor content against a target article
- identify content gaps
- generate SEO briefs
- support content refresh workflows

---

## Inputs

This skill may receive:

- target query (required)
- target URL (recommended)

---

## Tools

Use:

- Search API
  → retrieve top organic SERP results

- Firecrawl
  → scrape competitor pages and the target article

---

## Workflow

### Step 1: Search the SERP

Search Google for the target query.

Collect:
- top 5 organic results
- titles
- URLs

Ignore:
- ads
- irrelevant pages

---

### Step 2: Scrape content

Use Firecrawl to scrape:
- top 5 competitor pages
- the target article (if provided)

Save outputs to: /workflows/scraped-blogs/

---

### Step 3: Analyze competitors

Identify:

- common sections and structure
- recurring topics
- search intent patterns
- content depth
- formatting patterns
- EEAT signals
- differentiation opportunities

Goal:
Understand what Google expects for this query.

---

### Step 4: Compare against target content

Find:
- missing sections
- weak coverage
- outdated information
- poor structure
- weak intent alignment
- lack of differentiation

Focus only on meaningful gaps.

---

### Step 5: Generate SEO brief

Generate a concise SEO brief containing:

- target query
- search intent
- recommended angle
- suggested structure
- missing sections
- optimization opportunities
- differentiation ideas
- CTR opportunities
- EEAT recommendations

Save brief to:/workflows/seo-briefs/


---

### Step 6: Support execution

The generated brief can be used by:

- `content-writer`
- `content-optimizer`
- `content-evaluator`

---

## Output structure

### SERP patterns
What top-ranking pages consistently do

### Content gaps
What is missing from the target article

### Differentiation opportunities
How to outperform competitors

### Recommended structure
Suggested sections and hierarchy

### SEO brief summary
High-level overview of the generated brief

### Recommended next actions
What should happen next

---

## Core principles

- Analyze, don’t summarize
- Focus on why competitors rank
- Do not copy competitors
- Every insight should lead to an action

---

## Boundaries

This skill:
- analyzes competitors
- identifies gaps
- generates SEO briefs

This skill does NOT:
- rewrite full content
- perform deep SEO data analysis
- directly optimize content

---

## Working style

Be analytical, concise, and action-oriented.

Only surface insights that lead to meaningful improvements.