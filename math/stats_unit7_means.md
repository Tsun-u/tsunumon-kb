# Unit 7: Inference for Quantitative Data: Means
> Exam Weight: 10–18% | ~14–16 Class Periods

## Topics

### 7.1 Introducing Statistics: Should I Worry About Error?
- **Learning Objective (UNC-4.E):** Understand sampling error and the need for inference about means
- **Essential Knowledge:**
  - Sample means vary from sample to sample due to sampling variability
  - We use sample data to make inferences about unknown population means
  - When $\sigma$ is unknown (almost always in practice), we use the **t-distribution** instead of the z-distribution

### 7.2 Constructing a Confidence Interval for a Population Mean
- **Learning Objective (UNC-4.F):** Construct a confidence interval for a population mean
- **Essential Knowledge:**
  - **One-sample t-interval for $\mu$:**
    $$\bar{x} \pm t^* \frac{s}{\sqrt{n}}$$
  - **Degrees of freedom:** $df = n - 1$
  - **Conditions:**
    1. **Random:** data come from a random sample or randomized experiment
    2. **Independence (10% condition):** $n < 10\%$ of population
    3. **Normal/Large Sample:** population is normal, OR $n \geq 30$ (CLT), OR graph of data shows no strong skew or outliers
  - The **t-distribution** is symmetric, bell-shaped, centered at 0, but has heavier tails than the standard normal
  - As $df$ increases, the t-distribution approaches the standard normal distribution
  - **Standard error:** $SE_{\bar{x}} = \frac{s}{\sqrt{n}}$

### 7.3 Justifying a Claim Based on a Confidence Interval for a Mean
- **Learning Objective (DAT-4.F):** Use a confidence interval for a mean to justify or refute a claim
- **Essential Knowledge:**
  - If the claimed value of $\mu$ falls inside the CI → no convincing evidence against the claim
  - If the claimed value falls outside the CI → convincing evidence that $\mu$ differs from the claimed value
  - Interpretation: "We are C% confident that the true mean of [context] is between [lower] and [upper]"

### 7.4 Setting Up a Test for a Population Mean
- **Learning Objective (VAR-6.I):** Set up hypotheses for a one-sample t-test
- **Essential Knowledge:**
  - $H_0: \mu = \mu_0$
  - $H_a: \mu \neq \mu_0$, $\mu > \mu_0$, or $\mu < \mu_0$
  - Same conditions as 7.2 (Random, Independence, Normal/Large Sample)
  - Use the **t-test** because $\sigma$ is unknown and estimated by $s$

### 7.5 Carrying Out a Test for a Population Mean
- **Learning Objective (DAT-4.G):** Calculate the test statistic and p-value for a one-sample t-test
- **Essential Knowledge:**
  - **Test statistic:** $t = \frac{\bar{x} - \mu_0}{s / \sqrt{n}}$ with $df = n - 1$
  - Find the p-value using the t-distribution with $df = n - 1$
  - Compare p-value to $\alpha$ and make a conclusion in context

### 7.6 Confidence Interval for the Difference of Two Means
- **Learning Objective (UNC-4.G):** Construct a confidence interval for $\mu_1 - \mu_2$
- **Essential Knowledge:**
  - **Two-sample t-interval:**
    $$(\bar{x}_1 - \bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$$
  - **Degrees of freedom:** Use calculator/technology (Welch's approximation) or conservative $df = \min(n_1 - 1, n_2 - 1)$
  - **Conditions:** Random (both samples), Independence (10% for both), Normal/Large Sample (both groups)
  - Do NOT assume equal variances (do NOT pool standard deviations) — use Welch's t

### 7.7 Setting Up a Test for the Difference of Two Means
- **Learning Objective (VAR-6.J):** Set up hypotheses for a two-sample t-test
- **Essential Knowledge:**
  - $H_0: \mu_1 = \mu_2$ (equivalently $\mu_1 - \mu_2 = 0$)
  - $H_a: \mu_1 \neq \mu_2$, $\mu_1 > \mu_2$, or $\mu_1 < \mu_2$
  - Two-sample t-tests compare means from two independent groups

### 7.8 Carrying Out a Test for the Difference of Two Means
- **Learning Objective (DAT-4.H):** Calculate the test statistic and p-value for a two-sample t-test
- **Essential Knowledge:**
  - **Test statistic:**
    $$t = \frac{(\bar{x}_1 - \bar{x}_2) - 0}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}$$
  - Degrees of freedom from technology (Welch's formula) or $df = \min(n_1 - 1, n_2 - 1)$
  - Compare p-value to $\alpha$; conclude in context

### 7.9 Matched Pairs Design
- **Learning Objective (VAR-6.K):** Perform inference for matched pairs
- **Essential Knowledge:**
  - **Matched pairs:** each subject serves as its own control, or subjects are paired based on similar characteristics
  - Analyze the **differences** within each pair: $d_i = x_{1i} - x_{2i}$
  - Treat the differences as a **single sample** and use a **one-sample t-procedure** on $\bar{d}$
  - **t-interval for matched pairs:** $\bar{d} \pm t^* \frac{s_d}{\sqrt{n}}$ with $df = n - 1$ (where $n$ = number of pairs)
  - **t-test for matched pairs:** $t = \frac{\bar{d} - 0}{s_d / \sqrt{n}}$ with $df = n - 1$
  - Conditions: Random assignment/selection of pairs, Independence of pairs, Normal/Large Sample for differences

### 7.10 Choosing an Appropriate Inference Procedure
- **Learning Objective (DAT-4.I):** Select the appropriate inference procedure
- **Essential Knowledge:**
  - **One-sample t:** one group, inference about one population mean
  - **Two-sample t:** two independent groups, comparing two population means
  - **Matched pairs t:** paired data (differences), effectively one-sample t on differences
  - Key decision: Are the samples independent or paired?
  - Always state hypotheses, check conditions, calculate test statistic, find p-value, and conclude in context (the "4-step process")

## The 4-Step Inference Process

1. **State:** Define parameters, state hypotheses ($H_0$ and $H_a$)
2. **Plan:** Identify the procedure, check conditions
3. **Do:** Calculate the test statistic and p-value (or construct CI)
4. **Conclude:** Make a decision and interpret in context

## Common Misconceptions
- Using z instead of t when $\sigma$ is unknown — always use t in practice
- Confusing two-sample t-test with matched pairs — check if data are independent or paired
- Pooling standard deviations in a two-sample t-test — do NOT pool unless explicitly told to assume equal variances
- Forgetting to check the Normal/Large Sample condition — graph the data to assess
- Interpreting the confidence interval as the probability the parameter is in the interval
- Not defining the parameter ($\mu$) clearly in context before stating hypotheses
