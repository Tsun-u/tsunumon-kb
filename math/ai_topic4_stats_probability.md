# IB Math AI — Topic 4: Statistics and Probability

> SL: 36 hours | HL: 52 hours
> The statistical heart of IB Math AI — the largest topic at both levels.

## SL Content

### SL 4.1 Sampling Concepts
- Population, sample, random sample; distinguishing discrete from continuous data
- Evaluating source reliability; recognizing sampling bias; handling outliers in context
- **Sampling methods**: simple random, convenience, systematic, quota, stratified

### SL 4.2 Data Presentation
- Frequency distributions and histograms
- **Cumulative frequency graphs**: extracting the median, quartiles, percentiles, range, and IQR
- **Box-and-whisker diagrams**; flagging outliers using the $Q_1 - 1.5 \times IQR$ and $Q_3 + 1.5 \times IQR$ fences

### SL 4.3 Descriptive Statistics
- Measures of centre: mean, median, mode; estimating from grouped frequency data
- Measures of spread: standard deviation, variance, IQR
- Effect of adding a constant or multiplying by a constant on each measure

### SL 4.4 Linear Correlation and Regression
- Scatter diagrams; **Pearson's product-moment correlation coefficient** $r$
- Line of best fit drawn by eye through the mean point $(\bar{x}, \bar{y})$
- **Least-squares regression line of $y$ on $x$** (computed with technology); difference between interpolation and extrapolation

