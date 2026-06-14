# Unit 4: Probability, Random Variables, and Probability Distributions
> Exam Weight: 10–20% | ~18–20 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content now in **new Unit 2**. Removed from the course: combining random variables (4.9) and the geometric distribution (4.12). See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 4.1 Randomness and Patterns
Random processes generate variable outcomes, but over the long run those outcomes follow predictable patterns.
- Apparent structure in a small sample is often just chance variation, not a genuine signal
- Statistical reasoning helps distinguish real patterns from random noise

### 4.2 Estimating Probabilities Through Simulation
When theoretical probabilities are hard to compute, simulation provides an estimate.
- A **simulation** models a random process using random number generators, coins, dice, or similar tools
- Steps: (1) define how to model one trial, (2) specify what counts as the event of interest, (3) run many trials, (4) estimate probability as the proportion of favorable outcomes
- **Law of Large Numbers:** as the number of trials grows, the observed relative frequency of an outcome converges toward its true probability

### 4.3 Probability Basics
Probability assigns numbers between 0 and 1 to events, measuring how likely they are.
- **Sample space ($S$):** the set of all possible outcomes of a random process
- **Event:** any subset of the sample space
- For any event $A$: $0 \leq P(A) \leq 1$; $P(S) = 1$; $P(\emptyset) = 0$
- **Complement rule:** $P(A^c) = 1 - P(A)$

### 4.4 Mutually Exclusive Events
Two events are mutually exclusive (disjoint) when they cannot both occur.
- **Mutually exclusive events:** $P(A \cap B) = 0$
- **Addition rule for disjoint events:** $P(A \cup B) = P(A) + P(B)$
- **General addition rule (any events):** $P(A \cup B) = P(A) + P(B) - P(A \cap B)$

### 4.5 Conditional Probability
Conditional probability updates the likelihood of an event given that another has occurred.
- **Conditional probability:** $P(A|B) = \frac{P(A \cap B)}{P(B)}$, read as "the probability of $A$ given $B$"
- Conditional probabilities can be read directly from two-way tables by restricting to the given condition
- **General multiplication rule:** $P(A \cap B) = P(A) \cdot P(B|A)$

### 4.6 Independent Events
Two events are independent when knowledge of one does not change the probability of the other.
- Events $A$ and $B$ are **independent** if $P(A|B) = P(A)$, equivalently $P(A \cap B) = P(A) \cdot P(B)$
- Mutually exclusive events are **not** independent (unless one has probability zero) — knowing one occurred guarantees the other did not
- For independent events, the multiplication rule simplifies: $P(A \cap B) = P(A) \cdot P(B)$

### 4.7 Random Variables and Probability Distributions
A random variable assigns a number to each outcome of a random process.
- **Discrete random variable:** takes a countable number of values, each with an assigned probability
- **Continuous random variable:** takes values in an interval; probabilities correspond to areas under a density curve
- **Probability distribution:** a complete listing of possible values and their probabilities
- For discrete: $\sum P(X = x_i) = 1$; for continuous: total area under the density curve equals 1

### 4.8 Mean and Standard Deviation of a Discrete Random Variable
Probability distributions have their own measures of center and spread.
- **Expected value (mean):** $\mu_X = E(X) = \sum x_i \cdot P(x_i)$ — the long-run average over many repetitions
- **Variance:** $\sigma_X^2 = \sum (x_i - \mu_X)^2 \cdot P(x_i)$
- **Standard deviation:** $\sigma_X = \sqrt{\sigma_X^2}$
- The expected value is a long-run average; it does not have to equal any particular possible outcome

### 4.9 Combining Random Variables
Linear transformations and combinations of random variables follow predictable rules.
- **Linear transformation** (if $Y = a + bX$): $\mu_Y = a + b\mu_X$ and $\sigma_Y = |b| \sigma_X$
- **Sum:** $\mu_{X+Y} = \mu_X + \mu_Y$; **Difference:** $\mu_{X-Y} = \mu_X - \mu_Y$
- If $X$ and $Y$ are **independent**: $\sigma_{X+Y}^2 = \sigma_X^2 + \sigma_Y^2$ and $\sigma_{X-Y}^2 = \sigma_X^2 + \sigma_Y^2$ (variances always add)
- Standard deviations do **not** add — variances do

### 4.10 The Binomial Setting
A binomial random variable counts successes in a fixed number of independent trials.
- **Conditions (BINS):** Binary outcomes (success/failure), Independent trials, fixed Number of trials $n$, Same probability $p$ per trial
- $X \sim B(n, p)$
- **Binomial probability:** $P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$, where $\binom{n}{k} = \frac{n!}{k!(n-k)!}$

### 4.11 Mean and Standard Deviation of a Binomial Variable
- **Mean:** $\mu_X = np$
- **Standard deviation:** $\sigma_X = \sqrt{np(1-p)}$
- When $n$ is large, the binomial can be approximated by a normal distribution: $N(np, \sqrt{np(1-p)})$
- Normal approximation is reasonable when both $np \geq 10$ and $n(1-p) \geq 10$

### 4.12 The Geometric Distribution
A geometric random variable counts trials until the first success.
- Conditions: binary outcomes, independent trials, same probability $p$ per trial, no fixed endpoint
- $P(X = k) = (1-p)^{k-1} \cdot p$ for $k = 1, 2, 3, \ldots$
- **Mean:** $\mu_X = \frac{1}{p}$; **Standard deviation:** $\sigma_X = \frac{\sqrt{1-p}}{p}$
- $P(X > k) = (1-p)^k$ — probability of not succeeding in the first $k$ trials

## Common Misconceptions
- Mutually exclusive and independent are not synonyms — disjoint events cannot both occur; independent events have no influence on each other
- Standard deviations do not add when combining random variables — variances do, then take the square root
- The binomial formula requires independence; sampling without replacement from a small population violates this
- The expected value is a long-run average, not necessarily a value the variable can actually take
- Forgetting to verify BINS conditions before applying the binomial — checking independence matters
- Confusing $P(A \cup B)$ (union — at least one occurs) with $P(A \cap B)$ (intersection — both occur)
