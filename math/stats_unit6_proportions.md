# Unit 6: Inference for Categorical Data: Proportions
> Exam Weight: 12–15% | ~16–18 Class Periods

## Topics

### 6.1 Introducing Statistics: Why Be Normal?
- **Learning Objective (UNC-4.A):** Explain why normal distributions are used in inference
- **Essential Knowledge:**
  - The sampling distributions of many statistics are approximately normal when conditions are met
  - This normality allows us to use z-scores and standard normal tables/calculators for inference
  - Inference procedures have conditions that must be verified before proceeding

### 6.2 Constructing a Confidence Interval for a Population Proportion
- **Learning Objective (UNC-4.B):** Construct a confidence interval for a population proportion
- **Essential Knowledge:**
  - **One-sample z-interval for $p$:**
    $$\hat{p} \pm z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$$
  - **Conditions:**
    1. **Random:** data come from a random sample or randomized experiment
    2. **Independence (10% condition):** $n < 10\%$ of population when sampling without replacement
    3. **Large counts:** $n\hat{p} \geq 10$ and $n(1-\hat{p}) \geq 10$
  - **Margin of error:** $ME = z^* \cdot SE_{\hat{p}} = z^* \sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$
  - Common critical values: $z^* = 1.645$ (90%), $z^* = 1.96$ (95%), $z^* = 2.576$ (99%)
  - **Interpretation:** "We are C% confident that the true population proportion of [context] is between [lower] and [upper]"
  - To find required sample size for a given margin of error: $n = \left(\frac{z^*}{ME}\right)^2 \hat{p}(1-\hat{p})$ (use $\hat{p} = 0.5$ if unknown)

### 6.3 Justifying a Claim Based on a Confidence Interval
- **Learning Objective (DAT-4.A):** Use a confidence interval to justify or refute a claim about a proportion
- **Essential Knowledge:**
  - If the claimed value is **inside** the confidence interval, there is not convincing evidence against the claim
  - If the claimed value is **outside** the confidence interval, there is convincing evidence against the claim
  - Higher confidence level → wider interval → less precise
  - Larger sample size → narrower interval → more precise

### 6.4 Setting Up a Test for a Population Proportion
- **Learning Objective (VAR-6.G):** Set up hypotheses and identify the appropriate test for a proportion
- **Essential Knowledge:**
  - **Null hypothesis ($H_0$):** a statement of "no effect" or "no difference," typically $H_0: p = p_0$
  - **Alternative hypothesis ($H_a$):**
    - Two-sided: $H_a: p \neq p_0$
    - One-sided: $H_a: p > p_0$ or $H_a: p < p_0$
  - The alternative hypothesis is the claim we are looking for evidence to support
  - **Conditions for a one-proportion z-test:**
    1. Random sample
    2. Independence (10% condition)
    3. Large counts: $np_0 \geq 10$ and $n(1-p_0) \geq 10$ (use $p_0$, not $\hat{p}$!)

### 6.5 Interpreting p-Values
- **Learning Objective (DAT-4.B):** Calculate and interpret a p-value
- **Essential Knowledge:**
  - **Test statistic:** $z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}$
  - **p-value:** the probability of getting a test statistic as extreme as or more extreme than the observed value, assuming $H_0$ is true
  - Small p-value → strong evidence against $H_0$
  - Interpretation: "Assuming [H₀ in context], there is a [p-value] probability of observing a sample proportion as extreme as or more extreme than $\hat{p}$"

### 6.6 Concluding a Test for a Population Proportion
- **Learning Objective (DAT-4.C):** Make a conclusion based on the p-value and significance level
- **Essential Knowledge:**
  - **Significance level ($\alpha$):** the threshold for deciding whether the p-value is small enough to reject $H_0$ (typically $\alpha = 0.05$)
  - If $p\text{-value} \leq \alpha$: **reject $H_0$** — "There is convincing evidence that [H_a in context]"
  - If $p\text{-value} > \alpha$: **fail to reject $H_0$** — "There is not convincing evidence that [H_a in context]"
  - Never say "accept $H_0$" — we can only fail to reject it

