# Unit 9: Inference for Quantitative Data: Slopes
> Exam Weight: 2–5% | ~7–8 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). This unit was **removed from the course** — formal inference for regression slopes is no longer tested. See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 9.1 Why We Need Inference for Regression Slopes
A sample regression slope $b$ is a statistic that estimates the population slope $\beta$; because samples vary, a non-zero $b$ does not automatically mean $\beta \neq 0$.
- The key question: Is the linear relationship observed in the sample evidence of a real relationship in the population, or could it arise by chance?
- Inference provides a principled answer

### 9.2 Confidence Interval for a Regression Slope
A t-interval for $\beta$ estimates the plausible range of the true slope.
- **t-interval for the slope:**
  $$b \pm t^* \cdot SE_b$$
- **Degrees of freedom:** $df = n - 2$
- $SE_b$ is reported in computer output; calculating it by hand is not expected
- **Interpretation:** "We are C% confident that the true slope of the linear relationship between [x] and [y] is between [lower] and [upper]"
- In context: "For each one-unit increase in [x], [y] changes by between [lower] and [upper] units on average"

### 9.3 Using a Slope Interval to Evaluate a Claim
- If 0 falls inside the interval: insufficient evidence of a linear relationship in the population
- If 0 is outside the interval: convincing evidence that the slope is not zero — a linear relationship exists
- The direction and width of the interval reveal the plausible strength and direction of the relationship

### 9.4 Setting Up a t-Test for the Slope
A t-test evaluates whether a linear relationship exists in the population.
- **Hypotheses:**
  - $H_0: \beta = 0$ (no linear relationship between $x$ and $y$)
  - $H_a: \beta \neq 0$ (two-sided), $\beta > 0$, or $\beta < 0$ (one-sided)
- **Conditions (LINE):**
  1. **Linearity:** the true relationship is linear — check the scatterplot and residual plot
  2. **Independence:** observations are independent — random sample, 10% condition
  3. **Normality:** for a given $x$, the $y$-values are normally distributed — check the residual plot for strong skewness or outliers
  4. **Equal variance:** the variability of $y$ is consistent across all values of $x$ — check the residual plot for a fan or funnel shape
  - Random selection or assignment is also required

### 9.5 Carrying Out a t-Test for the Slope
- **Test statistic:**
  $$t = \frac{b - 0}{SE_b}$$
- **Degrees of freedom:** $df = n - 2$
- p-value from the t-distribution with $df = n - 2$; computer output typically reports both $t$ and the two-sided p-value
- **Conclusion template:** "Because the p-value of ___ is [less/greater] than $\alpha = ___$, we [reject/fail to reject] $H_0$. We [do/do not] have convincing evidence of a linear relationship between [x] and [y]."

## Reading Computer Output

Students should be able to extract relevant values from a standard regression table:

```
Predictor    Coef      SE Coef     T        P
Constant     a         SE_a        t_a      p_a
x            b         SE_b        t_b      p_b

S = ___    R-Sq = ___    R-Sq(adj) = ___
```

- **Coef column:** $a$ (intercept) and $b$ (slope)
- **SE Coef column:** standard errors of the estimates
- **T column:** t-test statistics
- **P column:** two-sided p-values for the test $H_0: \beta = 0$
- **S:** standard deviation of residuals ($s = \sqrt{\frac{\sum e_i^2}{n-2}}$)
- **R-Sq:** coefficient of determination ($r^2$)

## Key Formulas

| Quantity | Formula |
|----------|---------|
| Slope estimate | $b = r \cdot \frac{s_y}{s_x}$ |
| Standard error of slope | $SE_b$ provided in computer output |
| Test statistic | $t = \frac{b}{SE_b}$ (when $\beta_0 = 0$) |
| Confidence interval | $b \pm t^* \cdot SE_b$ |
| Degrees of freedom | $df = n - 2$ |

## Common Misconceptions
- Skipping the LINE conditions before inference — especially checking residual plots for linearity, equal variance, and normality
- Confusing $r$ (correlation) with $b$ (slope) — they share the same sign but have different magnitudes and units
- Interpreting a non-significant slope as "no relationship" — it means no convincing evidence of a **linear** relationship; a nonlinear pattern could still exist
- Using $df = n - 1$ instead of $df = n - 2$ for slope inference
- Attempting to compute $SE_b$ manually — it is always provided in the computer output on the exam
- Applying a one-sided p-value when the computer output gives a two-sided one — divide by 2 if the alternative is one-sided
