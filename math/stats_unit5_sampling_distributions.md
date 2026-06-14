# Unit 5: Sampling Distributions
> Exam Weight: 7–12% | ~10–12 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content redistributed: CLT to **new Unit 2 (2.12)**, proportion sampling distributions to **new Unit 3**, mean sampling distributions to **new Unit 4**. See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 5.1 Why Different Samples Give Different Results
Different random samples from the same population produce different values of a statistic — this is an unavoidable feature of sampling, not a flaw.
- **Sampling variability** (also called sampling error): the natural variation in a statistic from one sample to another
- A **sampling distribution** describes the distribution of a statistic across all possible samples of the same size from the same population
- Understanding sampling distributions is the bridge between descriptive statistics and formal inference

### 5.2 Using the Normal Distribution for Sampling Problems
Many sampling distributions are approximately normal when certain conditions are met.
- The normal distribution underlies most inference procedures
- To find probabilities, standardize the statistic: $z = \frac{\text{statistic} - \text{mean of sampling distribution}}{\text{standard deviation of sampling distribution}}$, then use normal probability tools

### 5.3 The Central Limit Theorem
One of the most important results in statistics: for large enough samples, the sampling distribution of $\bar{x}$ is approximately normal.
- **Central Limit Theorem (CLT):** regardless of the population's shape, the sampling distribution of $\bar{x}$ approaches a normal distribution as $n$ increases
- Guidelines for "large enough":
  - Population is approximately normal → any sample size works
  - Moderate skewness → $n \geq 30$ is typically sufficient
  - Strong skewness or outliers → larger samples (e.g., $n \geq 50$) may be needed
- The CLT justifies using normal-based methods for means even when the population shape is unknown

### 5.4 Biased vs. Unbiased Estimators
A good estimator is centered at the true parameter value it estimates.
- A **statistic is unbiased** if its sampling distribution is centered at the true population parameter
- $\bar{x}$ is an unbiased estimator of $\mu$; $\hat{p}$ is an unbiased estimator of $p$; $s^2$ (with $n-1$ denominator) is an unbiased estimator of $\sigma^2$
- **Bias** means systematically missing the target; **variability** means spread around whatever is being hit
- Increasing sample size reduces variability but does not eliminate bias if the estimation method itself is flawed

### 5.5 Sampling Distribution of $\hat{p}$
The sample proportion $\hat{p}$ varies predictably from sample to sample.
- For a population proportion $p$:
  - **Mean of $\hat{p}$:** $\mu_{\hat{p}} = p$
  - **Standard deviation:** $\sigma_{\hat{p}} = \sqrt{\frac{p(1-p)}{n}}$
- **Conditions for approximate normality:**
  - Independence: random sample and $n < 10\%$ of population (10% condition)
  - Large counts: $np \geq 10$ and $n(1-p) \geq 10$
- When both conditions hold: $\hat{p} \approx N\left(p, \sqrt{\frac{p(1-p)}{n}}\right)$

### 5.6 Sampling Distribution of $\hat{p}_1 - \hat{p}_2$
Comparing two sample proportions from independent groups follows a predictable pattern.
- For independent samples from two populations:
  - **Mean:** $\mu_{\hat{p}_1 - \hat{p}_2} = p_1 - p_2$
  - **Standard deviation:** $\sigma_{\hat{p}_1 - \hat{p}_2} = \sqrt{\frac{p_1(1-p_1)}{n_1} + \frac{p_2(1-p_2)}{n_2}}$
- **Conditions:** independence and large counts for both samples ($n_i p_i \geq 10$ and $n_i(1-p_i) \geq 10$ for each group)

### 5.7 Sampling Distribution of $\bar{x}$
The sample mean $\bar{x}$ varies from sample to sample in a predictable way.
- For a population with mean $\mu$ and standard deviation $\sigma$:
  - **Mean of $\bar{x}$:** $\mu_{\bar{x}} = \mu$
  - **Standard error:** $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$
- **Conditions for approximate normality:**
  - Independence: random sample and $n < 10\%$ of population
  - Normality/CLT: population is normal, or $n$ is large enough
- Larger samples produce smaller standard errors, yielding more precise estimates

### 5.8 Sampling Distribution of $\bar{x}_1 - \bar{x}_2$
Comparing two sample means from independent groups also follows a predictable sampling distribution.
- For independent samples from two populations:
  - **Mean:** $\mu_{\bar{x}_1 - \bar{x}_2} = \mu_1 - \mu_2$
  - **Standard deviation:** $\sigma_{\bar{x}_1 - \bar{x}_2} = \sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$
- **Conditions:** independence and large-sample/normality conditions for both groups

## Key Formulas Summary

| Statistic | Mean | Standard Deviation |
|-----------|------|--------------------|
| $\hat{p}$ | $p$ | $\sqrt{\frac{p(1-p)}{n}}$ |
| $\hat{p}_1 - \hat{p}_2$ | $p_1 - p_2$ | $\sqrt{\frac{p_1(1-p_1)}{n_1} + \frac{p_2(1-p_2)}{n_2}}$ |
| $\bar{x}$ | $\mu$ | $\frac{\sigma}{\sqrt{n}}$ |
| $\bar{x}_1 - \bar{x}_2$ | $\mu_1 - \mu_2$ | $\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$ |

## Common Misconceptions
- The sampling distribution of a statistic is not the same as the population distribution — they describe different things
- The CLT applies to the **sampling distribution of $\bar{x}$**, not to the population shape itself
- Forgetting the 10% condition when sampling without replacement from a finite population
- Using the population standard deviation $\sigma_{\hat{p}}$ when $p$ is unknown — in practice, estimate with $SE_{\hat{p}} = \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$
- Applying the CLT's $n \geq 30$ guideline universally — if the population is normal, any sample size is sufficient
