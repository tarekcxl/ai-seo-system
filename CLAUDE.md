# Project Overview

This project is an AI-powered SEO execution system designed to analyze, prioritize, improve, validate, and manage blog performance using real data.

It identifies opportunities from GSC, GA4, Ahrefs, SERP data, and competitor analysis workflows, then converts them into actionable outputs such as:

- content updates
- CTR improvements
- new articles
- SEO experiments
- project execution plans

The system is designed as a modular agent-based SEO operations framework.

---

# Objective

Maximize organic traffic, visibility, and conversions by:

- Identifying high-impact SEO opportunities
- Improving existing content
- Creating new content based on real demand
- Increasing CTR from search results
- Ensuring factual accuracy and trustworthiness
- Maintaining consistent tone of voice
- Validating content quality before publishing
- Organizing SEO execution into measurable projects

---

# Architecture

- `/agents` → self-contained agents with execution logic and responsibilities
- `/skills` → focused domain capabilities (analysis, writing, optimization, evaluation, management)
- `/workflows` → external workflows, scraped data, drafts, reports, and automation outputs
- `/skills/*/references` → optional contextual resources loaded only when needed

---

# Core Principles

- Always rely on real data when available
- Prioritize impact over volume
- Avoid generic SEO advice
- Every insight must lead to a clear action
- Strong content is clear, structured, useful, and differentiated
- Do not copy competitors — outperform them
- Accuracy and credibility matter as much as rankings
- Use focused skills instead of overloaded instructions
- Execution should align with SEO strategy

---

# System Workflow (IMPORTANT)

The system follows a structured SEO execution pipeline:

1. `seo-analyst`
   → identifies opportunities using SEO and performance data

2. `competitor-analyst`
   → analyzes SERPs, competitor gaps, and missing opportunities

3. `content-strategist`
   → defines what content should be created, updated, or prioritized

4. `project-manager`
   → prioritizes experiments and organizes execution backlog

5. `content-writer`
   → creates new SEO content from scratch

6. `content-optimizer`
   → improves existing content and CTR performance

7. `content-evaluator`
   → validates quality, accuracy, trustworthiness, and tone consistency

Always follow this sequence when tasks require multiple stages.

Do not skip validation steps unless explicitly unnecessary.

---

# Agent Responsibilities

## seo-analyst
Focus:
- GSC analysis
- GA4 analysis
- Ahrefs analysis
- identifying SEO opportunities
- performance insights

---

## competitor-analyst
Focus:
- SERP analysis
- competitor gap analysis
- identifying missing topics and structures
- triggering competitor scraping workflows

---

## content-strategist
Focus:
- keyword targeting
- search intent
- content briefs
- deciding whether to refresh or create content

---

## project-manager
Focus:
- prioritization
- execution planning
- Airtable-ready project tracking
- backlog management
- experiment organization

---

## content-writer
Focus:
- creating SEO content
- AEO optimization
- GEO optimization
- following tone of voice and content examples

---

## content-optimizer
Focus:
- improving existing pages
- rewriting weak sections
- improving CTR
- updating content using briefs and insights

---

## content-evaluator
Focus:
- quality validation
- EEAT evaluation
- fact-checking
- tone consistency
- identifying hallucinations
- final editorial review

---

# How to Work

## Step 1: Understand the task

Identify:

- the business goal
- the SEO objective
- available inputs
- required outputs
- whether the task is:
  - analysis
  - strategy
  - creation
  - optimization
  - evaluation
  - project management

---

## Step 2: Select the correct agent

Use the most appropriate agent from `/agents`.

Do not mix responsibilities unnecessarily.

Each agent should focus on its defined role.

---

## Step 3: Execute sequentially when needed

For multi-stage tasks:

- pass outputs from one agent to the next
- preserve context between stages
- avoid redoing completed work

Example:

`seo-analyst`
→ `content-strategist`
→ `project-manager`
→ `content-writer`
→ `content-evaluator`

---

## Step 4: Use skills appropriately

Skills define HOW execution happens.

Agents decide WHEN to use them.

Use focused skills instead of broad instructions.

Do not overload a single skill with unrelated responsibilities.

---

## Step 5: Use workflows when required

Use `/workflows` when external automation or data retrieval is needed.

Examples:
- competitor scraping
- Firecrawl extraction
- n8n workflows
- external SEO data pipelines

Treat workflows as execution tools, not reasoning tools.

---

## Step 6: Validate before final output

All high-quality content should go through evaluation before finalization.

Validation includes:

- SEO quality
- search intent alignment
- readability
- differentiation
- EEAT
- factual accuracy
- tone consistency
- hallucination checks

If issues are found:
→ improve content before finalizing.

---

# Skill Usage Guidelines

Use the most relevant skill for the problem.

## Analysis Skills

- `seo-data-analysis`
  → SEO insights from GSC, GA4, Ahrefs

- `competitor-analysis`
  → SERP and competitor gap analysis

- `content-freshness-audit`
  → determines whether content is outdated

---

## Strategy & Management Skills

- `seo-content-strategy`
  → content decisions and briefs

- `project-management`
  → prioritization, backlog management, Airtable-ready execution

---

## Writing & Optimization Skills

- `seo-content-writing`
  → writing SEO content from scratch

- `content-optimization`
  → improving existing content

- `ctr-optimization`
  → optimizing titles and meta descriptions

---

## Evaluation & Quality Skills

- `seo-quality-check`
  → EEAT, structure, readability, usefulness

- `fact-check`
  → validating claims, statistics, and factual accuracy

- `tone-voice-consistency`
  → validating tone consistency using reference feedback

---

# Airtable Project Tracking

The `project-manager` agent and `project-management` skill use a standardized Airtable structure.

Important fields include:

- Page name
- URL
- Status
- Project Type
- Target query
- Funnel stage
- Impressions (90 days)
- Clicks (90 days)
- CTR
- Avg position
- Hypothesis
- Recommended action
- Impact score
- Effort score
- Confidence score
- Urgency score
- Strategic fit score
- Success metric
- Notes

Always preserve field consistency when preparing Airtable-ready outputs.

---

# Output Expectations

- Be concise and specific
- Prefer structured outputs:
  - tables
  - lists
  - JSON
  - Airtable-ready records
- Avoid generic explanations
- Prioritize actionable recommendations
- Clearly explain prioritization logic when managing projects

---

# Progressive Context

Load only the context relevant to the task.

If needed, review:

- `/agents/*`
- `/skills/*`
- `/workflows/*`
- `/skills/*/references/*`

Avoid loading unnecessary references or instructions.

Focused context produces better outputs.