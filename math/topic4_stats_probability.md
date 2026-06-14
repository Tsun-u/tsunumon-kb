# Topic 4: Statistics and Probability

> SL: 27 hours | HL: 33 hours

## SL Content

### 4.1 Descriptive Statistics
- Data comes in different flavours: discrete (counted), continuous (measured), qualitative (categorical), quantitative (numerical)
- Measures of central tendency summarise where a dataset is centered: mean ($\bar{x}$), median (middle value), mode (most frequent value)
- Measures of dispersion describe how spread out the data is: range, interquartile range (IQR), standard deviation ($\sigma$), variance ($\sigma^2$)
- When data is grouped into class intervals, you work with the modal class, an estimated mean, and an estimated standard deviation
- Visual displays suited to different data types: histograms (continuous data), box plots (five-number summary), and cumulative frequency curves (running totals)

### 4.2 Probability Fundamentals
- A sample space lists every possible outcome; an event is any subset of outcomes you are interested in
- $P(A) = \frac{n(A)}{n(S)}$ when all outcomes in the sample space are equally likely
- $P(A') = 1 - P(A)$: the complement rule says the probability of an event not happening is one minus the probability it does
- $P(A \cup B) = P(A) + P(B) - P(A \cap B)$: the addition rule avoids double-counting outcomes in both events
- **Mutually exclusive** events share no outcomes: $P(A \cap B) = 0$
- **Independent events** do not influence each other: $P(A \cap B) = P(A) \cdot P(B)$
- **Conditional probability** updates a probability given known information: $P(A|B) = \frac{P(A \cap B)}{P(B)}$

### 4.3 Probability Diagrams
- Tree diagrams trace sequential outcomes branch by branch, multiplying along each path
- Venn diagrams show overlaps between event sets, making inclusion-exclusion intuitive
- Two-way tables cross-tabulate two categorical variables, making conditional probabilities easy to read off
- Sample space diagrams display all outcomes of a two-stage experiment in a grid

### 4.4 Discrete Random Variables
- Expected value is the long-run average outcome: $E(X) = \sum x_i P(X = x_i)$
- Variance measures how spread out the distribution is around its mean: $\text{Var}(X) = E(X^2) - [E(X)]^2$

### 4.5 Binomial Distribution
- Applies when you repeat the same trial a fixed number of times, each trial has only two possible outcomes, and the probability of success is the same every time
- $X \sim B(n, p)$
- $P(X = r) = \binom{n}{r} p^r (1-p)^{n-r}$
- Mean and variance: $E(X) = np$, $\text{Var}(X) = np(1-p)$

### 4.6 Normal Distribution
- $X \sim N(\mu, \sigma^2)$: a symmetric, bell-shaped distribution fully described by its mean $\mu$ and variance $\sigma^2$
- **Standard normal**: $Z \sim N(0, 1)$; any normal variable standardises via $z = \frac{x - \mu}{\sigma}$
- Empirical rule: approximately 68%, 95%, and 99.7% of data falls within one, two, and three standard deviations of the mean respectively
- A GDC computes normal probabilities and inverse normal values directly, making the $z$-table largely obsolete

### 4.7 Regression and Correlation
- A scatter diagram gives an immediate visual sense of whether two variables are linearly related and in which direction
- **Pearson's correlation coefficient** ($r$) quantifies linear association: $-1 \leq r \leq 1$, with values near $\pm 1$ indicating strong linear trends
- The least-squares regression line minimises the total squared vertical distances: $\hat{y} = ax + b$
- Interpolation (predicting inside the data range) is more reliable than extrapolation (predicting beyond it)

## HL Extension

### 4.8 Bayes' Theorem
- $P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$
- Provides a systematic method to reverse conditional probabilities — useful when you know $P(B|A)$ but need $P(A|B)$
- Tree diagrams are a natural scaffold: compute prior probabilities on the first set of branches, then update to posteriors on the second
- Classic applications: diagnostic accuracy of medical tests, reliability engineering

### 4.9 Poisson Distribution (HL)
- Suitable for counting how many times a rare event occurs in a fixed time or space, where events happen independently at a constant average rate
- $X \sim Po(\lambda)$
- $P(X = r) = \frac{e^{-\lambda}\lambda^r}{r!}$
- Mean and variance are both equal to $\lambda$: $E(X) = \lambda$, $\text{Var}(X) = \lambda$

### 4.10 Hypothesis Testing (HL)
- Null hypothesis ($H_0$) is the default assumption; alternative hypothesis ($H_1$) is what you are trying to find evidence for
- Significance level ($\alpha$) sets the threshold for "surprising enough to reject $H_0$" — commonly 5% or 1%
- $p$-value: the probability of observing data at least as extreme as what you got, if $H_0$ were true; small $p$-values cast doubt on $H_0$
- One-tailed tests look for an effect in one direction; two-tailed tests are sensitive to effects in either direction
- Chi-squared goodness of fit test checks whether observed frequencies match a theoretical distribution: $\chi^2 = \sum \frac{(O - E)^2}{E}$
- Chi-squared test for independence examines whether two categorical variables in a contingency table are related
- $t$-test compares sample means when population standard deviation is unknown

## Key Equations

| Equation | Description |
|----------|-------------|
| $P(A \cup B) = P(A) + P(B) - P(A \cap B)$ | Addition rule |
| $P(A\|B) = P(A \cap B)/P(B)$ | Conditional probability |
| $P(X=r) = \binom{n}{r}p^r(1-p)^{n-r}$ | Binomial probability |
| $z = (x-\mu)/\sigma$ | Standardization |
| $P(A\|B) = P(B\|A)P(A)/P(B)$ | Bayes' theorem (HL) |
| $\chi^2 = \sum(O-E)^2/E$ | Chi-squared statistic (HL) |

## Common Misconceptions

1. **"Correlation implies causation"** -- A strong $r$ value tells you two variables move together; it says nothing about whether one causes the other; a lurking third variable may be responsible.
2. **"The mean is always the best measure of center"** -- When data is heavily skewed or contains extreme outliers, the median gives a more honest picture of a typical value.
3. **"A p-value > 0.05 means $H_0$ is true"** -- Failing to reject $H_0$ simply means the data does not provide sufficient evidence against it; the null hypothesis may still be false.
4. **"Normal distribution applies to all data"** -- Many real datasets are skewed, multimodal, or bounded; assuming normality without checking can lead to badly wrong conclusions.
5. **"Independent and mutually exclusive are the same"** -- These are distinct concepts; two events with non-zero probability that are mutually exclusive are actually dependent (knowing one occurred tells you the other cannot have).

## Comparison with AP Mathematics

- AP Statistics dedicates an entire course to the material in this topic, so its treatment of inference and experimental design is considerably deeper than IB AA's
- IB AA treats statistics as one of five equal topics; students who want breadth across all of mathematics will find this balance suits that goal
- Poisson distribution and chi-squared tests appear in IB HL; AP Statistics also covers chi-squared procedures with similar emphasis
- Both curricula stress interpreting statistical results in real-world context rather than just calculating answers
