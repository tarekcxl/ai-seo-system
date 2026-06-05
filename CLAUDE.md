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
- reporting
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

- Prioritize real SEO and performance data over assumptions
- Avoid generic SEO advice
- Every insight must lead to a clear action
- Do not duplicate responsibilities across agents
- Use focused skills instead of overloaded instructions
- Load only relevant context
- Preserve factual accuracy and credibility
- Optimize for both traditional SEO and AI-search systems
- Do not copy competitors — identify gaps and outperform them
- Use workflows for execution, not reasoning
- Use references only when they improve output quality

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
9. `reporting-agent`

Do not skip evaluation when content quality matters.

---

# Agent Responsibilities

## seo-analyst
Analyze SEO and performance data to identify opportunities, ranking issues, CTR problems, and growth potential.

## seo-technical-analyst
Audit technical SEO issues affecting crawlability, indexing, rendering, internal linking, structured data, and Core Web Vitals.

## competitor-analyst
Analyze SERPs, competitor content, and content gaps. Trigger scraping workflows when needed.

## content-strategist
Define keyword targeting, search intent alignment, content priorities, and actionable content briefs.

## project-manager
Prioritize SEO projects and experiments, manage execution backlog, and organize Airtable-ready project tracking.

## content-writer
Create new SEO/AEO/GEO content using briefs, references, tone guidelines, and competitor insights.

## content-optimizer
Improve existing content, update weak sections, improve CTR, and optimize pages using briefs and SEO insights.

## content-evaluator
Validate content quality, EEAT, factual accuracy, hallucination risks, and tone consistency before publishing.

## reporting-agent
Generate SEO reports, experiment summaries, stakeholder updates, and performance insights from agent outputs.

---

# Skill Usage

Agents decide WHEN to use skills.

Skills define HOW execution happens.

Use the most focused skill possible.

Do not overload one skill with unrelated responsibilities.

---

# Skills

## seo-data-analysis
Analyze GSC, GA4, Ahrefs, and SEO data to identify ranking, CTR, and traffic opportunities.

## technical-seo
Audit crawlability, indexing, rendering, Core Web Vitals, and technical SEO issues.

## competitor-analysis
Analyze SERPs and competitor content to identify ranking patterns, gaps, and optimization opportunities.

## content-freshness-audit
Determine whether content is outdated and requires refreshing based on SEO relevance and recency.

## seo-content-strategy
Create keyword targeting plans, content priorities, and actionable SEO content briefs.

## project-management
Prioritize SEO projects and experiments, organize execution plans, and prepare Airtable-ready tracking updates.

## seo-content-writing
Write SEO/AEO/GEO blog content from briefs, keyword strategy, and reference materials.

## content-optimization
Improve existing content for clarity, structure, usefulness, rankings, and intent alignment.

## ctr-optimization
Optimize titles and meta descriptions using SERP analysis to improve CTR and differentiation.

## aeo-geo-optimization
Optimize content for AI-search systems, answer extraction, retrieval, and AI-generated summaries.

## seo-quality-check
Evaluate readability, EEAT, structure, usefulness, and overall SEO quality before publishing.

## fact-check
Validate claims, statistics, references, and factual accuracy to reduce hallucinations and credibility risks.

## tone-voice-consistency
Validate tone consistency using reference feedback, tone-of-voice guidelines, and blog examples.

## seo-reporting
Generate SEO reports, experiment summaries, stakeholder updates, and performance insights from agent outputs.

---

# Workflow Usage

Use `/workflows` for:
- competitor scraping
- Firecrawl extraction
- n8n automations
- external SEO pipelines
- Airtable updates
- report generation

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

For large or specialized tasks:
- use `/skills/*/references`
- load only the references relevant to the task
- avoid deep reference chains

---

# Quality Validation

High-quality outputs should validate:

- search intent alignment
- SEO quality
- readability
- differentiation
- EEAT
- factual accuracy
- tone consistency
- AI-search friendliness

If quality issues are detected:
→ improve content before finalizing.

---

# Reporting Rules

Reports should:
- focus on actionable insights
- prioritize business impact
- summarize execution status clearly
- avoid vanity metrics
- explain what changed, why it matters, and what happens next

Prefer:
- summaries
- trends
- prioritized recommendations
- experiment outcomes
- stakeholder-friendly formatting

---

# Context Efficiency

Keep reasoning focused.

Avoid:
- loading unrelated skills
- repeating instructions
- unnecessary verbosity
- generic SEO explanations

Use progressive disclosure whenever possible.

Load detailed references only when required for the task.