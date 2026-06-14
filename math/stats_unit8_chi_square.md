# Unit 8: Inference for Categorical Data: Chi-Square
> Exam Weight: 2–5% | ~8–10 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Homogeneity and independence tests now in **new Unit 3 (3.14–3.15)**. The goodness of fit test was removed from the course. See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 8.1 When Chi-Square Tests Are Needed
Chi-square tests compare observed categorical counts to expected counts, detecting departures from a claimed distribution or independence.
- The **chi-square distribution** is right-skewed and always non-negative
- Larger chi-square values correspond to more evidence against $H_0$
- Three chi-square tests: Goodness of Fit, Homogeneity, Independence

### 8.2 Chi-Square Goodness of Fit Test: Setup
The goodness of fit test asks whether a single categorical variable follows a claimed distribution.
- **Hypotheses:**
  - $H_0$: The distribution of [variable] matches the claimed distribution (state the specific proportions)
  - $H_a$: The distribution does not match the claimed distribution
- **Expected counts:** $E_i = n \cdot p_i$, where $p_i$ is the hypothesized proportion for category $i$
- **Conditions:**
  1. Random sample or randomized experiment
  2. Independence (10% condition)
  3. Large counts: all expected counts $\geq 5$

### 8.3 Chi-Square Goodness of Fit Test: Execution
- **Test statistic:**
  $$\chi^2 = \sum_{i=1}^{k} \frac{(O_i - E_i)^2}{E_i}$$
  where $O_i$ = observed count and $E_i$ = expected count for category $i$
- **Degrees of freedom:** $df = k - 1$ (where $k$ = number of categories)
- **p-value:** area to the right of $\chi^2$ under the chi-square distribution with $df = k - 1$
- Chi-square tests are always **one-sided** (right tail) — any deviation from expected counts increases $\chi^2$
- To identify which categories drive the result, examine individual $\frac{(O - E)^2}{E}$ contributions

### 8.4 Expected Counts in Two-Way Tables
For a two-way table, expected counts represent what the data would look like if $H_0$ were true.
- For a table with $r$ rows and $c$ columns:
  $$E_{ij} = \frac{(\text{row } i \text{ total}) \times (\text{column } j \text{ total})}{\text{grand total}}$$
- Expected counts reflect the $H_0$ assumption (no association, or same distribution across groups)

### 8.5 Chi-Square Tests for Homogeneity and Independence: Setup
Two different research questions use the same two-way table test statistic.
- **Test for Homogeneity:**
  - Compares the distribution of one categorical variable across two or more separate populations or groups
  - Data come from separate random samples (or separate treatment groups in an experiment)
  - $H_0$: The distribution of [variable] is the same across all groups
  - $H_a$: The distribution differs across at least one group
- **Test for Independence:**
  - Asks whether two categorical variables are associated within a single population
  - Data come from one random sample, with two variables recorded per individual
  - $H_0$: [Variable 1] and [Variable 2] are independent (no association)
  - $H_a$: [Variable 1] and [Variable 2] are not independent (there is an association)
- **Conditions (same for both):** Random, Independence (10% condition), Large counts (all expected counts $\geq 5$)

### 8.6 Chi-Square Tests for Homogeneity and Independence: Execution
Both tests use the same formula and the same procedure.
- **Test statistic:**
  $$\chi^2 = \sum_{\text{all cells}} \frac{(O_{ij} - E_{ij})^2}{E_{ij}}$$
- **Degrees of freedom:** $df = (r - 1)(c - 1)$
- **p-value:** area to the right of $\chi^2$ under the chi-square distribution with $df = (r-1)(c-1)$
- When rejecting $H_0$, examine which cells contribute most to $\chi^2$ and describe the nature of the association using conditional proportions
- **Conclusion template:** "Because the p-value of ___ is [less/greater] than $\alpha = ___$, we [reject/fail to reject] $H_0$. We [do/do not] have convincing evidence that [context]."

## Choosing the Right Chi-Square Test

| Feature | Goodness of Fit | Homogeneity | Independence |
|---------|----------------|-------------|--------------|
| **Number of variables** | 1 | 1 | 2 |
| **Number of populations** | 1 | 2 or more | 1 |
| **Data structure** | One-way table | Two-way table | Two-way table |
| **$df$** | $k - 1$ | $(r-1)(c-1)$ | $(r-1)(c-1)$ |
| **Question** | Does this distribution match a claim? | Is the distribution the same across groups? | Are the two variables associated? |

## Common Misconceptions
- Confusing the test for homogeneity with the test for independence — the formula is identical but the research design and question differ
- Applying chi-square when some expected counts fall below 5 — the approximation breaks down; merge categories to fix this
- Treating chi-square as a two-sided test — it is always right-tailed (any deviation from expected increases the statistic)
- Forgetting to compute expected counts before comparing — observed counts alone are not sufficient
- Drawing causal conclusions from a chi-square test of independence — association does not imply causation unless random assignment was used
- Confusing observed and expected counts in the $\frac{(O-E)^2}{E}$ formula
