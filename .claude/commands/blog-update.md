# Skill: blog-update

## Purpose
Update an existing blog post using an SEO brief and generate an improved version of the content while strictly following the CXL tone of voice.

---

## Input
A keyword or URL provided by the user.

---

## Instructions

### Step 0: Load Tone of Voice (MANDATORY)
- Navigate to: `/cxl-resources/`
- Read:
  - `tone-of-voice.md`
  - `/blog-examples/` subfolder

- Extract tone characteristics:
  - Writing style
  - Sentence structure
  - Level of depth
  - Use of examples
  - Use of data and specificity
  - Clarity and directness

- These rules MUST be applied when rewriting content.

---

### Step 1: Find SEO Brief
- Search in `/seo-briefs/`
- Match file based on:
  - keyword OR
  - URL
- Extract:
  - Primary keyword
  - Secondary keywords
  - Content gaps
  - Recommendations
  - Suggested structure

---

### Step 2: Find Original Blog
- Search in `/workflows/scraped-blogs/`
- Match based on:
  - URL OR
  - keyword

---

### Step 3: Analyze Differences
Compare blog vs brief:
- Missing keywords
- Weak sections
- Missing sections
- Poor structure
- Lack of depth
- Outdated content

---

### Step 4: Improve Content (BRIEF-DRIVEN + CXL STYLE)

Rewrite and improve the blog **strictly based on the SEO brief recommendations**.

#### Core Principle:
Every improvement MUST be tied to the brief:
- If the brief suggests a section → add it
- If the brief highlights a gap → fix it
- If the brief suggests keywords → integrate them
- If the brief suggests structure → follow it

#### Apply Improvements:
- Add missing sections from the brief
- Restructure content based on suggested outline
- Integrate primary and secondary keywords naturally
- Expand sections identified as weak or incomplete
- Address all content gaps explicitly mentioned in the brief
- Improve clarity and flow where needed

#### Tone Enforcement (CXL Style):
- Write like an expert practitioner
- Be direct and practical
- Avoid vague or high-level statements
- Prioritize clarity over cleverness
- Use short to medium-length sentences
- Add concrete examples where relevant
- Match the depth and specificity of `/blog-examples/`

---

### Step 5: Track Changes
At the end of the document, add:

## Changes Made
- Added: [section based on brief]
- Improved: [section]
- Expanded: [topic]
- Keywords added: [list]
- Structure changes: [what was reorganized]
- Tone adjustments: [what changed to match CXL style]

---

### Step 6: Save Output
- Create a NEW file in:
  `/workflow/updated-drafts/`

- File name:
  `updated-{original-name}.md`

---

## Rules
- Never overwrite original file
- Always create a new version
- STRICTLY follow SEO brief recommendations
- STRICTLY follow CXL tone of voice
- Do not keyword stuff
- Avoid generic AI phrasing
- Prioritize depth, clarity, and usefulness

---

## Output
Return the full updated blog content.