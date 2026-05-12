---
name: tone-of-voice-consistency
description: Evaluate whether written content matches the desired tone of voice using reference feedback and copywriter comments. Use this skill whenever reviewing drafted copy, checking tone consistency, validating whether content sounds on-brand, or applying tone feedback from reference files such as remark-1 and remark-2.
---

# Tone Voice Consistency

A skill for reviewing whether content matches the intended tone of voice.

This skill uses tone references and copywriter feedback to identify where copy feels off-brand, too generic, too formal, too fluffy, too salesy, or inconsistent with the desired writing style.

---

## What this skill does

Use this skill to:

- evaluate whether copy matches the desired tone of voice
- identify tone inconsistencies
- compare output against copywriter feedback
- flag phrases that feel off-brand
- suggest improvements that bring the copy closer to the intended style

---

## When to use this skill

Use this skill when the user wants to:

- check if content sounds on-brand
- review tone of voice
- compare copy against tone feedback
- improve writing based on copywriter comments
- validate whether AI-written copy sounds natural and consistent

Trigger when the user says things like:

- “check the tone”
- “does this sound on-brand?”
- “make sure this matches our voice”
- “review this against the copywriter feedback”
- “is the tone consistent?”

---

## Core principles

- Tone consistency is about judgment, not only rules
- Use the reference feedback as calibration
- Do not rewrite everything unless asked
- Identify what feels off and why
- Suggest focused improvements that preserve the original meaning

---

## Inputs

This skill may receive:

- draft copy
- blog sections
- full articles
- landing page copy
- email or social copy
- tone feedback references

---

## Reference Materials

This skill includes additional reference files.

### references/remark-1.md
Use this to understand copywriter feedback patterns, recurring issues, and what needs to be avoided.

### references/remark-2.md
Use this to understand additional tone expectations, preferred phrasing, and examples of what “good” or “bad” tone looks like.

Always consult these references when evaluating tone consistency.

Do not copy the references directly. Use them to calibrate judgment.

---

## How to work

### Step 1: Review the references

Before evaluating the copy, read:

- `references/remark-1.md`
- `references/remark-2.md`

Look for:

- repeated feedback themes
- phrases or styles to avoid
- preferred tone qualities
- examples of weak vs strong writing

---

### Step 2: Identify the intended tone

Infer the desired tone from the references.

Look for qualities such as:

- clear vs vague
- direct vs overly polished
- useful vs fluffy
- confident vs hype-heavy
- human vs generic AI-sounding
- specific vs broad

---

### Step 3: Evaluate the copy

Check whether the copy:

- matches the desired tone
- sounds natural and human
- avoids generic AI phrasing
- uses clear and specific language
- has the right level of confidence
- avoids unnecessary hype or filler

---

### Step 4: Flag tone issues

For each issue, identify:

- the original phrase or section
- what feels off
- why it conflicts with the reference feedback
- how to improve it

---

### Step 5: Suggest improvements

Provide targeted edits.

Focus on:

- improving tone
- keeping the original meaning
- making the copy sharper and more natural
- removing generic or off-brand phrasing

---

## Output structure

### Overall tone assessment

Briefly explain whether the copy is:

- on-brand
- mostly on-brand
- partially off-brand
- off-brand

---

### Tone score

Score from **1 to 10**.

- 9–10 = strongly on-brand
- 7–8 = mostly on-brand, minor fixes
- 5–6 = usable but needs tone refinement
- 3–4 = noticeably off-brand
- 1–2 = does not match the intended tone

---

### What works

List the parts that match the desired tone.

---

### What feels off

List specific phrases, sections, or patterns that feel inconsistent.

For each issue, include:

- original text
- issue
- suggested fix

---

### Recommended edits

Provide improved versions of the most important problematic lines or sections.

---

## Output quality bar

Strong evaluation:

- references the copywriter feedback patterns
- identifies specific tone issues
- explains why something feels off
- suggests practical improvements

Weak evaluation:

- gives vague feedback like “make it better”
- rewrites everything without explaining why
- ignores the reference files
- focuses only on grammar instead of tone

---

## Boundaries

This skill evaluates tone consistency.

It does not:

- perform SEO analysis
- fact-check claims
- decide content strategy
- rewrite the full piece unless explicitly asked

---

## Working style

Be precise, editorial, and practical.

Think like a copy editor applying previous feedback consistently across new content.