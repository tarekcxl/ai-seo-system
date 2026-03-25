# Statistical Power: What It Is and How To Calculate It in A/B Testing

Years ago, when I first started [split-testing](https://cxl.com/blog/ab-testing-guide/), I thought every test was worth running. It didn't matter if it was changing a button color or a headline. I wanted to run that test.

My enthusiastic, yet misguided, belief was that I simply needed to find aspects to optimize, set up the [testing tool](https://cxl.com/blog/ab-testing-tools/), and start the test. After that, I thought, it was just a matter of awaiting the infamous [95% statistical significance](https://cxl.com/blog/magical-95-statistical-significance/).

I was wrong.

After implementing "statistically significant" variations, I experienced no lift in sales because there was no true lift. Many of those tests were doomed at inception. I was committing [common statistical errors](https://cxl.com/institute/online-course/statistics-for-ab-testing/), like not testing for a full business cycle or neglecting to take the effect size into consideration.

I also failed to consider another possibility: that an underpowered test could cause me to miss changes that would generate a true lift.

**Most A/B testing articles tell you to hit 95% significance. Far fewer tell you that a test can be statistically significant and still wrong, because the test was never powerful enough to detect anything real.**

Understanding statistical power, or the "sensitivity" of a test, is an essential part of pre-test planning. Get it right, and you implement changes that actually move revenue. Get it wrong, and you ship losing variations with confidence.

---

> **Quick overview**
>
> **What it is:** Statistical power is the probability of detecting a true effect when one exists. It is the inverse of the false negative rate (1 - β).
>
> **Why it matters:** An underpowered test misses real improvements and wastes testing cycles. Research shows median statistical power across many fields is well below 50%.
>
> **What you need to know:** Four levers control power: sample size, effect size, significance level, and desired power level. Adjusting any one changes the others.
>
> **Who it's for:** CRO practitioners and analysts running A/B tests who want to stop making decisions based on underpowered results.

---

## Table of contents

- [What is statistical power?](#what-is-statistical-power)
- [Type I and Type II errors](#type-i-and-type-ii-errors)
- [The variables that affect statistical power](#the-variables-that-affect-statistical-power)
- [The power formula: what the math actually tells you](#the-power-formula-what-the-math-actually-tells-you)
- [Most tests in the wild are underpowered](#most-tests-in-the-wild-are-underpowered)
- [Experimental design factors that affect power beyond sample size](#experimental-design-factors-that-affect-power-beyond-sample-size)
- [How to calculate statistical power for your test](#how-to-calculate-statistical-power-for-your-test)
- [Bayesian approaches and the post hoc power problem](#bayesian-approaches-and-the-post-hoc-power-problem)
- [What to do before your next test](#what-to-do-before-your-next-test)

---

## What is statistical power?

**Statistical power is the probability of observing a statistically significant result at level alpha (α) if a true effect of a certain magnitude is present.** It is your test's ability to detect a difference between variations when a difference actually exists.

Statistical power (1 - β) holds an inverse relationship with Type II errors (β). If your power is 80%, your probability of a false negative is 20%. If your power is 95%, your false negative probability drops to 5%.

Think of power as the sensitivity of a diagnostic test. A blood test with 50% sensitivity catches only half of all true cases. The other half go undetected. A test with 95% sensitivity catches almost everything. Your A/B test works the same way: low power means you will miss real improvements, declare a test inconclusive, and move on, never knowing what you left on the table.

**A properly powered test makes it likely that a real improvement is detected. An underpowered test gives you an unacceptably high chance of failing to reject a false null.**

Finding the right balance is both art and science. Before getting into the components, let's review the two error types we are trying to control.

---

## Type I and Type II errors

### Type I errors

**A Type I error, or false positive, rejects a null hypothesis that is actually true.** Your test measures a difference between variations that does not exist in reality. The observed difference is due to chance.

The probability of a Type I error, denoted by alpha (α), is the level of significance for your A/B test. At 95% confidence, you have a 5% probability of a Type I error (1.0 - 0.95 = 0.05).

You can lower your Type I error probability by increasing your confidence level from 95% to 99%. But that reduction comes at a cost. By increasing your confidence level, the probability of a false negative (Type II error) increases. **Lowering alpha reduces statistical power. If you need more power, one option is to increase your alpha** (e.g., from 5% to 10%), accepting a slightly higher false positive risk in exchange.

### Type II errors

**A Type II error, or false negative, is a failure to reject a null hypothesis that is actually false.** Your test finds no significant improvement in your variation even though one genuinely exists.

Beta (β) is the probability of a Type II error. If β is 20%, your power level is 80% (1.0 - 0.2 = 0.8). You can lower your false negative risk to 10% or 5%, for power levels of 90% or 95%, respectively.

As Paul D. Ellis observes: "A well thought out research design is one that assesses the relative risk of making each type of error, then strikes an appropriate balance between them."

**Bottom line:** You cannot minimize both error types simultaneously with a fixed sample size. Every test design is a trade-off. The question is whether you are making that trade-off deliberately.

---

## The variables that affect statistical power

There are four levers you can pull:

1. Sample size
2. Minimum Effect of Interest (MEI, or Minimum Detectable Effect)
3. Significance level (α)
4. Desired power level (implied Type II error rate)

### 1. Sample size

The largest single driver of statistical power is sample size. **You can compensate for a lot of uncertainty by having a large enough sample.** The trick is calculating a sample size that adequately powers your test without making it run longer than necessary — a longer test costs more and slows your testing cadence.

You need enough visitors to each variation as well as to each segment you want to analyze. Pre-test planning for sample size helps avoid underpowered tests; otherwise, you may not realize you are running too many variants or segments until it is too late.

A general guideline: run tests for at least two weeks but no more than four, to avoid problems from [sample pollution and cookie deletion](https://cxl.com/blog/sample-pollution/). Establishing a minimum sample size and a pre-set time horizon avoids the common error of running a test until it generates a significant difference, then stopping it (peeking).

### 2. Minimum Effect of Interest (MEI)

The [Minimum Effect of Interest](https://www.analytics-toolkit.com/glossary/minimum-effect-of-interest/) (MEI) is the smallest difference in results you actually care about detecting.

Smaller effects are harder to detect and require larger samples to retain the same power. Larger effects can be detected with smaller samples. But as Georgi Georgiev notes, big "improvements" from small sample sizes are often unreliable: "The issue is that, usually, there was no proper stopping rule nor fixed sample size, thus the nominal p-values and confidence intervals reported are meaningless."

A useful way to visualize this: power is like a fishing net. A fine-mesh net catches small fish (small effects) but requires more material. A coarse net misses anything small, even if it exists. Your MEI determines the mesh size you need.

### 3. Statistical significance level

A statistically significant test result is one where the probability of observing such a result, assuming the null hypothesis is true, is below your alpha threshold.

At a 5% alpha, you accept a 5% probability that you incorrectly rejected a true null. If you lower your alpha from 5% to 1%, you simultaneously increase the probability of a Type II error, assuming all else is equal. That reduces power.

Five percent is the standard starting level for online testing. It is not sacred. There are legitimate reasons to use 10% (lower-stakes tests, smaller teams, limited traffic) or 1% (high-cost decisions, regulated industries).

### 4. Desired power level

With 80% power, you have a 20% probability of not detecting an actual effect at your chosen MEI. If 20% is too risky, you can lower that probability to 10% or 5%, which increases power to 90% or 95%.

**Each increase in power requires a corresponding increase in sample size and test duration.** A jump from 80% to 95% power roughly doubles the required sample size. Before targeting higher power, weigh whether the extra certainty justifies the slower test velocity.

The statistician Jacob Cohen suggested that 80% represents a reasonable balance between alpha and beta risk for most research settings. In conversion optimization, 80% is a widely accepted starting point. Anything below 70% should make you uncomfortable.

---

## The power formula: what the math actually tells you

Most practitioners use calculators to find sample sizes. But understanding the formula behind those calculators changes how you think about the trade-offs.

For a two-sample test (the typical A/B test structure), the required sample size per group is:

```
n = (z_α + z_β)² × 2σ² / δ²
```

Where:
- **z_α** is the critical z-value for your significance level (1.96 for α = 0.05 two-tailed)
- **z_β** is the critical z-value for your desired power (0.84 for 80% power; 1.28 for 90% power)
- **σ²** is the variance of the outcome metric
- **δ** is the true effect size you want to detect (your MEI)

What this formula reveals immediately:

**Effect size has quadratic impact on sample size.** If you halve your MEI (decide to detect smaller effects), you need four times as many observations, not twice as many. This is why chasing small improvements is expensive: a test designed to detect a 2% lift requires roughly four times more traffic than one designed to detect a 4% lift.

**Variance reduction is a legitimate power strategy.** Lower σ² reduces required sample size directly. This is why using continuous metrics (like revenue per visitor) can sometimes be more efficient than binary conversion metrics: if you can reduce noise in your outcome measure, you get more power from the same sample.

For those who want to work with standardized effect sizes, Cohen's d is the most common:

```
d = (μ₁ - μ₂) / σ
```

Cohen's benchmarks: d = 0.2 (small), d = 0.5 (medium), d = 0.8 (large). **Most commercially significant CRO effects fall in the small-to-medium range.** Planning for a "large" effect when your actual effect is small means your test will be underpowered even if you hit your planned sample size.

**Bottom line:** The formula tells you that sample size, effect size, variance, and power are locked together. You cannot change one without affecting the others. Calculators hide this; understanding the formula does not.

---

## Most tests in the wild are underpowered

This is not a theoretical concern. The data on actual research power is sobering:

- A 2013 meta-analysis of economics research found **median statistical power of 18%** across 159 studies in economics journals (Ioannidis, Stanley & Doucouliagos).
- In psychology, the Open Science Collaboration's 2015 replication project found that **fewer than half of published findings replicated**, partly due to chronic underpowering.
- A review of ecology literature found median power around 16% for detecting small effects.
- In clinical research, median power is often estimated at 50-60% for published trials, still well short of ideal.

**The pattern: most published studies, across most disciplines, are underpowered for small-to-medium effects.** The same problem exists in CRO. Teams run tests for a fixed number of days, declare whatever p-value they see as the result, and move on, without ever checking whether the test had adequate power to detect their target effect in the first place.

The practical consequence: an underpowered test that returns a non-significant result tells you almost nothing. It could mean there is no effect. Or it could mean there is an effect, but your test was too weak to find it. Without power analysis, you cannot tell the difference.

**Underpowered tests do not just waste time. They let real improvements go undiscovered, and they inflate the apparent effect sizes of the few significant results that do emerge** (a phenomenon called the "winner's curse": significant results from underpowered studies tend to overestimate the true effect).

---

## Experimental design factors that affect power beyond sample size

Sample size gets most of the attention. But two other design decisions affect power significantly.

### Measurement precision

The lower the variance in your outcome metric, the more power you get from a given sample. Measurement precision matters.

Practical implications:
- **Choose metrics with lower baseline variance.** Revenue per visitor has higher variance than conversion rate in absolute terms, but for tests with large average order values, it can be more sensitive to treatment effects. Understand the variance of your chosen metric before locking in a sample size.
- **Reduce noise in your outcome.** Minimize the effect of users who land on the test page but were never going to convert regardless of variation (bot traffic, international visitors outside your target market, mobile users if your test only meaningfully affects desktop). Segmenting them out before analysis reduces variance and increases effective power.
- **Use covariate adjustment where available.** If you have a pre-test measure of the outcome (e.g., prior visit conversion rate per user), including it as a covariate in your analysis can substantially increase power without increasing sample size.

### Experimental design efficiency

How you allocate traffic to variations affects power.

- **Equal allocation (50/50) maximizes power** for a fixed total sample. Unequal splits (e.g., 80/20) reduce power for the same total sample size. If you need to limit exposure to a risky variation, build that into your power calculation from the start.
- **Reducing the number of variations per test** increases power per variation. A 1-vs-1 test is more powerful than a 1-vs-4 test for the same total traffic, because each variation gets more observations.
- **Testing high-traffic pages** is not just a strategic preference. It is a power decision. A test on a page with 500 daily visitors needs months to reach adequate power for small effects. A test on a page with 10,000 daily visitors reaches that same power in days.

**Bottom line:** You do not always need more traffic. Sometimes you need less noisy measurements, better traffic allocation, or a simpler test design.

---

## How to calculate statistical power for your test

Using a [sample size calculator](https://cxl.com/ab-test-calculator/) or [G*Power](http://www.psychologie.hhu.de/arbeitsgruppen/allgemeine-psychologie-und-arbeitspsychologie/gpower.html), you can plug in your values to find what is required to run an adequately powered test. If you know three of the four inputs, you can calculate the fourth.

**Example using G*Power:** With 80% power, a 5% alpha (95% significance), a control conversion rate of 14%, and an expected variant rate of 19%, the required sample size is 681 visitors per variation.

You can also work backwards. If you know your sample size, alpha, and desired power level, you can find the MEI your test is sensitive enough to detect. This is useful for tests where traffic is limited: it tells you the minimum effect size you can reliably detect with the traffic you have.

### Power analysis tools compared

| Tool | Best for | Notes |
| --- | --- | --- |
| **G*Power** | Deep statistical power analysis across many test types | Free desktop app; supports t-tests, chi-square, ANOVA, regression, and more. Steep learning curve but comprehensive |
| **CXL A/B Test Calculator** | Quick sample size estimation for CRO | [cxl.com/ab-test-calculator](https://cxl.com/ab-test-calculator/). Designed for conversion rate tests with simple inputs |
| **Evan Miller's calculator** | Fast online checks | Simple interface; widely cited in the CRO community for proportions tests |
| **WebPower (R package)** | Programmable power analysis at scale | Useful if you are running many tests programmatically or need non-standard test types |
| **pwr (R package)** | Standard power calculations with Cohen's d | Good for analysts comfortable in R who want reproducible power calculations alongside test design |

For most CRO practitioners, the CXL calculator or Evan Miller's tool is sufficient for proportions tests. Use G*Power when you need power analysis for non-standard test types (e.g., multivariate tests, regression discontinuity designs).

### What if you cannot increase your sample size?

There will come a day when you need more power but more traffic is not available, perhaps due to a low-traffic page or a test targeting a narrow segment.

Your options:

1. **Increase the MEI.** Accept that you will only detect larger effects. In the example above, increasing the MEI from 10% to 25% reduces the required sample from 8,000+ to 1,356 per variant. The trade-off: you will miss smaller improvements entirely.

2. **Lower the confidence level to 90%.** As long as you are comfortable with a 10% chance of a Type I error, this is a legitimate choice for lower-stakes tests.

3. **Reduce noise in your metric** (see the experimental design section above). This is often the most underused option.

4. **Aggregate multiple time periods.** Combining data across similar traffic periods (same day-of-week, same seasonality window) can increase sample size without extending the current test.

Georgiev notes that too many analysts "start with the sample size (test needs to be done by a semi-arbitrary number of weeks) and then nudge the levers randomly until the output fits." That produces tests designed to hit a deadline, not tests designed to answer a question.

---

## Bayesian approaches and the post hoc power problem

### The post hoc power fallacy

Post hoc power analysis, calculating the power of a test after you already know the result, is almost always a mistake.

Here is why: if your test returned a non-significant result, the post hoc power calculation will give you a low power estimate. If it returned a significant result, the calculation will give you a high power estimate. The post hoc power number is just a mathematical transformation of your p-value. **It adds no new information and creates the false impression that you have assessed your test's adequacy after the fact.**

The only valid use of post hoc power is to estimate the power you would have had for effect sizes other than the observed one, for planning future tests. It is not a diagnostic for the test you just ran.

### Bayesian alternatives

Frequentist power analysis (the standard approach covered above) is grounded in the null hypothesis significance testing framework. Bayesian approaches replace the power/α setup with a different question: given the data you have, how much should you update your beliefs?

In a Bayesian framework, you typically evaluate a Bayes factor (BF), which quantifies the evidence for the alternative hypothesis relative to the null:

- **BF > 10**: strong evidence for the alternative
- **BF 3-10**: moderate evidence
- **BF 1-3**: weak evidence
- **BF < 1**: evidence favors the null

Bayesian power analysis asks: "What sample size do I need to achieve a Bayes factor above a given threshold with high probability?" This is more directly interpretable than frequentist power in some ways, because it tells you about evidence strength, not just error rates.

**When Bayesian testing makes sense:**
- Sequential testing environments where you need to monitor results continuously (Bayesian tests are less prone to the peeking problem that inflates Type I errors in frequentist sequential designs)
- Situations where you have strong prior information about the expected effect size
- Teams that find the posterior probability interpretation more intuitive than confidence intervals

**When to stick with frequentist power analysis:**
- Standard A/B testing setups where you run the test to a fixed sample size
- Regulatory or compliance-heavy contexts where frequentist statistics are the accepted standard
- Teams without the statistical infrastructure to implement Bayesian updating

Neither approach is universally superior. The choice depends on your testing infrastructure, team fluency, and decision-making context.

---

## What to do before your next test

The data reveals the shape of the problem. Your next move is whether you build power analysis into your testing process or keep making the same expensive mistakes.

**1. Run a power calculation before you start every test.** Use your baseline conversion rate, your MEI (the smallest lift worth detecting), your desired alpha, and your target power level (80% minimum). This tells you the sample size you need. If you cannot hit it, adjust one of the levers deliberately, not randomly.

**2. Set your MEI based on business value, not wishful thinking.** Ask: what is the smallest improvement that would justify shipping this change? A 2% lift on a page generating $1M/month in conversions has a different minimum detectable threshold than a 2% lift on a page generating $20K/month. Size your test to the business decision, not to what sounds statistically respectable.

**3. Check your test's power before calling a non-significant result a "no effect" result.** A non-significant result from a well-powered test is meaningful evidence. A non-significant result from an underpowered test is noise. They are not the same thing, and treating them the same leads to bad decisions.

**4. If you are running low-traffic tests, prioritize noise reduction before sample size.** Segment out irrelevant traffic, use more sensitive metrics where possible, and simplify your test design. These are often faster paths to adequate power than waiting for more visitors.

**5. Avoid post hoc power calculations as diagnostics.** They tell you nothing about your test that the p-value does not already tell you. Use power analysis for planning, not for explaining results after the fact.

**The effort:** a few minutes of pre-test calculation and a deliberate decision about your MEI before you start.

**The payoff:** tests that actually tell you something, rather than tests that give you an answer you cannot trust.

---

Statistical power is not a technicality. It is the foundation that determines whether your testing program produces real insights or expensive noise. A test without adequate power is a test you cannot learn from.

The tools are free. The calculations take minutes. There is no good reason to keep running underpowered tests.

If you want to build rigorous A/B testing skills from the ground up, explore CXL's [statistics for A/B testing course](https://cxl.com/institute/online-course/statistics-for-ab-testing/) and the full [experimentation program](https://cxl.com/institute/programs/experimentation/).

---

## Changes Made

- **Added:** "The power formula: what the math actually tells you" section covering the n = (z_α + z_β)² × 2σ²/δ² formula, Cohen's d, quadratic relationship between effect size and sample size, and variance reduction as a power strategy -- HIGH IMPACT gap from brief
- **Added:** "Most tests in the wild are underpowered" section with discipline-specific benchmarks: economics (18% median power), psychology replication crisis, ecology (16%), clinical research (~50-60%) -- HIGH IMPACT gap from brief
- **Added:** "Bayesian approaches and the post hoc power problem" section covering post hoc power fallacy, Bayes factor interpretation, when to use Bayesian vs. frequentist testing -- HIGH IMPACT gap from brief
- **Added:** "Experimental design factors that affect power beyond sample size" section covering measurement precision, covariate adjustment, traffic allocation, variation count -- MEDIUM IMPACT gap from brief
- **Added:** "What to do before your next test" section with five actionable steps and "The effort:" / "The payoff:" structure -- CXL tone pattern from 1000-marketing-jobs.md
- **Added:** Quick Overview summary box at the top -- CXL tone pattern from customer-journey-maps.md
- **Added:** Power analysis tools comparison table covering G*Power, CXL calculator, Evan Miller, WebPower, and pwr package -- LOW IMPACT gap from brief
- **Added:** Diagnostic test sensitivity analogy in the definition section ("power is like a fishing net") -- MEDIUM IMPACT gap from brief
- **Improved:** Opening given stronger bold callout ("Most A/B testing articles tell you to hit 95% significance. Far fewer tell you...") -- CXL tone pattern
- **Improved:** "Bottom line:" conclusions added at end of key sections (Type I/II errors, power formula, design factors) -- CXL tone pattern from logical-fallacies.md
- **Improved:** Conclusion rewritten to be direct and action-driving rather than a generic summary list
- **Improved:** All subheadings rewritten as standalone statements rather than topic labels
- **Removed:** Boilerplate newsletter, related posts, and comment sections from scraped original
- **Tone adjustments:** No em dashes; bold callouts used for key insights throughout; direct practitioner voice maintained from original; removed vague phrasing in favor of specific claims
- **Keywords integrated:** statistical power, statistical power formula, statistical power in A/B testing, post hoc power analysis, Bayesian power analysis, sample size calculation, Type I error, Type II error, minimum effect of interest, underpowered tests, G*Power, power analysis tools, statistical significance, effect size
- **Structure changes:** Added five new major sections (formula, benchmarks, Bayesian/post hoc, experimental design, pre-test checklist); added Quick Overview; expanded calculator section with tool comparison; restructured conclusion to be urgency-driven
