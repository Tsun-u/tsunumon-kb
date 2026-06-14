# AP Statistics (2026-27 CED) -- Unit 2: Probability, Random Variables, and Probability Distributions

> Exam Weight: 15–25% | ~24 Class Periods
> This unit brings together the analysis of two categorical variables, the rules of probability, random variables, the binomial and normal distributions, and the Central Limit Theorem.

## Topics

### 2.1 Tabular and Graphical Representations for the Distributions of Two Categorical Variables
- Two-way (contingency) tables organize counts; we distinguish joint, **marginal**, and **conditional relative frequencies** among entries
- Visual displays include side-by-side bar charts and segmented (stacked) bar charts
- Patterns in conditional distributions serve as evidence when exploring whether two categorical variables are associated

### 2.2 Summary Statistics for Two Categorical Variables
- Conditional proportions are computed for each group and placed side by side for comparison
- A meaningful difference between conditional distributions across groups points toward an association between the variables

### 2.3 Estimating Probabilities Using Simulation
- To simulate a random process: identify what constitutes one trial, decide what counts as success, repeat many trials, and record the proportion of successes as the probability estimate
- **Law of Large Numbers**: as the number of trials grows, the observed relative frequency gets closer to the true probability

### 2.4 Introduction to Probability
- A sample space lists every possible outcome; an event is a subset of those outcomes; $0 \leq P(A) \leq 1$ for any event
- **Complement rule**: $P(A^c) = 1 - P(A)$

### 2.5 Mutually Exclusive Events
- Two events are disjoint if they cannot happen at the same time: $P(A \cap B) = 0$
- When events are mutually exclusive, their union simplifies to $P(A \cup B) = P(A) + P(B)$
- **General addition rule** applies regardless: $P(A \cup B) = P(A) + P(B) - P(A \cap B)$

### 2.6 Conditional Probability
- $P(A|B) = \frac{P(A \cap B)}{P(B)}$ expresses how the probability of $A$ shifts once we know $B$ occurred
- **General multiplication rule**: $P(A \cap B) = P(A) \cdot P(B|A)$
- Two-way tables and tree diagrams are common tools for working out conditional probabilities

### 2.7 Independent Events and Unions of Events
- Events $A$ and $B$ are independent when $P(A|B) = P(A)$, which is equivalent to $P(A \cap B) = P(A)P(B)$
- Mutually exclusive events with positive probability are **never** independent -- knowing one occurred rules out the other

### 2.8 Introduction to Random Variables and Probability Distributions
- A random variable assigns a number to each outcome of a random process
- Discrete random variables take on a countable set of values; continuous random variables cover an interval
- A valid discrete distribution requires $\sum P(X = x_i) = 1$; for continuous distributions, total area under the density curve must equal 1

### 2.9 Parameters of Random Variables
- Mean (expected value): $\mu_X = E(X) = \sum x_i P(x_i)$ — the long-run average value of the variable
- Variance: $\sigma_X^2 = \sum (x_i - \mu_X)^2 P(x_i)$; taking the square root gives the standard deviation $\sigma_X$

### 2.10 The Binomial Distribution
- **BINS conditions** must all hold: Binary outcomes, Independent trials, fixed Number of trials, Same probability of success on each trial
- $P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$
- Mean $\mu_X = np$; standard deviation $\sigma_X = \sqrt{np(1-p)}$

### 2.11 The Normal Distribution
- The normal curve is symmetric and bell-shaped; the **empirical rule** states roughly 68%, 95%, and 99.7% of values fall within 1, 2, and 3 standard deviations of the mean
- Any value can be converted to a standardized score: $z = \frac{x - \mu}{\sigma}$; technology or tables then give the corresponding probability
- Inverse normal calculations locate the value at a given **percentile**
- Graphical tools and outlier checks help assess whether a dataset is approximately normal

### 2.12 Sampling Distributions and the Central Limit Theorem
- The **sampling distribution** of a statistic describes how that statistic varies across all possible samples of a given size
- **Central Limit Theorem**: when $n$ is large enough (often cited as $n \geq 30$), the sampling distribution of $\bar{x}$ is approximately normal no matter what shape the population has
- Larger sample sizes reduce sampling variability, pulling the distribution tighter around the true parameter

## Key Formulas

| Formula | Description |
|---------|-------------|
| $P(A \cup B) = P(A) + P(B) - P(A \cap B)$ | General addition rule |
| $P(A \cap B) = P(A) \cdot P(B\|A)$ | General multiplication rule |
| $P(X=k) = \binom{n}{k}p^k(1-p)^{n-k}$ | Binomial probability |
| $\mu_X = np$, $\sigma_X = \sqrt{np(1-p)}$ | Binomial parameters |
| $z = \frac{x-\mu}{\sigma}$ | Standardized score |

## Common Misconceptions

- Mutually exclusive and independent are entirely different ideas -- do not treat them as interchangeable
- The empirical rule (68–95–99.7) only holds for data that follow an approximately **normal** distribution
- The binomial model breaks down when trials are not independent, such as when sampling without replacement from a small population
- The Law of Large Numbers says nothing about short-run outcomes -- past results do not "balance out" future ones (this is the gambler's fallacy)
- The distribution of one sample's data is not the same thing as the **sampling distribution** of a statistic across many samples
