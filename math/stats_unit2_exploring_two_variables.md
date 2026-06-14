# Unit 2: Exploring Two-Variable Data
> Exam Weight: 5–7% | ~10–11 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Bivariate quantitative content now in **new Unit 5 (Regression Analysis)**; two-categorical analysis moved to new Unit 2. Topic 2.9 (departures from linearity) removed from the course. See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 2.1 Questions About Two Variables
When a dataset records two variables per individual, the natural question is whether — and how — those variables are related.
- Two-variable (bivariate) data consist of pairs of measurements on the same individual
- A relationship between two variables is described as an association
- Association does not imply causation

### 2.2 Two Categorical Variables in a Table
A two-way table organizes counts for combinations of two categorical variables.
- A **two-way table** (contingency table) shows counts at the intersection of each row category and column category
- **Joint relative frequencies:** each cell count divided by the grand total
- **Marginal relative frequencies:** row or column totals divided by the grand total
- **Conditional relative frequencies:** a cell count divided by its row total or column total

### 2.3 Association Between Categorical Variables
Comparing conditional distributions reveals whether two categorical variables are associated.
- If the conditional distributions across categories look similar, the variables are likely not associated
- If conditional distributions differ substantially, there is evidence of an association
- **Simpson's Paradox:** a trend visible in separate groups can reverse or disappear when those groups are combined — a lurking variable is typically responsible
- Side-by-side or segmented bar charts are useful for visualizing conditional distributions

### 2.4 Scatterplots for Two Quantitative Variables
A scatterplot displays the relationship between two quantitative variables, one on each axis.
- By convention, the **explanatory (independent) variable** goes on the x-axis and the **response (dependent) variable** on the y-axis
- Describe a scatterplot by its **direction** (positive or negative), **form** (linear or curved), **strength** (weak, moderate, strong), and any **unusual features** (outliers, clusters)

### 2.5 Correlation
The correlation coefficient $r$ measures the strength and direction of a linear association.
- **Pearson correlation:** $r = \frac{1}{n-1} \sum \left(\frac{x_i - \bar{x}}{s_x}\right)\left(\frac{y_i - \bar{y}}{s_y}\right)$
- Properties:
  - $-1 \leq r \leq 1$; positive values signal a positive association, negative values a negative one
  - $|r|$ near 1 indicates a strong linear relationship; near 0 indicates a weak one
  - $r$ has no units and is unaffected by changes in scale or which variable is labeled $x$ or $y$
  - $r$ is sensitive to outliers
- $r$ only captures **linear** association — a perfectly curved relationship may have $r \approx 0$

### 2.6 Linear Regression Models
A least-squares regression line (LSRL) models the linear relationship between two quantitative variables.
- **Population model:** $y = \alpha + \beta x + \varepsilon$
- **Estimated LSRL:** $\hat{y} = a + bx$
- **Slope $b$:** for each one-unit increase in $x$, the predicted $y$ changes by $b$ units
- **Intercept $a$:** the predicted $y$ when $x = 0$ (may lack practical meaning in context)
- Formulas: $b = r \cdot \frac{s_y}{s_x}$ and $a = \bar{y} - b\bar{x}$
- The LSRL always passes through $(\bar{x}, \bar{y})$
- **Extrapolation:** predicting $y$ for $x$ values outside the observed range is unreliable and should be avoided

### 2.7 Residuals
A residual measures how far an observed value deviates from the model's prediction.
- **Residual:** $e = y - \hat{y}$ (observed minus predicted)
- Positive residual: the model underpredicted; negative residual: the model overpredicted
- The sum of all residuals for a least-squares line equals zero: $\sum e_i = 0$

### 2.8 Assessing Model Fit
Two key tools evaluate how well the LSRL describes the data.
- **Coefficient of determination ($r^2$):** the proportion of variation in $y$ that is explained by its linear relationship with $x$
- Interpretation template: "About $r^2 \times 100\%$ of the variation in [y] is accounted for by the linear model with [x]"
- **Residual plot:** residuals graphed against $x$ (or $\hat{y}$) — a good model leaves no pattern, only random scatter around zero
- A curved residual pattern suggests a nonlinear model may fit better
- $s$ (standard deviation of residuals) describes the typical size of prediction errors

### 2.9 Departures from Linearity
Influential observations and nonlinear patterns can distort regression results.
- **Outlier:** a point that falls far from the overall pattern
- **High-leverage point:** a point with an $x$-value far from $\bar{x}$; it has the potential to pull the regression line
- **Influential point:** a point whose removal substantially changes the slope, intercept, or $r$; high-leverage points are often (but not always) influential
- **Transformations** for nonlinear data: applying $\log$, $\sqrt{}$, or reciprocal to $x$ and/or $y$ can linearize the relationship
- Common cases: power model ($y = ax^b$) → plot $\log y$ vs. $\log x$; exponential model ($y = ab^x$) → plot $\log y$ vs. $x$

## Common Misconceptions
- Correlation measures association, not causation — a high $r$ does not mean $x$ causes $y$
- $r^2$ and $r$ answer different questions — $r^2$ is the proportion of explained variation, while $r$ describes the direction and strength of the linear association
- $r$ measures only **linear** associations — strong nonlinear relationships can have $r$ near 0
- Predictions from the LSRL are only trustworthy within the range of observed data; extrapolating outside that range is risky
- Overlooking influential points can lead to a regression line that misrepresents the bulk of the data
