# AP Statistics (2026-27 CED) -- Unit 5: Regression Analysis

> Exam Weight: 10–20% | ~9 Class Periods
> This unit focuses on describing relationships between two quantitative variables: scatterplots, correlation, and least-squares regression. Formal inference for regression slopes is not included in the 2026-27 course.

## Topics

### 5.1 Graphical Representations Between Two Quantitative Variables
- **Scatterplots** display pairs of quantitative measurements; by convention the explanatory variable goes on the x-axis and the response variable on the y-axis
- When describing a scatterplot, address direction (positive or negative), form (linear or curved), strength of the pattern, and any unusual features such as outliers or clusters

### 5.2 Correlation
- The **correlation coefficient** $r$ quantifies both the direction and the strength of a **linear** relationship between two quantitative variables; it is bounded by $-1 \leq r \leq 1$
- $r$ is dimensionless, so it does not change when units are converted, but it is sensitive to outliers
- **A strong correlation does not establish a cause-and-effect relationship**

### 5.3 Linear Regression Models
- The least-squares regression line (LSRL) takes the form $\hat{y} = a + bx$ and can be used to predict $y$ for a given $x$
- **Interpolation** (predicting within the observed range) is generally reasonable; **extrapolation** (predicting well beyond the data) is unreliable
- The slope $b$ is interpreted as the predicted change in $y$ for each one-unit increase in $x$; the intercept $a$ is the predicted value of $y$ when $x = 0$

### 5.4 Residuals
- A **residual** measures prediction error: $\text{residual} = y - \hat{y}$ (observed minus predicted)
- A **residual plot** graphs residuals against $x$; random scatter supports using a linear model, while curved or systematic patterns signal that a line is a poor fit
- Points with extreme x-values (high leverage) can exert strong influence on the slope and position of the regression line

### 5.5 Least-Squares Regression
- The LSRL is the unique line that makes the sum of squared residuals as small as possible
- Slope: $b = r \cdot \frac{s_y}{s_x}$; because the line must pass through $(\bar{x}, \bar{y})$, the intercept is $a = \bar{y} - b\bar{x}$
- The **coefficient of determination** $r^2$ tells us what fraction of the variability in $y$ is accounted for by the linear relationship with $x$
- Computer regression output typically reports the slope, intercept, $r^2$, and the residual standard deviation $s$

## Key Formulas

| Formula | Description |
|---------|-------------|
| $\hat{y} = a + bx$ | Least-squares regression line |
| $b = r \frac{s_y}{s_x}$ | Slope |
| $a = \bar{y} - b\bar{x}$ | Intercept (line passes through means) |
| residual $= y - \hat{y}$ | Residual |
| $r^2$ | Proportion of variation in $y$ explained by $x$ |

## Common Misconceptions

- $r = 0$ means no **linear** relationship, not necessarily no relationship at all -- a strong curved pattern can yield $r \approx 0$
- The slope interpretation is tied to a specific direction: a one-unit change in the explanatory variable predicts a change of $b$ in the response, not the other way around
- A large $r^2$ is not evidence of causation, nor does it guarantee the model is appropriate
- A clean residual plot (random scatter) supports a linear fit; a pattern in the residuals is a warning sign, not confirmation that the model is fine
- Applying the regression equation to x-values far outside the observed data range is extrapolation and leads to unreliable predictions
