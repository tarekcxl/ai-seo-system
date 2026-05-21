---
name: seo-reporting
description: Generate SEO performance reports using GSC, GA4, and SEO data to monitor trends, wins, losses, and performance changes.
---

# SEO Reporting

A skill for generating recurring SEO performance reports using Google Search Console, GA4, and SEO datasets.

This skill focuses on:

- performance monitoring
- week-over-week reporting
- identifying trends
- highlighting wins and losses
- surfacing opportunities and risks
- turning SEO data into actionable summaries

This skill is designed for reporting and monitoring.

It is NOT the primary skill for:
- deep SEO analysis
- diagnosing ranking bottlenecks
- identifying strategic SEO opportunities

The `seo-data-analysis` skill remains the primary analysis skill for:
- opportunity discovery
- bottleneck analysis
- ranking diagnostics
- SEO strategy insights

---

## What this skill does

Use this skill to:

- generate weekly SEO reports
- compare SEO performance periods
- monitor traffic and visibility trends
- identify ranking improvements or declines
- surface CTR opportunities
- identify content performance changes
- summarize SEO performance clearly
- provide actionable reporting summaries

---

## When to use this skill

Use this skill when:

- the user wants weekly SEO reporting
- performance needs monitoring
- traffic changes need explanation
- rankings improved or dropped
- leadership needs SEO summaries
- stakeholders need updates
- reporting automation is required

Trigger when the user says things like:

- “generate weekly SEO report”
- “compare this week vs last week”
- “show SEO performance changes”
- “what improved this week?”
- “what declined?”
- “monitor SEO performance”
- “create SEO dashboard summary”

For deeper opportunity analysis or SEO diagnostics:
→ use `seo-data-analysis`.

---

## Core principles

- focus on trends, not raw data dumps
- explain what changed and why it matters
- prioritize actionable insights
- surface opportunities and risks
- make reports easy to scan
- connect metrics to business impact

---

## Reporting metrics

Prioritize:

### Google Search Console
- clicks
- impressions
- CTR
- average position
- top gaining pages
- top declining pages
- query trends

---

### GA4
- organic sessions
- conversions
- engagement
- bounce/engagement trends
- landing page performance

---

### SEO insights
- ranking movement
- CTR opportunities
- content decay
- emerging opportunities
- technical SEO impact

---

## Weekly comparison logic

Compare:

- current week
vs
- previous week

Highlight:

- traffic increases
- traffic declines
- ranking improvements
- CTR changes
- new opportunities
- unusual changes

Focus on meaningful deltas.

Avoid reporting noise.

---

## Important limitation

This skill surfaces:
- trends
- patterns
- anomalies

But it should NOT attempt to perform:
- full root-cause analysis
- advanced SEO diagnostics
- deep opportunity prioritization

If deeper investigation is required:
→ escalate to `seo-data-analysis`.

---

## Output structure

# SEO Weekly Report

## Executive Summary
High-level overview of SEO performance.

---

## KPI Overview

| Metric | Current Week | Previous Week | Change |
|---|---|---|---|

Include:
- clicks
- impressions
- CTR
- average position
- organic sessions
- conversions

---

## Top Wins

Highlight:
- improving pages
- growing queries
- CTR improvements
- ranking gains

---

## Top Risks

Highlight:
- declining pages
- ranking drops
- traffic losses
- CTR declines

---

## Opportunities

Identify:
- high-impression low-CTR pages
- content refresh candidates
- new keyword opportunities
- technical issues

---

## Recommended Actions

Prioritized next steps.

Focus on:
- highest-impact actions
- quick wins
- strategic improvements

Recommend escalation to:
- `seo-analyst`
when deeper analysis is needed.

---

## Output quality bar

Strong output:
- identifies meaningful trends
- explains impact clearly
- surfaces actionable insights
- prioritizes actions
- is easy to understand quickly

Weak output:
- dumps raw metrics
- lacks prioritization
- gives generic insights
- ignores important changes
- lacks recommendations

---

## Boundaries

This skill focuses on reporting and monitoring.

It does not:
- rewrite content
- perform deep competitor analysis
- execute technical fixes
- create full content strategies
- replace `seo-data-analysis`

Use:
- `seo-data-analysis`
- `content-optimization`
- `technical-seo`
- `seo-content-strategy`

when deeper execution is required.

---

## Working style

Think like an SEO lead reporting to stakeholders.

Focus on:
- what changed
- why it matters
- what should happen next

Avoid turning reporting into full SEO consulting.