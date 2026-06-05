# SEO Operations System

AI-powered modular SEO operations system built around specialized agents, focused skills, and reusable workflows to scale SEO analysis, content strategy, technical SEO, optimization, evaluation, project management, and reporting.

The system transforms SEO data, competitor insights, and performance opportunities into structured execution workflows and measurable SEO growth.

---

## What It Does

* Analyzes SEO performance using:

  * GSC
  * GA4
  * Ahrefs
  * SERP data

* Performs:

  * technical SEO audits
  * competitor analysis
  * keyword research
  * content strategy
  * content optimization
  * CTR optimization
  * content freshness audits
  * fact-checking
  * quality validation

* Creates:

  * SEO content briefs
  * SEO articles
  * optimization plans
  * project execution plans
  * Airtable-ready project tracking

---

## Architecture

```bash
/agents
  → orchestration and decision-making

/skills
  → focused execution capabilities

/skills/*/references
  → examples, frameworks, tone references

/workflows
  → reports, drafts, scraped data, exports
```

---

## Agents

| Agent                 | Purpose                                 |
| --------------------- | --------------------------------------- |
| seo-analyst           | SEO and performance analysis            |
| seo-technical-analyst | Technical SEO auditing                  |
| competitor-analyst    | SERP and competitor analysis            |
| content-strategist    | SEO briefs and strategy                 |
| project-manager       | Prioritization and execution management |
| content-writer        | SEO/AEO/GEO content creation            |
| content-optimizer     | Content and CTR optimization            |
| content-evaluator     | Quality validation and EEAT review      |

---

## Skills

| Skill                   | Purpose                               |
| ----------------------- | ------------------------------------- |
| seo-data-analysis       | SEO performance analysis              |
| competitor-analysis     | SERP and competitor analysis          |
| content-freshness-audit | Detect outdated content               |
| technical-seo           | Technical SEO auditing                |
| seo-content-strategy    | Content planning and briefs           |
| project-management      | Prioritization and Airtable tracking  |
| seo-content-writing     | SEO/AEO/GEO article writing           |
| content-optimization    | Existing content improvements         |
| ctr-optimization        | Title and meta optimization           |
| aeo-geo-optimization    | AI-search and answer optimization     |
| seo-quality-check       | EEAT and quality validation           |
| fact-check              | Accuracy and hallucination validation |
| tone-voice-consistency  | Tone consistency validation           |

---

## Example Workflow

```text
SEO Analysis
    ↓
Technical SEO Audit
    ↓
Competitor Analysis
    ↓
Content Strategy
    ↓
Project Prioritization
    ↓
Content Writing
    ↓
Content Optimization
    ↓
Quality Evaluation
```

---

## Core Principles

* modular agents over giant prompts
* focused skills over overloaded instructions
* progressive disclosure
* real data over assumptions
* actionable outputs over generic advice
* reusable workflows
* structured execution
* SEO + AI-search optimization

---

## Output Style

Prefer:

* concise outputs
* structured tables
* actionable recommendations
* Airtable-ready records
* execution-focused deliverables

Avoid:

* generic SEO advice
* repetitive summaries
* unnecessary context
* bloated prompts

---

## Workflow Usage

Use `/workflows` for:

* scraped competitor data
* reports
* exports
* optimization outputs
* SEO audits
* content drafts
* automation outputs

---

## Philosophy

The goal is not to generate random SEO recommendations.

The goal is to identify, prioritize, execute, validate, and scale SEO operations using real performance data, modular agents, and reusable workflows.
