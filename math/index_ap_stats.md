# AP Statistics — Course Overview

> **Exam Format:** 40 MC (1 hr 30 min, 50%) + 6 FRQ (1 hr 30 min, 50%)
> **Calculator:** Permitted (graphing calculator)
> **Reference Materials:** Formula sheet + probability tables provided

## Big Ideas

| Code | Big Idea |
|------|----------|
| **VAR** | Variation and Distribution |
| **UNC** | Patterns and Uncertainty |
| **DAT** | Data-Based Predictions, Decisions, and Conclusions |

## Units and Exam Weights

| Unit | Title | Exam Weight | Class Periods |
|------|-------|-------------|---------------|
| 1 | Exploring One-Variable Data | 15–23% | ~14–16 |
| 2 | Exploring Two-Variable Data | 5–7% | ~10–11 |
| 3 | Collecting Data | 12–15% | ~9–10 |
| 4 | Probability, Random Variables, and Probability Distributions | 10–20% | ~18–20 |
| 5 | Sampling Distributions | 7–12% | ~10–12 |
| 6 | Inference for Categorical Data: Proportions | 12–15% | ~16–18 |
| 7 | Inference for Quantitative Data: Means | 10–18% | ~14–16 |
| 8 | Inference for Categorical Data: Chi-Square | 2–5% | ~8–10 |
| 9 | Inference for Quantitative Data: Slopes | 2–5% | ~7–8 |

## Four Content Areas

1. **Exploring Data** (Units 1–2): Describing patterns, distributions, and relationships in data
2. **Collecting Data** (Unit 3): Planning and conducting studies — surveys, experiments, observational studies
3. **Probability & Sampling Distributions** (Units 4–5): Anticipating patterns using probability and simulation
4. **Statistical Inference** (Units 6–9): Estimating population parameters and testing hypotheses

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
- Geometric: $P(X = k) = (1-p)^{k-1} p$

### Sampling Distributions
- Standard error of $\hat{p}$: $\sigma_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$
- Standard error of $\bar{x}$: $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$

### Inference
- Confidence interval: $\text{statistic} \pm (\text{critical value}) \cdot (\text{standard error})$
- Chi-square statistic: $\chi^2 = \sum \frac{(O - E)^2}{E}$
- t-statistic for slope: $t = \frac{b - \beta_0}{SE_b}$

## Common Misconceptions (Cross-Unit)

1. **Correlation vs. causation:** Association does not imply causation without random assignment
2. **Random sampling vs. random assignment:** Sampling supports generalization; assignment supports causation
3. **Confidence level misinterpretation:** A 95% CI does NOT mean "95% probability the parameter is in this interval" — it means the method captures the true parameter 95% of the time
4. **p-value misinterpretation:** A p-value is NOT the probability that $H_0$ is true — it is the probability of observing data as extreme or more extreme, assuming $H_0$ is true
5. **"Fail to reject" vs. "accept":** We never "accept" $H_0$; we fail to reject it
6. **Standard deviation vs. standard error:** SD describes variability of data; SE describes variability of a statistic
