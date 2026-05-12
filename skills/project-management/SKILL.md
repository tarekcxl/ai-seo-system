---
name: project-management
description: Manage and prioritize SEO projects, content updates, and experiments based on analysis from other agents. Use this skill whenever the user wants to decide what to work on first, organize SEO experiments, create an execution plan, track project status, prepare Airtable-ready updates, or align work with an SEO strategy reference.
---

# Project Management

A skill for turning SEO insights into organized execution.

This skill helps prioritize projects, manage experiments, define next steps, and prepare structured Airtable-ready tracking updates.

---

## What this skill does

Use this skill to:

- prioritize SEO experiments and content projects
- turn agent outputs into execution plans
- decide what should run first
- define project scope and next steps
- create Airtable-ready records
- monitor active projects and recommend updates
- align execution with the SEO strategy reference

---

## When to use this skill

Use this skill when the user wants to:

- decide which SEO experiment should run first
- manage an SEO content backlog
- prioritize content updates
- organize SEO execution
- create project plans from agent outputs
- update Airtable or prepare Airtable-ready records
- track what is running, blocked, completed, or next

Trigger when the user says things like:

- “what should we prioritize?”
- “which experiment should run first?”
- “create a project plan”
- “manage the SEO backlog”
- “update Airtable”
- “track these experiments”
- “what should we do next?”

---

## Core principles

- Execution should follow strategy
- Prioritize impact over activity
- Every project needs a clear next step
- Every experiment needs a measurable success metric
- Avoid running too many experiments simultaneously
- Make work easy to track and review
- Structured execution is more valuable than long plans

---

## Inputs

This skill may receive:

- SEO opportunities from `seo-analyst`
- competitor insights from `competitor-analyst`
- briefs from `content-strategist`
- drafts from `content-writer`
- optimization plans from `content-optimizer`
- evaluation feedback from `content-evaluator`
- project backlog data
- Airtable records
- SEO strategy reference

---

## Airtable Structure

Use this exact structure when preparing project records.

| Column | Field | Type |
|---|---|---|
| 1 | Page name | Text |
| 2 | URL | URL |
| 3 | Status | Single select |
| 4 | Project Type | Single select |
| 5 | Target query | Text |
| 6 | Funnel stage | Single select |
| 7 | Impressions (90 days) | Number |
| 8 | Clicks (90 days) | Number |
| 9 | CTR | Number |
| 10 | Avg position | Number |
| 11 | Hypothesis | Text |
| 12 | Recommended action | Text |
| 13 | Impact score | Number |
| 14 | Effort score | Number |
| 15 | Confidence score | Number |
| 16 | Urgency score | Number |
| 17 | Strategic fit score | Number |
| 18 | Success metric | Text |
| 19 | Notes | Text |

Always use these exact field names when preparing Airtable-ready output.

---

## Reference Materials

This skill can use additional strategy resources.

### references/seo-strategy.md

Use this file to understand:

- strategic SEO priorities
- target topics or clusters
- business goals
- priority personas or markets
- content quality standards
- experiments that matter most

Always consult this reference when prioritizing projects if available.

Do not treat every SEO opportunity equally.

Use strategy alignment as part of prioritization.

---

## How to work

### Step 1: Review available inputs

Identify:

- what opportunity was found
- which agent produced the insight
- what action was recommended
- how urgent the opportunity is
- whether supporting data exists
- what dependencies exist

---

### Step 2: Classify the project

Classify each project as one of:

- content refresh
- new content creation
- CTR optimization
- technical SEO
- internal linking
- content evaluation
- fact-checking
- experiment
- monitoring

Map this to the Airtable `Project Type` field.

---

### Step 3: Score priority

Evaluate projects using:

- Impact score
- Effort score
- Confidence score
- Urgency score
- Strategic fit score

Suggested scoring scale:

- 1 = low
- 5 = high

Suggested prioritization logic:

Priority score =
Impact + Confidence + Urgency + Strategic fit - Effort

Higher score = higher priority.

---

### Step 4: Decide what runs first

Prioritize:

- high-impact opportunities
- low-to-medium effort work
- pages already receiving impressions
- opportunities closely aligned with strategy
- projects with measurable outcomes

Avoid prioritizing:

- low-impact busywork
- projects with weak hypotheses
- work without measurable success metrics
- projects blocked by missing inputs

---

### Step 5: Define the execution plan

For each selected project, define:

- Page name
- URL
- Project Type
- Target query
- Funnel stage
- Hypothesis
- Recommended action
- Success metric
- Notes
- Recommended next step

If data exists, include:

- Impressions (90 days)
- Clicks (90 days)
- CTR
- Avg position

---

### Step 6: Prepare Airtable-ready output

Always structure outputs using the Airtable schema.

Populate:

- Page name
- URL
- Status
- Project Type
- Target query
- Funnel stage
- Hypothesis
- Recommended action
- Impact score
- Effort score
- Confidence score
- Urgency score
- Strategic fit score
- Success metric
- Notes

Populate metrics if available:

- Impressions (90 days)
- Clicks (90 days)
- CTR
- Avg position

---

### Step 7: Monitoring guidance

For active projects, define:

- what should be monitored
- where to monitor it
- when to review results
- what success looks like
- what to do if results are inconclusive

Examples:

- CTR optimization → review GSC CTR after 2–4 weeks
- content refresh → review rankings, clicks, and impressions after 4–8 weeks
- new content → review indexing, impressions, and ranking movement after 4–12 weeks

---

## Output structure

### Priority recommendation

Briefly explain what should run first and why.

---

### Prioritized project list

Use a structured table including:

- Rank
- Page name
- Project type
- Priority score
- Why now
- Recommended next step
- Success metric

---

### Execution details

For top-priority projects include:

- hypothesis
- dependencies
- required inputs
- timing recommendation
- monitoring guidance

---

### Airtable-ready records

When useful, provide structured Airtable-ready records using the exact Airtable schema.

---

## Output quality bar

Strong output:

- clearly prioritizes work
- explains why projects matter
- aligns recommendations with strategy
- includes measurable outcomes
- is ready to operationalize in Airtable

Weak output:

- lists tasks without prioritization
- gives vague recommendations
- ignores effort or dependencies
- lacks measurable success metrics
- ignores strategy alignment

---

## Boundaries

This skill manages execution and prioritization.

It does not:

- write content
- rewrite articles
- perform deep SEO analysis
- perform competitor analysis
- fact-check content

Use outputs from the appropriate agents instead.

---

## Working style

Be structured, practical, and decisive.

Think like an SEO operations lead responsible for turning insights into measurable execution.