# Unit 10: Infinite Sequences and Series
> BC Only | BC Exam Weight: 17–18% | ~17–18 Class Periods

## Big Ideas: LIM, FUN

---

## Topics

### 10.1 Defining Convergent and Divergent Infinite Series
- **Learning Objective (LIM-7.A):** Determine convergence or divergence of a series.
- **Essential Knowledge:**
  - An **infinite series** $\sum_{n=1}^{\infty} a_n = a_1 + a_2 + a_3 + \cdots$
  - **Partial sums:** $S_n = \sum_{k=1}^{n} a_k$
  - The series **converges** if $\lim_{n \to \infty} S_n = S$ exists (finite). Otherwise it **diverges**.
  - A **sequence** $\{a_n\}$ converges if $\lim_{n \to \infty} a_n = L$ exists.

### 10.2 Working with Geometric Series
- **Learning Objective (LIM-7.A):** Analyze geometric series.
- **Essential Knowledge:**
  - **Geometric series:** $\sum_{n=0}^{\infty} ar^n = a + ar + ar^2 + \cdots$
  - **Converges** if $|r| < 1$, with sum $S = \frac{a}{1 - r}$
  - **Diverges** if $|r| \geq 1$
  - First term is $a$, common ratio is $r$.
  - Can be used to find sums of related series by manipulation (e.g., reindexing, multiplying by constants).

### 10.3 The $n$th Term Test for Divergence
- **Learning Objective (LIM-7.A):** Apply the $n$th Term Test.
- **Essential Knowledge:**
  - **$n$th Term Test (Divergence Test):** If $\lim_{n \to \infty} a_n \neq 0$, then $\sum a_n$ diverges.
  - **Contrapositive:** If $\sum a_n$ converges, then $\lim_{n \to \infty} a_n = 0$.
  - IMPORTANT: $\lim_{n \to \infty} a_n = 0$ does NOT guarantee convergence (e.g., harmonic series).
  - Common misconception: If $a_n \to 0$, the series converges. This is FALSE.

### 10.4 Integral Test for Convergence
- **Learning Objective (LIM-7.A):** Apply the Integral Test.
- **Essential Knowledge:**
  - **Integral Test:** If $f$ is continuous, positive, and decreasing for $x \geq N$, and $a_n = f(n)$, then:
    $$\sum_{n=N}^{\infty} a_n \text{ and } \int_N^{\infty} f(x)\,dx \text{ either both converge or both diverge.}$$
  - The integral test does NOT give the sum of the series.
  - Used to establish convergence/divergence, not to find the exact sum.

### 10.5 Harmonic Series and $p$-Series
- **Learning Objective (LIM-7.A):** Classify $p$-series.
- **Essential Knowledge:**
  - **$p$-series:** $\sum_{n=1}^{\infty} \frac{1}{n^p}$
    - Converges if $p > 1$
    - Diverges if $p \leq 1$
  - **Harmonic series** ($p = 1$): $\sum_{n=1}^{\infty} \frac{1}{n}$ diverges.
  - Examples:
    - $\sum \frac{1}{n^2}$ converges ($p = 2$)
    - $\sum \frac{1}{\sqrt{n}}$ diverges ($p = 1/2$)

### 10.6 Comparison Tests for Convergence
- **Learning Objective (LIM-7.A):** Apply comparison tests.
- **Essential Knowledge:**
  - **Direct Comparison Test:** For $0 \leq a_n \leq b_n$:
    - If $\sum b_n$ converges, then $\sum a_n$ converges.
    - If $\sum a_n$ diverges, then $\sum b_n$ diverges.
  - **Limit Comparison Test:** If $a_n > 0$, $b_n > 0$, and $\lim_{n \to \infty} \frac{a_n}{b_n} = L$ where $0 < L < \infty$, then $\sum a_n$ and $\sum b_n$ either both converge or both diverge.
  - Typically compare to a known $p$-series or geometric series.

