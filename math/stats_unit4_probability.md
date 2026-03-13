# Unit 4: Probability, Random Variables, and Probability Distributions
> Exam Weight: 10–20% | ~18–20 Class Periods

## Topics

### 4.1 Introducing Statistics: Random and Non-Random Patterns?
- **Learning Objective (UNC-2.A):** Distinguish between random and non-random patterns
- **Essential Knowledge:**
  - Random processes generate outcomes that vary but follow a predictable distribution over the long run
  - Apparent patterns in small samples may be due to chance variation
  - Statistics helps distinguish genuine effects from random noise

### 4.2 Estimating Probabilities Using Simulation
- **Learning Objective (VAR-4.A):** Estimate probabilities using simulation
- **Essential Knowledge:**
  - A **simulation** models a random process using random number generators, coins, dice, etc.
  - Steps: (1) describe how to model one trial, (2) define what counts as a "success," (3) run many trials, (4) estimate probability as proportion of successes
  - The **Law of Large Numbers:** as the number of trials increases, the relative frequency of an outcome approaches its true probability

### 4.3 Introduction to Probability
- **Learning Objective (UNC-2.B):** Calculate basic probabilities
- **Essential Knowledge:**
  - **Sample space ($S$):** the set of all possible outcomes
  - **Event:** any subset of the sample space
  - For any event $A$: $0 \leq P(A) \leq 1$
  - $P(S) = 1$ and $P(\emptyset) = 0$
  - **Complement rule:** $P(A^c) = 1 - P(A)$

### 4.4 Mutually Exclusive Events
- **Learning Objective (UNC-2.C):** Calculate probabilities for mutually exclusive events
- **Essential Knowledge:**
  - **Mutually exclusive (disjoint)** events cannot occur at the same time: $P(A \cap B) = 0$
  - **Addition rule for mutually exclusive events:** $P(A \cup B) = P(A) + P(B)$
  - **General addition rule:** $P(A \cup B) = P(A) + P(B) - P(A \cap B)$

### 4.5 Conditional Probability
- **Learning Objective (UNC-2.D):** Calculate conditional probabilities
- **Essential Knowledge:**
  - **Conditional probability:** $P(A|B) = \frac{P(A \cap B)}{P(B)}$
  - Read as: "the probability of $A$ given $B$"
  - Conditional probability can be computed from two-way tables by restricting to the given condition
  - **General multiplication rule:** $P(A \cap B) = P(A) \cdot P(B|A)$

### 4.6 Independent Events and Unions of Events
- **Learning Objective (UNC-2.E):** Determine independence and calculate probabilities using independence
- **Essential Knowledge:**
  - Events $A$ and $B$ are **independent** if knowing one occurred does not change the probability of the other: $P(A|B) = P(A)$
  - Equivalently: $P(A \cap B) = P(A) \cdot P(B)$
  - **Mutually exclusive events are NOT independent** (unless one has probability 0)
  - For independent events, the multiplication rule simplifies: $P(A \cap B) = P(A) \cdot P(B)$

### 4.7 Introduction to Random Variables and Probability Distributions
- **Learning Objective (VAR-5.A):** Describe random variables and their probability distributions
- **Essential Knowledge:**
  - A **random variable** assigns numerical values to outcomes of a random process
  - **Discrete random variable:** takes on a countable number of values with specific probabilities
  - **Continuous random variable:** takes on any value in an interval; described by a density curve
  - **Probability distribution:** lists all possible values and their probabilities
  - For discrete: $\sum P(X = x_i) = 1$
  - For continuous: the total area under the density curve equals 1

### 4.8 Mean and Standard Deviation of Random Variables
- **Learning Objective (VAR-5.B):** Calculate the mean (expected value) and standard deviation of a discrete random variable
- **Essential Knowledge:**
  - **Mean (expected value):** $\mu_X = E(X) = \sum x_i \cdot P(x_i)$
  - **Variance:** $\sigma_X^2 = \sum (x_i - \mu_X)^2 \cdot P(x_i)$
  - **Standard deviation:** $\sigma_X = \sqrt{\sigma_X^2}$
  - The expected value is the long-run average; it does not have to be a possible outcome
  - Interpretation: "If this random process were repeated many times, the average outcome would be approximately $\mu_X$"

### 4.9 Combining Random Variables
- **Learning Objective (VAR-5.C):** Calculate the mean and standard deviation of linear combinations of random variables
- **Essential Knowledge:**
  - **Linear transformation:** If $Y = a + bX$:
    - $\mu_Y = a + b\mu_X$
    - $\sigma_Y = |b| \sigma_X$
  - **Sum of two random variables:** $\mu_{X+Y} = \mu_X + \mu_Y$
  - **Difference of two random variables:** $\mu_{X-Y} = \mu_X - \mu_Y$
  - If $X$ and $Y$ are **independent**:
    - $\sigma_{X+Y}^2 = \sigma_X^2 + \sigma_Y^2$
    - $\sigma_{X-Y}^2 = \sigma_X^2 + \sigma_Y^2$ (variances always ADD)
  - **Important:** Standard deviations do NOT add — variances do

### 4.10 Introduction to the Binomial Distribution
- **Learning Objective (VAR-5.D):** Determine whether a setting meets binomial conditions
- **Essential Knowledge:**
  - **BINS conditions:** Binary outcomes (success/failure), Independent trials, fixed Number of trials ($n$), Same probability of success ($p$) on each trial
  - $X \sim B(n, p)$ — "$X$ has a binomial distribution with parameters $n$ and $p$"
  - **Binomial probability:** $P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$
  - where $\binom{n}{k} = \frac{n!}{k!(n-k)!}$

### 4.11 Parameters for a Binomial Distribution
- **Learning Objective (VAR-5.E):** Calculate the mean and standard deviation of a binomial random variable
- **Essential Knowledge:**
  - **Mean:** $\mu_X = np$
  - **Standard deviation:** $\sigma_X = \sqrt{np(1-p)}$
  - When $n$ is large, the binomial distribution can be approximated by a normal distribution: $N(np, \sqrt{np(1-p)})$
  - Normal approximation is appropriate when $np \geq 10$ and $n(1-p) \geq 10$

### 4.12 The Geometric Distribution
- **Learning Objective (VAR-5.F):** Calculate probabilities for geometric random variables
- **Essential Knowledge:**
  - A **geometric random variable** counts the number of trials until the first success
  - Conditions: Binary outcome, Independent trials, Same probability $p$, trials continue until first success
  - $P(X = k) = (1-p)^{k-1} \cdot p$ for $k = 1, 2, 3, \ldots$
  - **Mean:** $\mu_X = \frac{1}{p}$
  - **Standard deviation:** $\sigma_X = \frac{\sqrt{1-p}}{p}$
  - $P(X > k) = (1-p)^k$ — probability of no success in first $k$ trials

## Common Misconceptions
- Confusing mutually exclusive with independent — they are fundamentally different concepts
- Adding standard deviations instead of variances when combining random variables
- Applying binomial formulas when trials are not independent (e.g., sampling without replacement from a small population)
- Thinking the expected value must be a possible outcome — it is a long-run average
- Forgetting to check conditions (BINS) before using the binomial distribution
- Confusing $P(A \cup B)$ (union/or) with $P(A \cap B)$ (intersection/and)