### 6.7 Potential Errors When Performing Tests
- **Learning Objective (UNC-4.C):** Describe Type I and Type II errors, and the concept of power
- **Essential Knowledge:**
  - **Type I error:** rejecting $H_0$ when $H_0$ is actually true (false positive)
    - $P(\text{Type I error}) = \alpha$
  - **Type II error:** failing to reject $H_0$ when $H_0$ is actually false (false negative)
    - $P(\text{Type II error}) = \beta$
  - **Power:** $1 - \beta$ — the probability of correctly rejecting $H_0$ when it is false
  - Factors that increase power:
    - Larger sample size ($n$)
    - Larger significance level ($\alpha$)
    - Larger true effect (difference between true parameter and $p_0$)
  - There is a tradeoff: decreasing $\alpha$ reduces Type I error but increases Type II error

### 6.8 Confidence Interval for the Difference of Two Proportions
- **Learning Objective (UNC-4.D):** Construct a confidence interval for $p_1 - p_2$
- **Essential Knowledge:**
  - **Two-proportion z-interval:**
    $$(\hat{p}_1 - \hat{p}_2) \pm z^* \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$
  - **Conditions:** Random (both samples), Independence (10% condition for both), Large counts ($n_1\hat{p}_1 \geq 10$, $n_1(1-\hat{p}_1) \geq 10$, $n_2\hat{p}_2 \geq 10$, $n_2(1-\hat{p}_2) \geq 10$)

### 6.9 Justifying a Claim Based on a Confidence Interval for a Difference
- **Learning Objective (DAT-4.D):** Use a two-proportion CI to justify or refute a claim
- **Essential Knowledge:**
  - If 0 is in the interval for $p_1 - p_2$: no convincing evidence of a difference
  - If 0 is NOT in the interval: convincing evidence that $p_1 \neq p_2$
  - If the entire interval is positive: evidence that $p_1 > p_2$
  - If the entire interval is negative: evidence that $p_1 < p_2$

### 6.10 Setting Up a Test for the Difference of Two Proportions
- **Learning Objective (VAR-6.H):** Set up hypotheses for a two-proportion z-test
- **Essential Knowledge:**
  - $H_0: p_1 = p_2$ (or equivalently $p_1 - p_2 = 0$)
  - $H_a: p_1 \neq p_2$ (two-sided), $p_1 > p_2$ (one-sided), or $p_1 < p_2$ (one-sided)
  - Under $H_0$, use the **pooled proportion:** $\hat{p}_c = \frac{X_1 + X_2}{n_1 + n_2}$

### 6.11 Carrying Out a Test for the Difference of Two Proportions
- **Learning Objective (DAT-4.E):** Carry out and interpret a two-proportion z-test
- **Essential Knowledge:**
  - **Test statistic:**
    $$z = \frac{(\hat{p}_1 - \hat{p}_2) - 0}{\sqrt{\hat{p}_c(1-\hat{p}_c)\left(\frac{1}{n_1} + \frac{1}{n_2}\right)}}$$
  - Conditions: same as 6.8, but use $\hat{p}_c$ for large counts check
  - Conclusion follows the same logic as 6.6 (compare p-value to $\alpha$)

## Common Misconceptions
- Using $\hat{p}$ instead of $p_0$ when checking conditions for a hypothesis test (use $p_0$ under $H_0$)
- Using $\hat{p}$ instead of the pooled $\hat{p}_c$ in the two-proportion z-test
- Misinterpreting confidence level: "95% confident" does NOT mean 95% probability the parameter is in this specific interval
- Saying "accept $H_0$" instead of "fail to reject $H_0$"
- Confusing statistical significance with practical significance
- Thinking a p-value is the probability that $H_0$ is true
