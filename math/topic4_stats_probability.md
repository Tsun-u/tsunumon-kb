# Topic 4: Statistics and Probability

> SL: 27 hours | HL: 33 hours

## SL Content

### 4.1 Descriptive Statistics
- Types of data: discrete, continuous, qualitative, quantitative
- Measures of central tendency: mean ($\bar{x}$), median, mode
- Measures of dispersion: range, interquartile range (IQR), standard deviation ($\sigma$), variance ($\sigma^2$)
- Grouped data: modal class, estimated mean, standard deviation
- Graphical representations: histograms, box plots, cumulative frequency curves

### 4.2 Probability Fundamentals
- Sample space, events, complementary events
- $P(A) = \frac{n(A)}{n(S)}$ (equally likely outcomes)
- $P(A') = 1 - P(A)$
- $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
- **Mutually exclusive**: $P(A \cap B) = 0$
- **Independent events**: $P(A \cap B) = P(A) \cdot P(B)$
- **Conditional probability**: $P(A|B) = \frac{P(A \cap B)}{P(B)}$

### 4.3 Probability Diagrams
- Tree diagrams
- Venn diagrams
- Two-way tables
- Sample space diagrams

### 4.4 Discrete Random Variables
- Expected value: $E(X) = \sum x_i P(X = x_i)$
- Variance: $\text{Var}(X) = E(X^2) - [E(X)]^2$

### 4.5 Binomial Distribution
- Conditions: fixed $n$ trials, two outcomes, constant probability $p$, independent trials
- $X \sim B(n, p)$
- $P(X = r) = \binom{n}{r} p^r (1-p)^{n-r}$
- $E(X) = np$, $\text{Var}(X) = np(1-p)$

### 4.6 Normal Distribution
- $X \sim N(\mu, \sigma^2)$: bell-shaped, symmetric about $\mu$
- **Standard normal**: $Z \sim N(0, 1)$; $z = \frac{x - \mu}{\sigma}$
- 68-95-99.7 rule
- Using GDC for normal probabilities and inverse normal calculations

### 4.7 Regression and Correlation
- Scatter diagrams and types of correlation (positive, negative, none)
- **Pearson's correlation coefficient** ($r$): $-1 \leq r \leq 1$
- Least-squares regression line: $\hat{y} = ax + b$
- Interpolation vs. extrapolation

## HL Extension

### 4.8 Bayes' Theorem
- $P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$
- Using tree diagrams for prior and posterior probabilities
- Applications in medical testing, reliability

### 4.9 Poisson Distribution (HL)
- Conditions: events occur independently, at a constant average rate
- $X \sim Po(\lambda)$
- $P(X = r) = \frac{e^{-\lambda}\lambda^r}{r!}$
- $E(X) = \lambda$, $\text{Var}(X) = \lambda$

### 4.10 Hypothesis Testing (HL)
- Null hypothesis ($H_0$) and alternative hypothesis ($H_1$)
- Significance level ($\alpha$): typically 5% or 1%
- $p$-value: probability of obtaining results at least as extreme as observed, given $H_0$ is true
- One-tailed and two-tailed tests
- Chi-squared goodness of fit test: $\chi^2 = \sum \frac{(O - E)^2}{E}$
- Chi-squared test for independence (contingency tables)
- $t$-test for means

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

1. **"Correlation implies causation"** -- Correlation shows association, not cause and effect.
2. **"The mean is always the best measure of center"** -- Median is better for skewed data or data with outliers.
3. **"A p-value > 0.05 means $H_0$ is true"** -- It means we fail to reject $H_0$; it does not prove $H_0$.
4. **"Normal distribution applies to all data"** -- Many real-world distributions are not normal (skewed, bimodal, etc.).
5. **"Independent and mutually exclusive are the same"** -- They are different concepts; mutually exclusive events (with non-zero probability) are actually dependent.

## Comparison with AP Mathematics

- AP Statistics covers descriptive statistics, probability, and inference with greater depth overall
- IB AA SL covers statistics as one of five topics; AP Statistics is an entire course
- IB HL includes Poisson distribution and chi-squared tests; AP Statistics covers chi-squared similarly
- Both curricula emphasize interpretation of results in context
