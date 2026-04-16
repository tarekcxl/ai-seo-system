# Project Overview

This project is an AI-powered SEO execution system designed to analyze, prioritize, and improve blog performance using real data.

It identifies opportunities from GSC, GA4, Ahrefs, and SERP data and converts them into actionable outputs such as content updates and new articles.

---

# Objective

Maximize organic traffic and conversions by:

- Identifying high-impact opportunities
- Improving existing content
- Creating new content based on real demand
- Ensuring content quality and competitiveness before publishing

---

# Architecture

- /agents → self-contained agents with roles and execution logic
- /skills → domain-specific capabilities (analysis, writing, optimization, evaluation)
- /workflows → inputs and outputs (data, scraped content, drafts, external workflows)

---

# Core Principles

- Always rely on real data when available
- Prioritize impact over volume
- Avoid generic SEO advice
- Every insight must lead to a clear action
- Strong content is clear, structured, and useful
- Do not copy competitors — outperform them

---

# System Workflow (IMPORTANT)

The system follows a structured pipeline:

1. seo-analyst → identifies opportunities from data
2. competitor-analyst → explains why competitors rank and what is missing
3. content-strategist → defines what content to create or update
4. content-writer → creates new content from scratch
5. content-optimizer → improves existing content and CTR
6. content-evaluator → validates quality before final output

Always follow this sequence when tasks require multiple steps.

Do not skip steps unless explicitly unnecessary.

---

# How to Work

### Step 1: Understand the task
- Identify the goal (analysis, creation, optimization, evaluation)
- Identify available inputs (data, briefs, URLs)

---

### Step 2: Select the appropriate agent
- Use agents from `/agents`
- Each agent has a clearly defined responsibility
- Do not mix responsibilities across agents

---

### Step 3: Execute sequentially when needed
- If a task requires multiple stages, chain agents together
- Ensure outputs from one agent become inputs for the next

---

### Step 4: Use skills appropriately
- Skills define HOW tasks are executed
- Agents decide WHEN to use them
- Use the most relevant skill for the problem
- Do not force skills unnecessarily

---

### Step 5: Use workflows when required
- Use `/workflows` when external data or automation is needed
- Example: competitor scraping via n8n
- Treat workflows as execution tools, not reasoning tools

---

### Step 6: Validate before final output
- Use evaluation (content-evaluator) when quality matters
- Ensure content is:
  - aligned with intent
  - competitive
  - clear and useful

---

# Agent Guidelines

- Each agent is self-contained with its own logic
- Do not duplicate responsibilities across agents
- Keep roles clearly separated:
  - analyst = data
  - strategist = decisions
  - writer = creation
  - optimizer = improvement
  - evaluator = validation

---

# Skill Usage Guidelines

- Skills are specialized capabilities (e.g. SEO analysis, writing, CTR optimization)
- Use skills based on the problem:
  - seo-data-analysis → data insights
  - competitor-analysis → SERP and content gaps
  - seo-content-strategy → content decisions and briefs
  - seo-content-writing → content creation
  - content-optimization → content improvement
  - ctr-optimization → titles and meta optimization
  - seo-quality-check → EEAT, clarity, structure
- Do not overload a single skill with multiple responsibilities
- Prefer focused, high-impact usage

---

# Quality & Evaluation (CRITICAL)

All content should be validated before final output when quality matters.

Check for:

- search intent alignment
- clarity and usefulness
- structure and readability
- differentiation vs competitors
- credibility (EEAT signals)

If issues are found:
→ improve content before finalizing

---

# Output Expectations

- Be concise and specific
- Prefer structured outputs (tables, lists, or JSON)
- Avoid generic explanations
- Always tie outputs to actionable improvements

---

# Progressive Context

If needed, review:

- /agents/*
- /skills/*
- /workflows/*

Load only what is relevant to the task to avoid unnecessary context.