### 10.7 Alternating Series Test for Convergence
- **Learning Objective (LIM-7.A):** Apply the Alternating Series Test.
- **Essential Knowledge:**
  - **Alternating Series Test (Leibniz Test):** $\sum_{n=1}^{\infty} (-1)^{n+1} b_n$ converges if:
    1. $b_n > 0$ for all $n$
    2. $b_{n+1} \leq b_n$ (terms are non-increasing in absolute value)
    3. $\lim_{n \to \infty} b_n = 0$
  - Classic example: $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n} = \ln 2$ (alternating harmonic series converges).

### 10.8 Ratio Test for Convergence
- **Learning Objective (LIM-7.A):** Apply the Ratio Test.
- **Essential Knowledge:**
  - **Ratio Test:** Let $L = \lim_{n \to \infty} \left|\frac{a_{n+1}}{a_n}\right|$:
    - If $L < 1$: series converges absolutely.
    - If $L > 1$ (or $L = \infty$): series diverges.
    - If $L = 1$: test is inconclusive.
  - Especially useful for series involving factorials, exponentials, and $n$th powers.

### 10.9 Determining Absolute or Conditional Convergence
- **Learning Objective (LIM-7.A):** Determine absolute or conditional convergence.
- **Essential Knowledge:**
  - **Absolute convergence:** $\sum |a_n|$ converges $\Rightarrow$ $\sum a_n$ converges absolutely.
  - **Conditional convergence:** $\sum a_n$ converges but $\sum |a_n|$ diverges.
  - Absolute convergence $\Rightarrow$ convergence, but not vice versa.
  - Example: $\sum \frac{(-1)^n}{n}$ converges conditionally (converges, but $\sum \frac{1}{n}$ diverges).

### 10.10 Alternating Series Error Bound
- **Learning Objective (LIM-7.B):** Bound the error of a partial sum for an alternating series.
- **Essential Knowledge:**
  - **Alternating Series Error Bound:** If $S = \sum_{n=1}^{\infty} (-1)^{n+1} b_n$ satisfies the alternating series test, and $S_N$ is the $N$th partial sum, then:
    $$|S - S_N| \leq b_{N+1}$$
  - The error is bounded by the absolute value of the first omitted term.
  - This allows determination of how many terms are needed for a desired accuracy.

### 10.11 Finding Taylor Polynomial Approximations of Functions
- **Learning Objective (LIM-8.A):** Construct Taylor polynomials.
- **Essential Knowledge:**
  - **Taylor polynomial of degree $n$ centered at $x = a$:**
    $$P_n(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!}(x - a)^k = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \cdots$$
  - **Maclaurin polynomial:** Taylor polynomial centered at $a = 0$.
  - Higher-degree polynomials generally provide better approximations near $x = a$.

### 10.12 Lagrange Error Bound
- **Learning Objective (LIM-8.B):** Apply the Lagrange error bound.
- **Essential Knowledge:**
  - **Lagrange Error Bound (Taylor's Remainder):** If $|f^{(n+1)}(c)| \leq M$ for all $c$ between $a$ and $x$, then:
    $$|R_n(x)| = |f(x) - P_n(x)| \leq \frac{M}{(n+1)!}|x - a|^{n+1}$$
  - Used to guarantee that the Taylor polynomial approximation is within a certain error.
  - Must find or bound the $(n+1)$th derivative on the relevant interval.

### 10.13 Radius and Interval of Convergence of Power Series
- **Learning Objective (LIM-8.C):** Determine radius and interval of convergence.
- **Essential Knowledge:**
  - A **power series** centered at $a$: $\sum_{n=0}^{\infty} c_n(x - a)^n$
  - **Radius of convergence $R$:** The series converges for $|x - a| < R$ and diverges for $|x - a| > R$.
  - **Interval of convergence:** $(a - R, a + R)$ plus possible endpoints. Test endpoints separately.
  - Use the Ratio Test to find $R$: $R = \lim_{n \to \infty} \left|\frac{c_n}{c_{n+1}}\right|$ (when the limit exists).
  - Special cases: $R = 0$ (converges only at $x = a$), $R = \infty$ (converges for all $x$).

### 10.14 Finding Taylor or Maclaurin Series for a Function
- **Learning Objective (LIM-8.D):** Find Taylor/Maclaurin series.
- **Essential Knowledge:**
  - **Taylor series** of $f$ centered at $a$: $\sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!}(x - a)^n$
  - **Key Maclaurin series to memorize:**
    - $e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots$ (for all $x$)
    - $\sin x = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!} = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots$ (for all $x$)
    - $\cos x = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{(2n)!} = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \cdots$ (for all $x$)
    - $\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n = 1 + x + x^2 + x^3 + \cdots$ (for $|x| < 1$)
    - $\ln(1+x) = \sum_{n=1}^{\infty} \frac{(-1)^{n+1} x^n}{n} = x - \frac{x^2}{2} + \frac{x^3}{3} - \cdots$ (for $-1 < x \leq 1$)

