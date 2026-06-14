# AP Statistics (2026-27 CED) -- Unit 4: Inference for Quantitative Data: Means

> Exam Weight: 10–20% | ~18 Class Periods
> This unit develops t-based inference procedures for one-sample, paired, and two-independent-sample settings.

## Topics

### 4.1 Sampling Distributions for Sample Means
- $\bar{x}$ has mean $\mu$ and standard deviation $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$
- When the population is normal, the sampling distribution of $\bar{x}$ is exactly normal; when it is not, the Central Limit Theorem guarantees approximate normality for sufficiently large $n$ (often $n \geq 30$)
- Because $\sigma$ is rarely known in practice, the **t-distribution** is used instead; it has heavier tails than the normal and depends on degrees of freedom $n - 1$

### 4.2 Constructing a Confidence Interval for a Population Mean or Population Mean Difference
- One-sample t-interval: $\bar{x} \pm t^* \frac{s_x}{\sqrt{n}}$
- For **paired data**, subtract within each pair to form a single set of differences, then apply the one-sample t-procedure to those differences (parameter of interest: mean difference $\mu_d$)
- Conditions to verify: random sample, independence (10% condition when relevant), Normal/Large Sample

### 4.3 Justifying a Claim Based on a Confidence Interval for a Population Mean or Population Mean Difference
- State the interval in context and use it to evaluate a specific claim about the parameter
- For mean differences, check whether 0 is a plausible value -- if it is not in the interval, the data suggest a real difference

### 4.4 Setting Up a Test for a Population Mean or Population Mean Difference
- For one sample: $H_0: \mu = \mu_0$; for paired data: $H_0: \mu_d = 0$; alternatives can be one- or two-sided
- The same three conditions required for intervals must hold before proceeding

### 4.5 Carrying Out a Test for a Population Mean or Population Mean Difference
- Test statistic: $t = \frac{\bar{x} - \mu_0}{s_x / \sqrt{n}}$ with $df = n - 1$
- The p-value is found using the t-distribution; state the conclusion in the context of the problem

### 4.6 Sampling Distributions for the Difference Between Two Sample Means
- The difference $\bar{x}_1 - \bar{x}_2$ is centered at $\mu_1 - \mu_2$ and has standard deviation $\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}$
- Approximate normality follows from normality of each population or from sufficiently large sample sizes

### 4.7 Constructing a Confidence Interval for the Difference Between Two Population Means
- Two-sample t-interval: $(\bar{x}_1 - \bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$

### 4.8 Justifying a Claim Based on a Confidence Interval for the Difference Between Two Population Means
- Check whether 0 falls inside the interval to judge whether the data support a real difference
- Describe the direction and practical size of the difference in plain language tied to the context

### 4.9 Setting Up a Test for the Difference Between Two Population Means
- Null hypothesis: $H_0: \mu_1 = \mu_2$
- Key design decision: distinguish paired data (one group, two measurements) from two independent samples (separate groups) -- the correct choice changes which procedure to use

### 4.10 Carrying Out a Test for the Difference Between Two Population Means
- Test statistic: $t = \frac{(\bar{x}_1 - \bar{x}_2) - 0}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}$ with degrees of freedom determined by technology
- State the conclusion in context, referencing whether the p-value falls below $\alpha$

## Key Formulas

| Formula | Description |
|---------|-------------|
| $\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}$ | SD of the sampling distribution of $\bar{x}$ |
| $\bar{x} \pm t^* \frac{s_x}{\sqrt{n}}$ | One-sample t-interval |
| $t = \frac{\bar{x} - \mu_0}{s_x/\sqrt{n}}$ | One-sample t-test |
| $(\bar{x}_1-\bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$ | Two-sample t-interval |

## Common Misconceptions

- Reaching for z when $\sigma$ is unknown -- if the population standard deviation is not given, use t
- Treating paired data as two independent samples (or vice versa) -- always check the study design first
- Mixing up the standard deviation of the raw data with the standard error of a sample mean
- Reading a confidence interval as capturing 95% of individual data values rather than the parameter
- Assuming t-procedures break whenever data are skewed -- the procedures are quite robust, particularly as sample size grows
