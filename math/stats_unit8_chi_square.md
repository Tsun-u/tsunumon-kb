# Unit 8: Inference for Categorical Data: Chi-Square
> Exam Weight: 2–5% | ~8–10 Class Periods

## Topics

### 8.1 Introducing Statistics: Are My Results Unexpected?
- **Learning Objective (UNC-4.H):** Understand when chi-square tests are appropriate
- **Essential Knowledge:**
  - Chi-square tests are used to analyze **categorical** data — comparing observed counts to expected counts
  - The chi-square distribution is **right-skewed** and always non-negative
  - Larger chi-square values provide stronger evidence against $H_0$
  - Three types of chi-square tests: Goodness of Fit, Homogeneity, Independence

### 8.2 Setting Up a Chi-Square Goodness of Fit Test
- **Learning Objective (VAR-7.A):** Set up hypotheses for a chi-square goodness of fit test
- **Essential Knowledge:**
  - **Purpose:** test whether the distribution of a single categorical variable matches a claimed distribution
  - **Hypotheses:**
    - $H_0:$ The distribution of [variable] matches the claimed distribution (state specific proportions)
    - $H_a:$ The distribution of [variable] does NOT match the claimed distribution
  - **Expected counts:** $E_i = n \cdot p_i$ where $p_i$ is the hypothesized proportion for category $i$
  - **Conditions:**
    1. **Random:** data come from a random sample or randomized experiment
    2. **Independence (10% condition):** $n < 10\%$ of population
    3. **Large counts:** all expected counts $\geq 5$

### 8.3 Carrying Out a Chi-Square Goodness of Fit Test
- **Learning Objective (DAT-4.J):** Calculate and interpret the chi-square GOF test
- **Essential Knowledge:**
  - **Chi-square test statistic:**
    $$\chi^2 = \sum_{i=1}^{k} \frac{(O_i - E_i)^2}{E_i}$$
    where $O_i$ = observed count and $E_i$ = expected count for category $i$
  - **Degrees of freedom:** $df = k - 1$ (where $k$ = number of categories)
  - p-value: area to the right of $\chi^2$ under the chi-square distribution with $df = k - 1$
  - Chi-square tests are always **one-sided** (right tail) — any deviation from expected increases $\chi^2$
  - Identify which categories contribute most to $\chi^2$ by examining individual $(O - E)^2 / E$ terms

### 8.4 Expected Counts in Two-Way Tables
- **Learning Objective (VAR-7.B):** Calculate expected counts for two-way tables
- **Essential Knowledge:**
  - For a two-way table with $r$ rows and $c$ columns:
    $$E_{ij} = \frac{(\text{row } i \text{ total}) \times (\text{column } j \text{ total})}{\text{grand total}}$$
  - Expected counts represent what we would expect to see if the null hypothesis were true (no association or same distribution)
  - Compare observed and expected counts to determine if there is evidence of an association

### 8.5 Setting Up a Chi-Square Test for Homogeneity or Independence
- **Learning Objective (VAR-7.C):** Distinguish between and set up chi-square tests for homogeneity and independence
- **Essential Knowledge:**
  - **Chi-Square Test for Homogeneity:**
    - Compares the distribution of **one categorical variable** across **two or more independent populations/groups**
    - Data come from **separate random samples** (or separate treatment groups in an experiment)
    - $H_0:$ The distribution of [variable] is the **same** across all populations
    - $H_a:$ The distribution of [variable] is **not the same** across all populations
  - **Chi-Square Test for Independence (Association):**
    - Tests whether two categorical variables are **associated** within **one population**
    - Data come from **one random sample**, and two variables are recorded for each individual
    - $H_0:$ [Variable 1] and [Variable 2] are **independent** (no association)
    - $H_a:$ [Variable 1] and [Variable 2] are **not independent** (there is an association)
  - **Conditions (same for both):**
    1. Random sample(s) or randomized experiment
    2. Independence (10% condition)
    3. Large counts: all expected counts $\geq 5$

### 8.6 Carrying Out a Chi-Square Test for Homogeneity or Independence
- **Learning Objective (DAT-4.K):** Calculate and interpret chi-square tests for homogeneity and independence
- **Essential Knowledge:**
  - **Test statistic (same formula for both):**
    $$\chi^2 = \sum_{\text{all cells}} \frac{(O_{ij} - E_{ij})^2}{E_{ij}}$$
  - **Degrees of freedom:** $df = (r - 1)(c - 1)$
  - p-value: area to the right of $\chi^2$ under chi-square distribution with $df = (r-1)(c-1)$
  - When rejecting $H_0$, examine which cells have the largest contributions to $\chi^2$ and describe the nature of the association using conditional proportions
  - Conclusion template: "Because the p-value of ___ is [less/greater] than $\alpha = ___$, we [reject/fail to reject] $H_0$. We [do/do not] have convincing evidence that [context]."

## Choosing the Right Chi-Square Test

| Feature | Goodness of Fit | Homogeneity | Independence |
|---------|----------------|-------------|--------------|
| **Number of variables** | 1 | 1 | 2 |
| **Number of populations** | 1 | 2 or more | 1 |
| **Data structure** | One-way table | Two-way table | Two-way table |
| **$df$** | $k - 1$ | $(r-1)(c-1)$ | $(r-1)(c-1)$ |
| **Question** | Does the distribution match a claim? | Is the distribution the same across groups? | Are the two variables associated? |

## Common Misconceptions
- Confusing the test for homogeneity with the test for independence — they use the same formula but answer different questions and arise from different study designs
- Using chi-square when expected counts are too small ($< 5$) — the approximation breaks down
- Thinking chi-square tests can be two-sided — they are always right-tailed
- Forgetting to compute expected counts using the formula (not the observed counts)
- Drawing causal conclusions from a chi-square test of independence — association is not causation (unless random assignment was used)
- Confusing observed and expected counts in the formula
