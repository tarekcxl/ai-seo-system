---
name: seo-technical-analysis
description: Analyze websites for technical SEO issues including crawlability, indexability, Core Web Vitals, structured data, and rendering. Use this skill whenever the user wants to audit a site’s technical SEO, diagnose ranking issues, or identify technical improvements.
---

# Technical SEO Analysis

A skill for auditing and diagnosing technical SEO performance across websites.

This skill evaluates how well a website can be crawled, indexed, and rendered, and identifies issues that may impact rankings.

---

## What this skill does

Use this skill to:

- analyze crawlability and indexability
- check robots.txt and sitemap configuration
- evaluate meta tags and canonical tags
- assess URL structure and redirects
- detect technical SEO issues
- identify Core Web Vitals risks
- analyze JavaScript rendering impact

---

## When to use this skill

Use this skill when the user wants to:

- perform a technical SEO audit
- diagnose ranking issues
- check if pages can be crawled and indexed
- evaluate site performance and structure
- identify technical improvements

---

## Inputs

This skill may receive:

- a URL or list of URLs
- domain
- HTML source (optional)
- crawl data (optional)

---

## Data Retrieval

To analyze pages effectively, you may need to retrieve HTML content.

If raw HTML or page data is not provided:

- use available tools (e.g. Firecrawl) to fetch:
  - full HTML source
  - metadata
  - rendered content (if needed)

Prefer tools that return structured output when possible.

Do not rely on partial or incomplete page data when performing technical analysis.

---

## How to work

### Step 1: Retrieve and inspect page data

If page content is not provided:

- fetch the page using available tools (e.g. Firecrawl)
- retrieve:
  - raw HTML
  - metadata
  - rendered content if needed

Use this data as the basis for all technical analysis.

Do not proceed with assumptions if the page cannot be properly inspected.

---

### Step 2: Analyze crawlability

Check:

- robots.txt accessibility
- sitemap availability
- blocked resources
- noindex directives

---

### Step 3: Analyze indexability

Check:

- canonical tags
- duplicate content signals
- thin content risks
- indexation signals

---

### Step 4: Analyze on-page technical signals

Check:

- meta tags (title, description, robots)
- canonical consistency
- structured data presence

---

### Step 5: Analyze URL structure

Check:

- clean, readable URLs
- redirect chains
- unnecessary parameters

---

### Step 6: Analyze security

Check:

- HTTPS usage
- security headers (if detectable)

---

### Step 7: Analyze Core Web Vitals (heuristics)

Evaluate potential risks:

- LCP issues (large images, slow loading elements)
- INP issues (heavy JavaScript, blocking scripts)
- CLS issues (layout shifts, missing dimensions)

**Reference thresholds:**
- LCP: Good <2.5s
- INP: Good <200ms
- CLS: Good <0.1

Do not reference FID.

---

### Step 8: Analyze mobile experience

Check:

- viewport configuration
- responsive design signals
- touch usability indicators

---

### Step 9: Analyze JavaScript rendering

Check:

- reliance on client-side rendering
- missing content in raw HTML
- delayed content loading

---

### Step 10: IndexNow (optional)

Check if IndexNow is implemented or recommended.

---

## Output structure

Provide:

### Technical score (0–100)

---

### Category breakdown

For each category:
- status (Pass / Warning / Fail)
- key issues

---

### Prioritized issues

Group by:

- Critical
- High
- Medium
- Low

---

### Recommendations

Provide:

- specific fixes
- implementation guidance

---

## Core principles

- Focus on issues that impact crawlability and rankings
- Prioritize high-impact fixes
- Avoid generic advice
- Be precise and actionable

---

## Boundaries

This skill analyzes technical SEO.

It does not:
- perform content optimization
- write content
- define content strategy

---

## Working style

Be structured and analytical.

Focus on identifying real issues that impact performance.