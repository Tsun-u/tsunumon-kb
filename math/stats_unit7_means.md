# Unit 7: Inference for Quantitative Data: Means
> Exam Weight: 10–18% | ~14–16 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content now in **new Unit 4**. See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 7.1 Inference About Means in Practice
Sample means vary from sample to sample; inference provides a framework for drawing conclusions about the unknown population mean $\mu$.
- When $\sigma$ is unknown (the usual case in practice), the t-distribution replaces the z-distribution
- t-based procedures are more appropriate and nearly always the right choice

### 7.2 Confidence Interval for a Population Mean
A one-sample t-interval estimates $\mu$ from sample data.
- **One-sample t-interval for $\mu$:**
  $$\bar{x} \pm t^* \frac{s}{\sqrt{n}}$$
- **Degrees of freedom:** $df = n - 1$
- **Conditions:**
  1. **Random:** data from a random sample or randomized experiment
  2. **Independence (10% condition):** $n < 10\%$ of the population
  3. **Normal/Large Sample:** population is normal, or $n \geq 30$ (CLT applies), or a graph of the data shows no strong skew or outliers
- The **t-distribution** is symmetric and bell-shaped like the normal, but with heavier tails; it approaches the standard normal as $df$ increases
- **Standard error of $\bar{x}$:** $SE_{\bar{x}} = \frac{s}{\sqrt{n}}$

### 7.3 Using a Confidence Interval for a Mean to Evaluate a Claim
- If the claimed value of $\mu$ falls inside the confidence interval: insufficient evidence against the claim
- If it falls outside: convincing evidence that the true mean differs from the claimed value
- **Interpretation template:** "We are C% confident that the true mean of [context] is between [lower] and [upper]"

### 7.4 Setting Up a One-Sample t-Test
A t-test evaluates whether sample data are consistent with a specific claim about $\mu$.
- $H_0: \mu = \mu_0$
- $H_a: \mu \neq \mu_0$ (two-sided), $\mu > \mu_0$, or $\mu < \mu_0$ (one-sided)
- Same conditions as 7.2 (Random, Independence, Normal/Large Sample)

### 7.5 Carrying Out a One-Sample t-Test
- **Test statistic:** $t = \frac{\bar{x} - \mu_0}{s / \sqrt{n}}$ with $df = n - 1$
- Find the p-value from the t-distribution with $df = n - 1$
- Compare the p-value to $\alpha$ and state a conclusion in context

### 7.6 Confidence Interval for the Difference Between Two Means
When comparing two groups, a two-sample t-interval estimates $\mu_1 - \mu_2$.
- **Two-sample t-interval:**
  $$(\bar{x}_1 - \bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}$$
- **Degrees of freedom:** use Welch's approximation (from technology) or the conservative $df = \min(n_1 - 1, n_2 - 1)$
- **Conditions:** Random and independence for both groups; Normal/Large Sample for both groups
- Do **not** assume equal variances or pool standard deviations — use Welch's t

### 7.7 Setting Up a Two-Sample t-Test
- $H_0: \mu_1 = \mu_2$ (equivalently $\mu_1 - \mu_2 = 0$)
- $H_a: \mu_1 \neq \mu_2$, $\mu_1 > \mu_2$, or $\mu_1 < \mu_2$
- Two-sample t-tests compare means from two **independent** groups

### 7.8 Carrying Out a Two-Sample t-Test
- **Test statistic:**
  $$t = \frac{(\bar{x}_1 - \bar{x}_2) - 0}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}$$
- Degrees of freedom from technology (Welch's) or conservative $df = \min(n_1 - 1, n_2 - 1)$
- Compare p-value to $\alpha$ and conclude in context

### 7.9 Matched Pairs
When data consist of natural pairs or repeated measures, analyze the within-pair differences.
- **Matched pairs:** each subject is its own control, or subjects are paired by similar characteristics
- Compute the difference for each pair: $d_i = x_{1i} - x_{2i}$
- Treat the differences as a single sample; apply a **one-sample t-procedure** to $\bar{d}$
- **t-interval:** $\bar{d} \pm t^* \frac{s_d}{\sqrt{n}}$, $df = n - 1$ (where $n$ = number of pairs)
- **t-test statistic:** $t = \frac{\bar{d} - 0}{s_d / \sqrt{n}}$, $df = n - 1$
- Conditions: random selection/assignment of pairs, independence of pairs, Normal/Large Sample for the differences

### 7.10 Choosing the Right Procedure for Means
- **One-sample t:** one group; making a claim about one population mean
- **Two-sample t:** two independent groups; comparing two population means
- **Matched pairs t:** paired data; treated as one-sample t on the differences
- Critical decision: Are the two samples independent or paired?
- Every inference solution should follow the same structure: State, Plan, Do, Conclude (SPDC)

## The 4-Step Inference Process

1. **State:** define parameters; write $H_0$ and $H_a$ (for tests) or the parameter of interest (for intervals)
2. **Plan:** name the procedure; verify conditions
3. **Do:** compute the test statistic and p-value, or construct the interval
4. **Conclude:** decide and interpret in context

## Common Misconceptions
- Using z instead of t when $\sigma$ is unknown — always use t in practice
- Confusing paired and two-sample designs — check whether observations are linked in pairs or come from independent groups
- Pooling standard deviations in a two-sample t-test — do not pool unless explicitly instructed to assume equal variances
- Skipping the Normal/Large Sample condition — graph the data before assuming normality
- Interpreting a confidence interval as a probability statement about the specific interval computed
- Defining the parameter vaguely — always state $\mu$ clearly in context before testing