### SL 4.5 Probability Concepts
- Trial, outcome, equally likely outcomes, relative frequency, sample space, event
- $P(A) = \frac{n(A)}{n(U)}$; complementary events $P(A') = 1 - P(A)$
- Expected frequency of an event over many repeated trials

### SL 4.6 Combined Events
- Venn diagrams, tree diagrams, sample space diagrams, two-way tables
- Union: $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
- Mutually exclusive events; **conditional probability** $P(A|B)$; independence criterion $P(A \cap B) = P(A)P(B)$

### SL 4.7 Discrete Random Variables
- Probability distribution of a discrete random variable
- **Expected value** $E(X) = \sum x P(X = x)$; applications to fair games and long-run averages

### SL 4.8 Binomial Distribution
- $X \sim B(n, p)$; conditions under which this model applies
- Mean $np$, variance $np(1-p)$; probabilities computed with technology

### SL 4.9 Normal Distribution
- The bell-shaped, symmetric normal curve described by mean $\mu$ and standard deviation $\sigma$
- Computing normal probabilities and **inverse normal** values using technology
- Standardization via z-scores

### SL 4.10 Spearman's Rank Correlation
- **Spearman's rank correlation coefficient** $r_s$ — measures monotonic association by ranking the data
- More suitable than Pearson's $r$ when the relationship is monotonic but not linear, or when outliers are present
- Understanding how outliers affect $r$ and $r_s$ differently

### SL 4.11 Hypothesis Testing (SL Toolkit)
- Null and alternative hypotheses $H_0$, $H_1$; significance levels; **p-values**
- **Chi-square test for independence**: contingency tables, degrees of freedom, expected frequencies
- **Chi-square goodness of fit test**
- **t-test** (one-sample and two-sample, with technology); one-tailed and two-tailed tests

## HL Extension

### AHL 4.12 Data Collection and Validity
- Designing sound data collection instruments (surveys, questionnaires)
- Selecting relevant variables; organizing data by type; checking for reliability and validity

### AHL 4.13 Non-Linear Regression
- Fitting quadratic, cubic, exponential, power, and sinusoidal models to data using technology
- **Sum of squared residuals ($SS_{res}$)** as a measure of how well a model fits
- **Coefficient of determination $R^2$**: interpretation and its limitations

### AHL 4.14 Transformations of Random Variables
- Linear transformation rules: $E(aX + b) = aE(X) + b$, $\text{Var}(aX + b) = a^2\text{Var}(X)$
- Expected value and variance of linear combinations of independent random variables
- **Unbiased estimators**: sample mean $\bar{x}$ for $\mu$; sample variance $s_{n-1}^2$ for $\sigma^2$

### AHL 4.15 Linear Combinations of Normal Variables and CLT
- A linear combination of independent normal random variables is also normally distributed
- **Central Limit Theorem**: for large samples ($n \geq 30$), the distribution of $\bar{X}$ is approximately normal regardless of the population shape

### AHL 4.16 Confidence Intervals
- Constructing confidence intervals for a population mean
- z-intervals (when $\sigma$ is known) and t-intervals (when $\sigma$ is unknown), both using technology

### AHL 4.17 Poisson Distribution
- $X \sim \text{Po}(m)$; mean equals variance: $E(X) = \text{Var}(X) = m$
- The sum of two independent Poisson variables is also Poisson
- Conditions: events occur independently at a fixed average rate over time or space

### AHL 4.18 Hypothesis Testing (Formal)
- **Critical values and critical regions**
- Tests for: population mean (normal and t-distribution), proportion (binomial), Poisson mean, correlation ($H_0: \rho = 0$)
- Paired and two-sample procedures
- **Type I error** (incorrectly rejecting a true $H_0$) and **Type II error** (failing to reject a false $H_0$); probabilities of each

### AHL 4.19 Markov Chains
- **Transition matrices**: encoding state-to-state probabilities
- Powers of transition matrices to find probabilities after $n$ steps
- **Steady-state (long-run) distribution**: found via eigenvectors or by solving $T\mathbf{s} = \mathbf{s}$

## Key Equations

| Equation | Description |
|----------|-------------|
| $E(X) = \sum x P(X=x)$ | Expected value |
| $P(A\|B) = \frac{P(A \cap B)}{P(B)}$ | Conditional probability |
| $X \sim B(n,p)$: $E(X) = np$, $\text{Var}(X) = np(1-p)$ | Binomial distribution |
| $z = \frac{x - \mu}{\sigma}$ | Standardization |
| $\chi^2 = \sum \frac{(f_o - f_e)^2}{f_e}$ | Chi-square statistic |
| $X \sim \text{Po}(m)$: $E(X) = \text{Var}(X) = m$ | Poisson distribution (HL) |
| $\text{Var}(aX+b) = a^2 \text{Var}(X)$ | Linear transformation (HL) |

## Core Vocabulary (for subject/topic classification)

distribution, normal distribution, binomial distribution, Poisson distribution, percentile, quartile, interquartile range, standard deviation, variance, mean, median, mode, correlation, regression, residual, scatter diagram, sampling, stratified sampling, bias, outlier, expected value, random variable, hypothesis test, null hypothesis, p-value, significance level, chi-square, t-test, confidence interval, z-score, central limit theorem, Markov chain, transition matrix, Spearman's rank, Pearson correlation

## Common Misconceptions

1. **Correlation and causation** — A high value of $r$ shows statistical association, not a cause-and-effect link.
2. **Spearman's vs. Pearson's** — Spearman's measures monotonic association of ranks; a perfectly monotone curve can give $r_s = 1$ while $r < 1$.
3. **Non-rejection of $H_0$** — Failing to reject $H_0$ is not proof of its truth; it means there is insufficient evidence to conclude otherwise.
4. **Binomial vs. Poisson** — Binomial counts successes across a fixed number of trials; Poisson counts events in a fixed interval at a constant average rate.
5. **Chi-square and small expected counts** — The chi-square approximation is unreliable when expected frequencies fall below 5; combine categories if needed.
6. **Extrapolation beyond observed data** — A regression model is only validated within the observed data range; predictions outside that range are speculative.

## Comparison with Other Courses

- AI SL statistics broadly parallels AP Statistics in topic coverage but at shallower depth; AI HL surpasses AP Statistics in several areas (Poisson, Markov chains, formal estimators, eigenvalue-based steady states)
- The 2026-27 AP Statistics revision removed the chi-square goodness of fit test; IB AI SL retains it
- Spearman's rank correlation is assessed in AI but absent from AP Statistics
- AA covers far less statistics than AI; Bayes' theorem appears only in AA HL (not in AI at either level)
