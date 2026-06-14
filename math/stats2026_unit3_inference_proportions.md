# AP Statistics (2026-27 CED) -- Unit 3: Inference for Categorical Data: Proportions

> Exam Weight: 15–25% | ~30 Class Periods
> The largest inference unit in the course. Covers one- and two-proportion confidence intervals and significance tests, plus chi-square tests for homogeneity and independence.

## Topics

### 3.1 Estimators
- A point estimator produces a single-number estimate of a population parameter; different samples give different estimates (sampling variability)
- An estimator is unbiased when the center of its sampling distribution equals the parameter it is estimating

### 3.2 Sampling Distributions for Sample Proportions
- $\hat{p}$ has mean $p$ and standard deviation $\sigma_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$
- The shape is approximately normal provided $np \geq 10$ and $n(1-p) \geq 10$ (the Large Counts condition)

### 3.3 Constructing a Confidence Interval for a Population Proportion
- One-sample z-interval: $\hat{p} \pm z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$
- Three conditions must be verified: the sample was selected randomly; observations are independent (apply the 10% condition when sampling without replacement); the Large Counts condition holds
- The margin of error grows with higher confidence levels and shrinks with larger sample sizes

### 3.4 Justifying a Claim Based on a Confidence Interval for a Population Proportion
- The confidence **level** (e.g., 95%) describes how often the procedure captures the true parameter across repeated sampling, not the probability for any single interval
- If a claimed parameter value falls outside the interval, the data provide evidence against that claim

### 3.5 Setting Up a Test for a Population Proportion
- Hypotheses take the form $H_0: p = p_0$ versus a one- or two-sided $H_a$
- The same three conditions required for the interval apply before computing the test statistic

### 3.6 p-Values
- The p-value is the probability of getting a sample result at least as far from $H_0$ as the observed one, **under the assumption that $H_0$ is true**
- Small p-values (below the chosen significance level $\alpha$) constitute evidence against $H_0$

### 3.7 Carrying Out a Test for a Population Proportion
- Test statistic: $z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$
- After obtaining the p-value, we either reject or fail to reject $H_0$ and state the conclusion in the context of the problem

### 3.8 Potential Errors When Performing Tests
- **Type I error**: rejecting $H_0$ when it is actually true; the probability of this equals $\alpha$
- **Type II error**: failing to reject $H_0$ when it is actually false; its probability is denoted $\beta$
- **Power** $= 1 - \beta$; power increases with larger sample size, larger $\alpha$, or a larger true difference from $H_0$
- Which error is more costly depends on the real-world consequences in the given scenario

### 3.9 Sampling Distributions for the Difference Between Sample Proportions
- The difference $\hat{p}_1 - \hat{p}_2$ has mean $p_1 - p_2$ and standard deviation $\sqrt{\frac{p_1(1-p_1)}{n_1} + \frac{p_2(1-p_2)}{n_2}}$
- Approximate normality requires both samples to satisfy their own Large Counts conditions

### 3.10 Constructing a Confidence Interval for the Difference Between Two Population Proportions
- Two-sample z-interval: $(\hat{p}_1 - \hat{p}_2) \pm z^* \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$

### 3.11 Justifying a Claim Based on a Confidence Interval for the Difference Between Two Population Proportions
- When the interval does not contain 0, the data suggest a real difference between the two proportions
- The direction and magnitude of the interval endpoints describe which group is higher and by roughly how much

### 3.12 Setting Up a Test for the Difference Between Two Population Proportions
- The null hypothesis is $H_0: p_1 = p_2$ (equivalently $p_1 - p_2 = 0$)
- Because $H_0$ assumes equal proportions, both samples are combined to form the pooled proportion: $\hat{p}_c = \frac{X_1 + X_2}{n_1 + n_2}$

### 3.13 Carrying Out a Test for the Difference Between Two Population Proportions
- The test statistic uses $\hat{p}_c$ in the standard error; the resulting z-value is used to find a p-value and reach a conclusion in context

### 3.14 Setting Up a Chi-Square Test for Homogeneity or Independence
- **Homogeneity**: the question is whether one categorical variable has the same distribution across several distinct populations or treatment groups
- **Independence**: the question is whether two categorical variables are associated within a single population
- Expected counts under $H_0$: $E = \frac{(\text{row total})(\text{column total})}{\text{table total}}$
- All expected counts must be at least 5; degrees of freedom equal $(r-1)(c-1)$

### 3.15 Carrying Out a Chi-Square Test for Homogeneity or Independence
- $\chi^2 = \sum \frac{(O - E)^2}{E}$; the p-value comes from a chi-square distribution with the appropriate degrees of freedom
- After reaching a conclusion, examine which cells contributed most to the statistic to understand where the distributions differ

## Key Formulas

| Formula | Description |
|---------|-------------|
| $\hat{p} \pm z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ | One-proportion z-interval |
| $z = \frac{\hat{p} - p_0}{\sqrt{p_0(1-p_0)/n}}$ | One-proportion z-test |
| $\hat{p}_c = \frac{X_1+X_2}{n_1+n_2}$ | Pooled proportion |
| $\chi^2 = \sum \frac{(O-E)^2}{E}$ | Chi-square statistic |

## Common Misconceptions

- A 95% confidence interval does not mean there is a 95% chance the parameter is inside this particular interval -- the level refers to how reliably the **procedure** works in the long run
- The p-value is not the probability that $H_0$ is true; it is the probability of the data given $H_0$
- "Fail to reject" means the data do not provide enough evidence against $H_0$, not that $H_0$ has been proven true
- In the test statistic formula, the standard error uses $p_0$ (the null value), not $\hat{p}$
- Choosing between chi-square independence and homogeneity depends on how the data were gathered: one sample with two variables recorded → independence; separate samples from different groups with one variable recorded → homogeneity