### 10.15 Representing Functions as Power Series
- **Learning Objective (LIM-8.E):** Manipulate known series to represent new functions.
- **Essential Knowledge:**
  - **Operations on power series** (within the interval of convergence):
    - **Substitution:** Replace $x$ with an expression (e.g., $e^{-x^2} = \sum \frac{(-x^2)^n}{n!}$).
    - **Multiplication:** Multiply a series by $x^k$ or a constant.
    - **Addition/Subtraction:** Combine series term by term.
    - **Differentiation:** $\frac{d}{dx}\left[\sum c_n x^n\right] = \sum n c_n x^{n-1}$ (same radius of convergence).
    - **Integration:** $\int \left[\sum c_n x^n\right] dx = C + \sum \frac{c_n x^{n+1}}{n+1}$ (same radius of convergence).
  - Example: Find the series for $\frac{1}{1+x^2}$ by substituting $-x^2$ into $\frac{1}{1-x}$.

---

## Key Formulas Summary

| Series/Concept | Formula |
|---------------|---------|
| Geometric series sum | $\frac{a}{1-r}$ for $\|r\| < 1$ |
| $p$-series convergence | $\sum \frac{1}{n^p}$ converges iff $p > 1$ |
| Ratio Test | $L = \lim \left\|\frac{a_{n+1}}{a_n}\right\|$; converges if $L < 1$ |
| Alternating series error | $\|S - S_N\| \leq b_{N+1}$ |
| Taylor polynomial | $P_n(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!}(x-a)^k$ |
| Lagrange error bound | $\|R_n(x)\| \leq \frac{M}{(n+1)!}\|x-a\|^{n+1}$ |
| $e^x$ | $\sum \frac{x^n}{n!}$ |
| $\sin x$ | $\sum \frac{(-1)^n x^{2n+1}}{(2n+1)!}$ |
| $\cos x$ | $\sum \frac{(-1)^n x^{2n}}{(2n)!}$ |
| $\frac{1}{1-x}$ | $\sum x^n$, $\|x\| < 1$ |
| $\ln(1+x)$ | $\sum \frac{(-1)^{n+1}x^n}{n}$, $-1 < x \leq 1$ |

## Convergence Tests Decision Guide

| Test | Use When | Conclusion |
|------|----------|------------|
| $n$th Term Test | Always check first | Diverges if $a_n \not\to 0$ |
| Geometric Series | $\sum ar^n$ form | Converges iff $\|r\| < 1$ |
| $p$-Series | $\sum 1/n^p$ form | Converges iff $p > 1$ |
| Integral Test | $f$ continuous, positive, decreasing | Same convergence as $\int f(x)\,dx$ |
| Direct Comparison | Can bound by known series | Smaller than convergent $\Rightarrow$ converges |
| Limit Comparison | Ratio to known series has finite nonzero limit | Same convergence as comparison series |
| Alternating Series | $\sum (-1)^n b_n$ form | Converges if $b_n$ decreasing to $0$ |
| Ratio Test | Factorials, exponentials, $n$th powers | Converges if $L < 1$, diverges if $L > 1$ |

## Common Misconceptions
- The $n$th Term Test can only show divergence, never convergence.
- The Ratio Test is inconclusive when $L = 1$ (must use another test).
- Confusing the radius of convergence with the interval of convergence (endpoints need separate testing).
- Forgetting to check endpoint convergence when finding the interval of convergence.
- Thinking Taylor series always converge to the function (they converge to $f(x)$ only within the interval of convergence).
- Forgetting that differentiation and integration of power series preserve the radius (but may change endpoint behavior).
- Assuming the Lagrange error bound gives the exact error (it gives an upper bound).
