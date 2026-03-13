# Unit 2: Exploring Two-Variable Data
> Exam Weight: 5–7% | ~10–11 Class Periods

## Topics

### 2.1 Introducing Statistics: Are Two Variables Related?
- **Learning Objective (DAT-1.C):** Identify questions that involve exploring the relationship between two variables
- **Essential Knowledge:**
  - Two-variable (bivariate) data involve pairs of measurements on the same individual
  - The relationship between two variables may be described as an association
  - Association does not imply causation

### 2.2 Representing Two Categorical Variables
- **Learning Objective (UNC-1.G):** Represent the relationship between two categorical variables using a two-way table
- **Essential Knowledge:**
  - A **two-way table** (contingency table) displays counts for combinations of two categorical variables
  - **Joint relative frequencies:** proportions for each cell relative to the grand total
  - **Marginal relative frequencies:** row or column totals divided by the grand total
  - **Conditional relative frequencies:** cell counts divided by the row or column total

### 2.3 Statistics for Two Categorical Variables
- **Learning Objective (DAT-1.D):** Describe associations between two categorical variables using conditional relative frequencies
- **Essential Knowledge:**
  - Compare conditional distributions to assess whether two categorical variables are associated
  - If the conditional distributions are approximately the same across categories, the variables are **not associated**
  - **Simpson's Paradox:** an association between two variables can reverse when data are combined over a lurking variable
  - Side-by-side or segmented bar charts can display conditional distributions

### 2.4 Representing the Relationship Between Two Quantitative Variables
- **Learning Objective (DAT-2.A):** Represent bivariate quantitative data using a scatterplot
- **Essential Knowledge:**
  - A **scatterplot** displays the relationship between two quantitative variables
  - The **explanatory variable** (independent) goes on the x-axis; the **response variable** (dependent) goes on the y-axis
  - Describe scatterplots by **direction** (positive/negative), **form** (linear/nonlinear), **strength** (weak/moderate/strong), and **unusual features** (outliers, clusters)

### 2.5 Correlation
- **Learning Objective (DAT-2.B):** Calculate and interpret the correlation coefficient $r$
- **Essential Knowledge:**
  - **Correlation ($r$):** measures the strength and direction of a **linear** relationship between two quantitative variables
  - Formula: $r = \frac{1}{n-1} \sum \left(\frac{x_i - \bar{x}}{s_x}\right)\left(\frac{y_i - \bar{y}}{s_y}\right)$
  - Properties of $r$:
    - $-1 \leq r \leq 1$
    - $r > 0$: positive association; $r < 0$: negative association
    - $|r|$ close to 1: strong linear relationship; close to 0: weak linear relationship
    - $r$ has no units and is not affected by changes in units or which variable is $x$ or $y$
    - $r$ is sensitive to outliers
  - $r$ only measures **linear** association — a strong curved relationship may have $r \approx 0$

### 2.6 Linear Regression Models
- **Learning Objective (DAT-2.C):** Describe the linear regression model and interpret the slope and y-intercept
- **Essential Knowledge:**
  - The **population regression model:** $y = \alpha + \beta x + \varepsilon$
  - The **least-squares regression line (LSRL):** $\hat{y} = a + bx$
  - **Slope $b$:** For each unit increase in $x$, the predicted $y$ changes by $b$ units
  - **y-intercept $a$:** The predicted value of $y$ when $x = 0$ (may not be meaningful in context)
  - Formulas: $b = r \cdot \frac{s_y}{s_x}$ and $a = \bar{y} - b\bar{x}$
  - The LSRL always passes through the point $(\bar{x}, \bar{y})$
  - **Extrapolation:** using the regression line to predict outside the range of observed $x$ values — unreliable

### 2.7 Residuals
- **Learning Objective (DAT-2.D):** Calculate and interpret residuals
- **Essential Knowledge:**
  - **Residual:** $e = y - \hat{y}$ (observed minus predicted)
  - Positive residual: the model **underestimated** the actual value
  - Negative residual: the model **overestimated** the actual value
  - The sum of residuals for the LSRL is always 0: $\sum e_i = 0$

### 2.8 Least Squares Regression
- **Learning Objective (DAT-2.E):** Use residual plots and $r^2$ to assess model fit
- **Essential Knowledge:**
  - **Coefficient of determination ($r^2$):** the proportion of variability in $y$ that is explained by the linear relationship with $x$
  - Interpretation: "Approximately $r^2 \times 100\%$ of the variation in [y] is explained by the linear model with [x]"
  - **Residual plot:** plot residuals vs. $x$ (or $\hat{y}$) to check model appropriateness
  - A good model shows **no pattern** in the residual plot (random scatter around 0)
  - A curved pattern in the residual plot suggests a nonlinear model may be more appropriate
  - Standard deviation of residuals ($s$): measures the typical size of prediction errors

### 2.9 Departures from Linearity
- **Learning Objective (DAT-2.F):** Identify influential points and apply transformations
- **Essential Knowledge:**
  - **Outlier:** a point that does not follow the overall pattern
  - **High-leverage point:** a point with an $x$-value far from $\bar{x}$
  - **Influential point:** a point whose removal substantially changes the regression line, slope, or $r$
  - High-leverage points are often (but not always) influential
  - **Transformations** for nonlinear data: taking $\log$, $\sqrt{}$, or reciprocal of $x$ and/or $y$ to linearize the relationship
  - Common: power model ($y = ax^b$) → plot $\log y$ vs. $\log x$; exponential model ($y = ab^x$) → plot $\log y$ vs. $x$

## Common Misconceptions
- Confusing correlation with causation — $r$ measures association, not cause-and-effect
- Thinking $r^2$ and $r$ have the same interpretation — $r^2$ is the proportion of explained variation, not strength of association
- Forgetting that $r$ only measures **linear** relationships
- Extrapolating beyond the range of observed data
- Ignoring influential points that can dramatically alter the LSRL
