# Unit 6: Inference for Categorical Data: Proportions
> Exam Weight: 12–15% | ~16–18 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content now in **new Unit 3** (Topics 3.1–3.13). See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 6.1 Why Normal-Based Methods Work for Inference
Inference for proportions rests on the fact that the sampling distribution of $\hat{p}$ is approximately normal when conditions are met.
- Using z-scores and normal probabilities for inference requires verifying conditions first
- Every inference procedure has conditions that must be checked before proceeding

### 6.2 Confidence Interval for a Population Proportion
A confidence interval estimates the unknown population proportion $p$ using sample data.
- **One-sample z-interval for $p$:**
  $$\hat{p} \pm z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$
- **Conditions:**
  1. **Random:** data from a random sample or randomized experiment
  2. **Independence (10% condition):** $n < 10\%$ of the population when sampling without replacement
  3. **Large counts:** $n\hat{p} \geq 10$ and $n(1-\hat{p}) \geq 10$
- **Margin of error:** $ME = z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$
- Common critical values: $z^* = 1.645$ (90%), $z^* = 1.96$ (95%), $z^* = 2.576$ (99%)
- **Interpretation template:** "We are C% confident that the true population proportion of [context] is between [lower] and [upper]"
- Required sample size for a desired margin of error: $n = \left(\frac{z^*}{ME}\right)^2 \hat{p}(1-\hat{p})$ (use $\hat{p} = 0.5$ if no prior estimate is available)

### 6.3 Using a Confidence Interval to Evaluate a Claim
A confidence interval lets us assess whether a specific claimed value of $p$ is plausible.
- If the claimed value lies **inside** the interval: the data do not provide convincing evidence against the claim
- If the claimed value lies **outside** the interval: there is convincing evidence the true proportion differs from the claimed value
- Higher confidence level → wider interval → less precision
- Larger sample size → narrower interval → more precision

### 6.4 Setting Up a Hypothesis Test for a Proportion
A hypothesis test evaluates whether sample data are consistent with a specific claim about $p$.
- **Null hypothesis ($H_0$):** no effect or no difference — typically $H_0: p = p_0$
- **Alternative hypothesis ($H_a$):** what we are looking for evidence to support
  - Two-sided: $H_a: p \neq p_0$
  - One-sided: $H_a: p > p_0$ or $H_a: p < p_0$
- **Conditions for the one-proportion z-test:**
  1. Random sample
  2. Independence (10% condition)
  3. Large counts using $p_0$: $np_0 \geq 10$ and $n(1-p_0) \geq 10$

### 6.5 The p-value and What It Means
The p-value quantifies how surprising the data would be if $H_0$ were true.
- **Test statistic:** $z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$
- **p-value:** the probability of obtaining a test statistic at least as extreme as the observed value, assuming $H_0$ is true
- A small p-value signals that the observed data would be rare under $H_0$ — evidence against it
- Interpretation: "Assuming [H₀ in context], the probability of observing a sample proportion as extreme as $\hat{p}$ is [p-value]"

### 6.6 Drawing a Conclusion from a Hypothesis Test
Compare the p-value to the significance level to reach a conclusion.
- **Significance level ($\alpha$):** the threshold for "small enough" — typically $\alpha = 0.05$
- If $p\text{-value} \leq \alpha$: **reject $H_0$** — "There is convincing evidence that [H_a in context]"
- If $p\text{-value} > \alpha$: **fail to reject $H_0$** — "There is not convincing evidence that [H_a in context]"
- Never say "accept $H_0$" — failing to reject is not the same as proving it true

### 6.7 Types of Errors and Power
Inference can lead to two kinds of mistakes.
- **Type I error:** rejecting $H_0$ when it is actually true (false positive); $P(\text{Type I}) = \alpha$
- **Type II error:** failing to reject $H_0$ when it is actually false (false negative); $P(\text{Type II}) = \beta$
- **Power:** $1 - \beta$ — the probability of correctly rejecting a false $H_0$
- Power increases with larger $n$, larger $\alpha$, or a larger true difference between $p$ and $p_0$
- There is a tradeoff: lowering $\alpha$ reduces Type I errors but raises Type II errors

### 6.8 Confidence Interval for the Difference Between Two Proportions
When comparing two population proportions, a two-proportion interval estimates $p_1 - p_2$.
- **Two-proportion z-interval:**
  $$(\hat{p}_1 - \hat{p}_2) \pm z^* \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$
- **Conditions:** Random (both samples), Independence (10% for both), Large counts for both groups

### 6.9 Interpreting a Two-Proportion Confidence Interval
- If 0 falls inside the interval for $p_1 - p_2$: no convincing evidence of a difference
- If 0 falls outside: convincing evidence that $p_1 \neq p_2$
- If the entire interval is positive: evidence that $p_1 > p_2$; if entirely negative: evidence that $p_1 < p_2$

### 6.10 Setting Up a Two-Proportion Hypothesis Test
- $H_0: p_1 = p_2$ (equivalently, $p_1 - p_2 = 0$)
- $H_a: p_1 \neq p_2$ (two-sided), $p_1 > p_2$, or $p_1 < p_2$ (one-sided)
- Under $H_0$, combine both samples to estimate the common proportion: **pooled proportion** $\hat{p}_c = \frac{X_1 + X_2}{n_1 + n_2}$

### 6.11 Carrying Out a Two-Proportion Hypothesis Test
- **Test statistic:**
  $$z = \frac{(\hat{p}_1 - \hat{p}_2) - 0}{\sqrt{\hat{p}_c(1-\hat{p}_c)\left(\frac{1}{n_1} + \frac{1}{n_2}\right)}}$$
- Use $\hat{p}_c$ to check the large-counts condition
- Compare the p-value to $\alpha$ and conclude in context

## Common Misconceptions
- Using $\hat{p}$ instead of $p_0$ to check large-counts conditions when performing a hypothesis test — use $p_0$ under $H_0$
- Using individual $\hat{p}_1$ and $\hat{p}_2$ instead of the pooled $\hat{p}_c$ in the two-proportion z-test statistic
- Misinterpreting the confidence level: "95% confident" refers to the method capturing the true value in 95% of repeated samples, not the probability that this specific interval contains the parameter
- Saying "accept $H_0$" — the correct language is "fail to reject $H_0$"
- Equating statistical significance with practical importance — a result can be statistically significant but practically trivial
- Treating the p-value as the probability that $H_0$ is true
