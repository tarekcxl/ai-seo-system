# SEO Operations System

AI-powered SEO execution system for analyzing, prioritizing, improving, validating, and managing blog performance using real SEO and performance data.

The system uses modular agents, focused skills, and external workflows to execute SEO operations end-to-end.

---

# Objective

Maximize:
- organic traffic
- search visibility
- AI-search visibility
- conversions

Through:
- SEO analysis
- technical SEO
- competitor analysis
- content strategy
- content creation
- optimization
- evaluation
- execution management

---

# Architecture

- `/agents`
  → self-contained operational agents

- `/skills`
  → focused capabilities used by agents

- `/skills/*/references`
  → optional context loaded only when needed

- `/workflows`
  → external automations, scraped data, drafts, reports

---

# Core Rules

- Always prioritize real data over assumptions
- Avoid generic SEO advice
- Every insight must lead to a clear action
- Do not duplicate agent responsibilities
- Use focused skills instead of broad instructions
- Load only relevant context
- Do not copy competitors — outperform them
- Preserve factual accuracy and credibility
- Optimize for both traditional SEO and AI-search systems

---

# Execution Flow

Default workflow:

1. `seo-analyst`
2. `seo-technical-analyst`
3. `competitor-analyst`
4. `content-strategist`
5. `project-manager`
6. `content-writer`
7. `content-optimizer`
8. `content-evaluator`

Do not skip evaluation when content quality matters.

---

# Agent Responsibilities

## seo-analyst
SEO and performance analysis.

## seo-technical-analyst
Technical SEO audits, crawlability, indexing, rendering, and Core Web Vitals analysis.

## competitor-analyst
SERP, competitor, and content gap analysis.

## content-strategist
Content planning, keyword targeting, and briefs.

## project-manager
Prioritization, backlog management, and execution tracking.

## content-writer
New SEO/AEO/GEO content creation.

## content-optimizer
Content updates, CTR improvements, and optimization.

## content-evaluator
Quality validation, EEAT checks, fact-checking, and tone consistency.

---

# Skill Usage

Agents decide when to use skills.

Skills define how execution happens.

Use the most focused skill possible.

---

# Skills

## seo-data-analysis
Analyze SEO data from GSC, GA4, and Ahrefs to identify ranking, CTR, and traffic opportunities.

## competitor-analysis
Analyze SERPs and competitor content to identify ranking patterns, gaps, and optimization opportunities.

## content-freshness-audit
Audit existing content freshness and determine whether pages need updates based on recency and SEO relevance.

## technical-seo
Audit technical SEO issues affecting crawlability, indexing, rendering, and Core Web Vitals.

## seo-content-strategy
Create SEO content strategies, keyword targeting plans, and actionable content briefs.

## project-management
Prioritize SEO projects and experiments, manage execution plans, and prepare Airtable-ready tracking updates.

## seo-content-writing
Write SEO blog content from briefs and keyword strategy for search-intent-focused content creation.

## content-optimization
Improve existing content for SEO, clarity, structure, and search intent alignment.

## ctr-optimization
Optimize titles and meta descriptions to improve CTR from search results.

## aeo-geo-optimization
Optimize content for AI search systems, answer extraction, and retrieval-friendly formatting.

## seo-quality-check
Evaluate content quality, EEAT, readability, structure, and usefulness before publishing.

## fact-check
Validate factual accuracy, statistics, and claims to reduce hallucinations and credibility risks.

## tone-voice-consistency
Validate tone consistency using reference feedback, tone guidelines, and blog examples.

---

# Workflow Usage

Use `/workflows` for:
- competitor scraping
- Firecrawl extraction
- n8n automations
- external SEO pipelines

Workflows execute tasks.

Agents perform reasoning.

---

# Output Expectations

Prefer:
- concise outputs
- structured tables
- JSON
- Airtable-ready records
- actionable recommendations

Avoid:
- generic explanations
- repetitive summaries
- unnecessary context

---

# Progressive Disclosure

Do not load unnecessary files.

Only load:
- relevant agents
- required skills
- necessary references
- relevant workflows

Focused context improves output quality.