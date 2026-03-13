# Unit 5: Sampling Distributions
> Exam Weight: 7–12% | ~10–12 Class Periods

## Topics

### 5.1 Introducing Statistics: Why Is My Sample Not Like Yours?
- **Learning Objective (UNC-3.A):** Describe the concept of sampling variability
- **Essential Knowledge:**
  - Different random samples from the same population will produce different values of a statistic
  - **Sampling variability** (sampling error) is the natural variation in a statistic from sample to sample
  - A **sampling distribution** shows the distribution of a statistic over all possible samples of the same size from the same population
  - Sampling distributions describe the long-run behavior of a statistic

### 5.2 The Normal Distribution, Revisited
- **Learning Objective (VAR-6.A):** Use the normal distribution to calculate probabilities for sampling distributions
- **Essential Knowledge:**
  - Many sampling distributions are approximately normal when conditions are met
  - The normal distribution serves as the foundation for inference
  - Use z-scores and normal probability calculations to find probabilities: $z = \frac{\text{statistic} - \text{mean of sampling distribution}}{\text{standard deviation of sampling distribution}}$

### 5.3 The Central Limit Theorem
- **Learning Objective (UNC-3.B):** Explain and apply the Central Limit Theorem
- **Essential Knowledge:**
  - **Central Limit Theorem (CLT):** For sufficiently large sample sizes, the sampling distribution of the sample mean $\bar{x}$ is approximately normal, regardless of the population's shape
  - Guidelines for "sufficiently large":
    - Population approximately normal → any $n$ works
    - Moderate skew → $n \geq 30$ is usually sufficient
    - Strong skew or outliers → $n \geq 50$ or larger
  - The CLT is one of the most important results in statistics — it justifies using normal-based inference methods

### 5.4 Biased and Unbiased Point Estimates
- **Learning Objective (VAR-6.B):** Distinguish between biased and unbiased estimators
- **Essential Knowledge:**
  - A **statistic** is **unbiased** if its sampling distribution is centered at the true parameter value
  - $\bar{x}$ is an unbiased estimator of $\mu$
  - $\hat{p}$ is an unbiased estimator of $p$
  - $s^2$ (with $n-1$ denominator) is an unbiased estimator of $\sigma^2$
  - **Bias** vs. **variability:** bias means systematically off-target; variability means spread
  - Increasing sample size reduces variability but does NOT fix bias (if the method is biased)

### 5.5 Sampling Distributions for Sample Proportions
- **Learning Objective (VAR-6.C):** Describe the sampling distribution of $\hat{p}$
- **Essential Knowledge:**
  - For a sample proportion $\hat{p}$ from a population with proportion $p$:
    - **Mean:** $\mu_{\hat{p}} = p$
    - **Standard deviation:** $\sigma_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$
  - **Conditions for approximate normality:**
    - **Independence:** Random sample/assignment AND $n < 10\%$ of population (10% condition)
    - **Large counts:** $np \geq 10$ and $n(1-p) \geq 10$
  - When conditions are met: $\hat{p} \sim N\left(p, \sqrt{\frac{p(1-p)}{n}}\right)$ approximately

### 5.6 Sampling Distributions for Differences in Sample Proportions
- **Learning Objective (VAR-6.D):** Describe the sampling distribution of $\hat{p}_1 - \hat{p}_2$
- **Essential Knowledge:**
  - For independent samples from two populations:
    - **Mean:** $\mu_{\hat{p}_1 - \hat{p}_2} = p_1 - p_2$
    - **Standard deviation:** $\sigma_{\hat{p}_1 - \hat{p}_2} = \sqrt{\frac{p_1(1-p_1)}{n_1} + \frac{p_2(1-p_2)}{n_2}}$
  - **Conditions:** Independence for both samples, large counts for both samples ($n_1 p_1 \geq 10$, $n_1(1-p_1) \geq 10$, $n_2 p_2 \geq 10$, $n_2(1-p_2) \geq 10$)

### 5.7 Sampling Distributions for Sample Means
- **Learning Objective (VAR-6.E):** Describe the sampling distribution of $\bar{x}$
- **Essential Knowledge:**
  - For a sample mean $\bar{x}$ from a population with mean $\mu$ and standard deviation $\sigma$:
    - **Mean:** $\mu_{\bar{x}} = \mu$
    - **Standard deviation (standard error):** $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$
  - **Conditions for approximate normality:**
    - **Independence:** Random sample AND $n < 10\%$ of population
    - **Normality:** Population is normal, OR $n$ is large enough (CLT, typically $n \geq 30$)
  - Larger $n$ → smaller standard error → more precise estimates

### 5.8 Sampling Distributions for Differences in Sample Means
- **Learning Objective (VAR-6.F):** Describe the sampling distribution of $\bar{x}_1 - \bar{x}_2$
- **Essential Knowledge:**
  - For independent samples from two populations:
    - **Mean:** $\mu_{\bar{x}_1 - \bar{x}_2} = \mu_1 - \mu_2$
    - **Standard deviation:** $\sigma_{\bar{x}_1 - \bar{x}_2} = \sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$
  - **Conditions:** Independence for both samples (random + 10% condition for each), normality/large sample for each group

## Key Formulas Summary

| Statistic | Mean | Standard Deviation |
|-----------|------|--------------------|
| $\hat{p}$ | $p$ | $\sqrt{\frac{p(1-p)}{n}}$ |
| $\hat{p}_1 - \hat{p}_2$ | $p_1 - p_2$ | $\sqrt{\frac{p_1(1-p_1)}{n_1} + \frac{p_2(1-p_2)}{n_2}}$ |
| $\bar{x}$ | $\mu$ | $\frac{\sigma}{\sqrt{n}}$ |
| $\bar{x}_1 - \bar{x}_2$ | $\mu_1 - \mu_2$ | $\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$ |

## Common Misconceptions
- Confusing the distribution of a population with the sampling distribution of a statistic
- Thinking larger samples change the population shape — the CLT applies to the **sampling distribution**, not the population
- Forgetting to check the 10% condition when sampling without replacement
- Using $\sigma_{\hat{p}}$ when you should use the standard error $SE_{\hat{p}} = \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ (known vs. estimated)
- Thinking the CLT requires $n \geq 30$ in all cases — if the population is normal, any $n$ works
