---
name: competitor-analysis
description: Analyze top-ranking competitors for a query to identify patterns, gaps, and opportunities. Use this skill whenever the user wants to understand why competitors rank, what they are doing in common, what is missing from their content, or how to improve an article based on competitor insights. This skill can trigger a workflow to scrape competitor data when needed.
---

# Competitor Analysis

A skill for understanding why competitors rank and how to outperform them.

This skill combines scraped competitor data with structured analysis to generate actionable SEO insights.

---

## What this skill does

Use this skill to:

- analyze top-ranking pages for a query
- identify common patterns across competitors
- detect content gaps
- define differentiation opportunities
- generate a clear action plan to improve content

---

## When to use this skill

Use this skill when the user wants to:

- analyze competitors for a keyword or topic
- understand why other pages rank higher
- compare their article against competitors
- identify what is missing in their content
- improve an article based on competitor insights

---

## Inputs

This skill may receive:

- target query (required)
- target URL (optional but recommended)
- competitor data (optional)

---

## How to work

### Step 1: Retrieve competitor data

If competitor data is not already provided:

- trigger the `/scrape-competitors` command
- provide:
  - target query
  - target URL (if available)

Wait for the workflow output before continuing.

---

### Step 2: Identify patterns

Analyze competitors to find:

- common structure (sections, headings)
- recurring topics and subtopics
- content depth and level of detail
- common formats (guides, lists, comparisons)

Goal:
Understand what is required to compete.

---

### Step 3: Identify gaps

Compare competitors with the target content.

Find:

- missing sections
- weak explanations
- shallow coverage
- missed angles

Goal:
Understand what is preventing better ranking.

---

### Step 4: Define differentiation

Identify how to outperform competitors:

- clearer explanations
- better structure
- more useful examples
- deeper or more focused content

Goal:
Do not copy — improve.

---

### Step 5: Generate action plan

Translate insights into clear actions:

- what to add
- what to improve
- what to restructure

---

## Output structure

Provide:

### Key patterns
What competitors consistently do

### Competitor strengths
What they do well

### Content gaps
What is missing from the target content

### Differentiation opportunities
How to outperform competitors

### Action plan
Clear, prioritized improvements

---

## Core principles

- Focus on WHY competitors rank, not just WHAT they contain
- Do not summarize — analyze
- Do not copy competitors — improve upon them
- Always translate insights into actions

---

## Boundaries

This skill focuses on competitor analysis.

It does not:
- rewrite content
- perform SEO data analysis
- define full content strategy

---

## Working style

Be analytical and focused.

Only surface insights that lead to clear improvements.