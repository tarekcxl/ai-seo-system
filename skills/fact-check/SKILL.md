---
name: fact-check
description: Verify factual accuracy, claims, statistics, dates, tools, and references within content to reduce hallucinations and misinformation. Use this skill whenever reviewing AI-generated content, validating blog articles, checking data accuracy, or ensuring statements align with real-world facts and current information.
---

# Fact Check

A skill for validating factual accuracy and reducing hallucinations in written content.

This skill reviews content to ensure that claims, statistics, dates, references, tools, and explanations are accurate, current, and trustworthy.

---

## What this skill does

Use this skill to:

- verify factual claims
- validate statistics and numbers
- confirm dates, timelines, and references
- check tools, platforms, and product information
- identify hallucinations or misleading statements
- flag uncertain or unverifiable claims

---

## When to use this skill

Use this skill when:

- reviewing AI-generated content
- validating SEO articles before publishing
- checking statistics or factual claims
- ensuring content accuracy
- auditing trustworthiness and reliability

Trigger when the user says things like:
- “fact check this”
- “verify the data”
- “make sure this is accurate”
- “check for hallucinations”
- “validate these claims”

---

## Core principles

- Accuracy is more important than sounding confident
- Unverified claims should be flagged
- Do not assume information is correct because it sounds plausible
- Prioritize trustworthy and current information
- If confidence is low, explicitly state uncertainty

---

## Inputs

This skill may receive:

- full article content
- sections of content
- claims, statistics, or references
- URLs or sources (optional)

---

## How to work

### Step 1: Identify factual claims

Extract and review:

- statistics
- percentages
- timelines
- product or tool capabilities
- SEO or marketing claims
- references to studies or reports
- statements presented as facts

---

### Step 2: Validate accuracy

Check whether:

- the information is factually correct
- the data is current
- the statement aligns with known best practices
- the claim is exaggerated or misleading

---

### Step 3: Identify hallucinations

Flag:

- fabricated statistics
- invented studies or references
- unsupported claims
- incorrect dates or timelines
- inaccurate product or feature descriptions

---

### Step 4: Assess confidence level

Classify findings as:

- verified
- likely accurate
- uncertain
- inaccurate

If uncertain:
- explain why
- recommend verification before publishing

---

### Step 5: Recommend corrections

For inaccurate or weak claims:

- suggest corrected wording
- recommend removing unsupported claims
- simplify overly confident statements

---

## Output structure

### Verified claims
Claims that appear accurate and trustworthy

---

### Questionable or inaccurate claims
Claims that may be incorrect, outdated, or unsupported

---

### Hallucination risks
Potential fabricated or misleading information

---

### Recommended corrections
Specific suggestions to improve accuracy

---

### Confidence assessment
Overall confidence level:
- high
- medium
- low

---

## Fact-checking guidelines

### Statistics
- ensure numbers are realistic and current
- avoid unsupported percentages or metrics

---

### SEO / marketing claims
- avoid absolute statements (“guaranteed rankings”)
- ensure advice reflects modern best practices

---

### Tool and platform references
- confirm features and capabilities are real
- avoid outdated functionality descriptions

---

### Dates and trends
- ensure trends and references are current
- flag outdated recommendations

---

## Output quality bar

Strong output:
- identifies real inaccuracies
- explains why claims are problematic
- improves trustworthiness

Weak output:
- accepts claims without validation
- ignores uncertainty
- gives vague feedback

---

## Boundaries

This skill validates accuracy and credibility.

It does not:
- rewrite full content
- define strategy
- optimize for SEO performance

---

## Working style

Be skeptical, precise, and evidence-oriented.

When uncertain, clearly communicate uncertainty instead of assuming accuracy.