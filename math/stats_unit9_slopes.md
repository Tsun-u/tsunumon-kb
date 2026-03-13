# Unit 9: Inference for Quantitative Data: Slopes
> Exam Weight: 2–5% | ~7–8 Class Periods

## Topics

### 9.1 Introducing Statistics: Do Those Points Align?
- **Learning Objective (UNC-4.I):** Understand the need for inference about regression slopes
- **Essential Knowledge:**
  - A sample regression slope $b$ is a statistic that estimates the population slope $\beta$
  - Just because a sample shows a non-zero slope does not mean the population slope is non-zero — we need inference
  - The key question: Is the observed linear relationship in the sample due to a real association in the population, or just chance?

### 9.2 Confidence Intervals for the Slope of a Regression Model
- **Learning Objective (UNC-4.J):** Construct a confidence interval for the slope of a regression model
- **Essential Knowledge:**
  - **t-interval for the slope:**
    $$b \pm t^* \cdot SE_b$$
  - **Degrees of freedom:** $df = n - 2$
  - $SE_b$ is typically provided in computer output (no need to calculate by hand)
  - **Interpretation:** "We are C% confident that the true slope of the linear relationship between [x] and [y] is between [lower] and [upper]"
  - In context: "For each one-unit increase in [x], [y] changes by between [lower] and [upper] units, on average"

### 9.3 Justifying a Claim About the Slope
- **Learning Objective (DAT-4.L):** Use a confidence interval for a slope to justify or refute a claim
- **Essential Knowledge:**
  - If 0 is in the confidence interval → no convincing evidence of a linear relationship
  - If 0 is NOT in the interval → convincing evidence that the slope is not zero (i.e., a linear relationship exists)
  - The sign and range of the interval tell us about the direction and plausible strength of the relationship

### 9.4 Setting Up a Test for the Slope of a Regression Model
- **Learning Objective (VAR-7.D):** Set up hypotheses for a t-test for the slope
- **Essential Knowledge:**
  - **Hypotheses:**
    - $H_0: \beta = 0$ (no linear relationship between $x$ and $y$)
    - $H_a: \beta \neq 0$ (two-sided), $\beta > 0$, or $\beta < 0$ (one-sided)
  - **Conditions (LINE/LINER):**
    1. **L — Linearity:** the true relationship is linear (check scatterplot and residual plot)
    2. **I — Independence:** observations are independent (random sample + 10% condition)
    3. **N — Normality:** for a given $x$, the responses ($y$-values) are normally distributed (check residual plot for normality — no strong skew or outliers)
    4. **E — Equal variance (constant variance):** the variability of $y$ is the same for all values of $x$ (check residual plot for constant spread — no fan/funnel shape)
    5. **R — Randomness:** data come from a random sample or randomized experiment

### 9.5 Carrying Out a Test for the Slope of a Regression Model
- **Learning Objective (DAT-4.M):** Calculate and interpret the t-test for a slope
- **Essential Knowledge:**
  - **Test statistic:**
    $$t = \frac{b - \beta_0}{SE_b} = \frac{b - 0}{SE_b}$$
  - **Degrees of freedom:** $df = n - 2$
  - p-value from the t-distribution with $df = n - 2$
  - $SE_b$ and often $t$ and p-value are provided in regression computer output
  - **Conclusion template:** "Because the p-value of ___ is [less/greater] than $\alpha = ___$, we [reject/fail to reject] $H_0$. We [do/do not] have convincing evidence of a linear relationship between [x variable] and [y variable]."

## Reading Computer Output

Students are expected to read and interpret standard regression output tables:

```
Predictor    Coef      SE Coef     T        P
Constant     a         SE_a        t_a      p_a
x            b         SE_b        t_b      p_b

S = ___    R-Sq = ___    R-Sq(adj) = ___
```

- **Coef** column: $a$ (intercept) and $b$ (slope)
- **SE Coef** column: standard errors of the estimates
- **T** column: t-test statistics
- **P** column: p-values (for the two-sided test $H_0: \beta = 0$)
- **S**: standard deviation of residuals ($s = \sqrt{\frac{\sum e_i^2}{n-2}}$)
- **R-Sq**: coefficient of determination ($r^2$)

## Key Formulas

| Quantity | Formula |
|----------|---------|
| Slope estimate | $b = r \cdot \frac{s_y}{s_x}$ |
| Standard error of slope | $SE_b = \frac{s}{\sqrt{\sum (x_i - \bar{x})^2}}$ (provided in output) |
| Test statistic | $t = \frac{b}{SE_b}$ (when $\beta_0 = 0$) |
| Confidence interval | $b \pm t^* \cdot SE_b$ |
| Degrees of freedom | $df = n - 2$ |

## Common Misconceptions
- Forgetting to check the LINE conditions before performing inference — especially checking residual plots
- Confusing $r$ (correlation) with $b$ (slope) — they have the same sign but different magnitudes
- Thinking a non-significant slope means "no relationship" — it means no convincing evidence of a **linear** relationship (a nonlinear relationship could still exist)
- Not using $df = n - 2$ (using $n - 1$ instead, which is for means)
- Trying to compute $SE_b$ by hand — it is always provided in computer output on the AP exam
- Confusing the p-value from the output (which tests $\beta = 0$) with a different hypothesis — if $H_a$ is one-sided, divide the two-sided p-value by 2
