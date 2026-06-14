# AP® Statistics — Course Overview

> **Current framework effective fall 2026** (2026-27 school year; first exam under this framework May 2027, fully digital via Bluebook).
> The legacy 2020 framework (9 units) applied through the May 2026 exam; see the legacy section below.
> Last updated: 2026-06-10

## Exam Format (effective with the May 2027 exam)

| Section | Questions | Time | Weight |
|---------|-----------|------|--------|
| I: Multiple-Choice | 42 questions (4 answer choices each) | 90 min | 50% |
| II: Free-Response | 4 questions, 10 points each | 90 min | 50% |

- Graphing calculator with statistical capabilities expected throughout
- Formula sheet and tables provided
- Prerequisite reduced to first-year algebra (second-year algebra requirement removed)

## Statistical Practices

| Practice | Name | MCQ Weighting |
|----------|------|---------------|
| 1 | Formulate Questions | 5–10% |
| 2 | Collect Data | 20–30% |
| 3 | Analyze Data | 25–35% |
| 4 | Interpret Results | 25–35% |

The course is structured around a four-step statistical investigation cycle: formulating questions → collecting data → analyzing data → interpreting results. All four practices weave through every unit.

## Units and Exam Weights (5 units)

| Unit | Title | Exam Weight | Class Periods | File |
|------|-------|-------------|---------------|------|
| 1 | Exploring One-Variable Data and Collecting Data | 20–30% | ~26 | [stats2026_unit1_exploring_and_collecting.md](https://tsun-u.github.io/tsunumon-kb/math/stats2026_unit1_exploring_and_collecting.md) |
| 2 | Probability, Random Variables, and Probability Distributions | 15–25% | ~24 | [stats2026_unit2_probability_distributions.md](https://tsun-u.github.io/tsunumon-kb/math/stats2026_unit2_probability_distributions.md) |
| 3 | Inference for Categorical Data: Proportions | 15–25% | ~30 | [stats2026_unit3_inference_proportions.md](https://tsun-u.github.io/tsunumon-kb/math/stats2026_unit3_inference_proportions.md) |
| 4 | Inference for Quantitative Data: Means | 10–20% | ~18 | [stats2026_unit4_inference_means.md](https://tsun-u.github.io/tsunumon-kb/math/stats2026_unit4_inference_means.md) |
| 5 | Regression Analysis | 10–20% | ~9 | [stats2026_unit5_regression.md](https://tsun-u.github.io/tsunumon-kb/math/stats2026_unit5_regression.md) |

## What Changed from the 2020 Framework

**Removed from the course:**
- Analyzing departures from linearity (old 2.9)
- Combining random variables (old 4.9)
- Geometric distribution (old 4.12)
- Chi-square goodness of fit test (old 8.2–8.3)
- All of old Unit 9: inference for regression slopes

**Restructured:**
- Old Units 1 + 3 → new Unit 1 (one-variable data + collecting data)
- Normal distribution moved from old Unit 1 into new Unit 2 (as a probability model)
- Two-categorical-variable analysis moved from old Unit 2 into new Unit 2
- Sampling distributions split across new Units 2–4, placed alongside the inference procedures that rely on them
- Chi-square homogeneity/independence joined proportions in new Unit 3
- Old Unit 2's bivariate quantitative content became new Unit 5 (descriptive only)

**Added:** investigative-question topics (Practice 1) woven through all units.

## Key Formulas (Reference Sheet Highlights)

### Descriptive Statistics
- Sample mean: $\bar{x} = \frac{\sum x_i}{n}$
- Sample standard deviation: $s_x = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n - 1}}$
- Interquartile range: $IQR = Q_3 - Q_1$
- Outlier fences: $Q_1 - 1.5 \cdot IQR$ and $Q_3 + 1.5 \cdot IQR$
- z-score: $z = \frac{x - \mu}{\sigma}$

### Regression
- Least-squares slope: $b = r \cdot \frac{s_y}{s_x}$
- Intercept: $a = \bar{y} - b\bar{x}$
- Coefficient of determination: $r^2$

### Probability
- Addition rule: $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
- Multiplication rule: $P(A \cap B) = P(A) \cdot P(B|A)$
- Binomial: $P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$

### Sampling Distributions
- Standard error of $\hat{p}$: $\sigma_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$
- Standard error of $\bar{x}$: $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$

### Inference
- Confidence interval: $\text{statistic} \pm (\text{critical value}) \cdot (\text{standard error})$
- Chi-square statistic: $\chi^2 = \sum \frac{(O - E)^2}{E}$

## Core Vocabulary (for subject/topic classification)

distribution, normal distribution, binomial distribution, sampling distribution, percentile, quartile, interquartile range, standard deviation, variance, mean, median, mode, proportion, sample proportion, population, sample, census, bias, random sampling, stratified, cluster, experiment, treatment, confounding, random assignment, placebo, blinding, probability, conditional probability, independence, random variable, expected value, z-score, empirical rule, central limit theorem, confidence interval, margin of error, hypothesis test, null hypothesis, alternative hypothesis, p-value, significance level, type I error, type II error, power, t-distribution, degrees of freedom, chi-square, two-way table, scatterplot, correlation, regression, least-squares, slope, intercept, residual, coefficient of determination, extrapolation

## Common Misconceptions (Cross-Unit)

1. **Correlation vs. causation:** Observing an association does not establish cause-and-effect — only random assignment in an experiment supports causal conclusions
2. **Random sampling vs. random assignment:** Random sampling supports generalization to a population; random assignment supports causal conclusions
3. **Confidence interval interpretation:** A 95% CI does not mean "95% probability the parameter falls here" — it means the interval-building method captures the true parameter 95% of the time across repeated samples
4. **p-value interpretation:** A p-value is not the probability that $H_0$ is true — it is the probability of observing a result at least as extreme as the data, assuming $H_0$ is true
5. **"Fail to reject" is not "accept":** We never conclude $H_0$ is true; we only conclude that the data do not provide convincing evidence against it
6. **Standard deviation vs. standard error:** Standard deviation describes variability within a dataset; standard error describes how much a statistic varies from sample to sample

## Legacy: 2020 Framework (9 units, last exam May 2026)

Older teaching materials and videos may reference this structure. Files retained for reference; each carries a restructure note.

| Old Unit | Title | Old Weight | File | Now lives in |
|----------|-------|-----------|------|--------------|
| 1 | Exploring One-Variable Data | 15–23% | [stats_unit1_exploring_one_variable.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit1_exploring_one_variable.md) | New Unit 1 (normal dist → Unit 2) |
| 2 | Exploring Two-Variable Data | 5–7% | [stats_unit2_exploring_two_variables.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit2_exploring_two_variables.md) | New Units 5 + 2 |
| 3 | Collecting Data | 12–15% | [stats_unit3_collecting_data.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit3_collecting_data.md) | New Unit 1 |
| 4 | Probability, Random Variables, and Probability Distributions | 10–20% | [stats_unit4_probability.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit4_probability.md) | New Unit 2 (geometric dist removed) |
| 5 | Sampling Distributions | 7–12% | [stats_unit5_sampling_distributions.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit5_sampling_distributions.md) | New Units 2–4 |
| 6 | Inference for Categorical Data: Proportions | 12–15% | [stats_unit6_proportions.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit6_proportions.md) | New Unit 3 |
| 7 | Inference for Quantitative Data: Means | 10–18% | [stats_unit7_means.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit7_means.md) | New Unit 4 |
| 8 | Inference for Categorical Data: Chi-Square | 2–5% | [stats_unit8_chi_square.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit8_chi_square.md) | New Unit 3 (GOF removed) |
| 9 | Inference for Quantitative Data: Slopes | 2–5% | [stats_unit9_slopes.md](https://tsun-u.github.io/tsunumon-kb/math/stats_unit9_slopes.md) | **Removed from course** |
