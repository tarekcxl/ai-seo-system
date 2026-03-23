# Free A/B Test Calculator

The A/B Test Calculator helps you plan and analyze experiments with precision. It calculates sample size, test duration, and statistical significance, ensuring your A/B tests are backed by solid data for confident decision-making.

## Pre-Test Calculator – MDE

- What is the minimum detectable effect (MDE) to consider?
- How long should the test run to detect meaningful results?
- What's the sample size required for this test?
- How does the confidence level influence the test duration?

### How to Use

This section helps you estimate the required sample size for a valid experiment and the time needed to run your A/B test.

1. **Input your data:**

   - Confidence Level: Keep it at 95% for industry-standard confidence.
   - [Statistical Power](https://cxl.com/blog/statistical-power/): 80% is commonly used, but you can adjust.
   - Conversion rate for control: Enter the current conversion rate of your control group (e.g., 10%).
   - Number of variants: Specify how many test variants you are comparing against the control.
   - Weekly Conversions: The number of conversions you typically get in a week. Used to get an estimate of how many weeks you need to run your experiment.

2. **Calculate your MDE**:

   Click **Calculate** to find out:

   - **Minimum Detectable Effect (MDE):** The smallest effect size you aim to detect in a study.
   - **Significance:** Represents a meaningful difference you don't want to miss if it exists.
   - **Expression:** Entered as a percentage, either relative or absolute.
   - **Relation to Control:** MDE is either relative to or an absolute difference from the control conversion rate.
   - Example:
     - Control conversion rate = 10%
     - Desired minimum test variant conversion rate = 15%
     - MDE absolute = 5% – (15 – 10)
     - MDE relative = 50% – (15 – 10) / 10 × 100

### Data Input

- Confidence level %
- Power Level %
- Conversion Rate for control %
- Minimum Detectable Effect (MDE) %
- Number of Variants (not including control)
- Weekly Traffic
- Is the Minimum Effect Relative? Yes / No
- One-sided or Two-sided Test? One-sided / Two-sided

### Results

| Metric | Value |
|--------|-------|
| Sample Size per Group | |
| Total Sample Size | |
| Estimated Duration (weeks) | |

## Test Result Calculator

Once you've collected all your data, you can test if your variant is significantly different from the control. Before using this calculator, ensure the following:

- **Required Sample Size:** The test has reached the necessary sample size.
- **Avoid Multiple Testing:** Test only once you have collected all your data. Testing multiple times increases the risk of Type I errors by inflating the chance of finding a significant result by chance. Stick to your planned sample size and test duration before analyzing.

### How to Use

This section helps you analyze the performance of your A/B test to determine if your results are statistically significant.

- **Input the following data**:

  - **Control Visitors:** Enter the total number of visitors who saw the control version of the experiment.
  - **Control Conversions:** Enter the number of conversions (e.g., purchases, sign-ups) from those who saw the control version.
  - **Variant Visitors:** Enter the total number of visitors who saw the test variant.
  - **Variant Conversions:** Enter the number of conversions from those who saw the test variant.
  - **Confidence Level (%):** Keep it at 95% (industry standard) or adjust if needed.

- **Click "Calculate"** to view the results:

  The results will display important metrics, including the conversion rates, lift, confidence interval of the difference between, p-value, z-score, and whether the results are statistically significant. We suggest looking at the 1-sided tests since they are more relevant for A/B testing.

### Results

| Metric | Value |
|--------|-------|
| Control Conversion Rate | – |
| Variant Conversion Rate | – |
| Lift (%) | – |

**Absolute differences**

| Metric | Value |
|--------|-------|
| Absolute difference | – |
| Confidence Interval (Difference, %) | – |
| Right-Sided Interval (%) | – |
| Left-Sided Interval (%) | – |
| Value ± SE (%) | – |
| P-Value (One-sided) | – |
| P-value (Two-sided) | – |
| Z-Score | – |
| Significance (One-sided) | – |
| Bayesian Probability: Variant Wins (%) | – |
| Bayesian Probability: Control Wins (%) | – |
| Bayes Factor (H1/H0) | – |

**Relative differences**

| Metric | Value |
|--------|-------|
| Relative Confidence Interval (Difference, %) | – |
| Relative Right-Sided Interval (%) | – |
| Relative Left-Sided Interval (%) | – |
| Relative Difference ± SE | – |
| Relative P-Value | – |
| Relative Z-Score | – |

## Become Certified at CRO

Become a certified expert at conversion optimization with this comprehensive online course.

- Learn how to build and run world-class optimization programs
- Master everything there is to master about A/B testing
- Immediately apply learnings with hundreds of playbooks
- Drive better results without increasing costs

**Source:** https://cxl.com/ab-test-calculator/
