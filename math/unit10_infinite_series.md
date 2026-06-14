# Unit 10: Infinite Sequences and Series
> BC Only | BC Exam Weight: 17–18% | ~17–18 Class Periods

---

## Topics

### 10.1 Defining Convergent and Divergent Infinite Series
- An **infinite series** is the sum of an unending list of terms: $\sum_{n=1}^{\infty} a_n = a_1 + a_2 + a_3 + \cdots$
- To make sense of "adding infinitely many numbers," we look at the sequence of **partial sums** $S_n = \sum_{k=1}^{n} a_k$.
- The series **converges** if the partial sums approach a finite limit $S$ as $n \to \infty$; if they grow without bound or oscillate, the series **diverges**.
- A **sequence** $\{a_n\}$ is a separate object: it converges if $\lim_{n \to \infty} a_n = L$ exists.

### 10.2 Working with Geometric Series
- A **geometric series** multiplies each term by a fixed ratio $r$: $\sum_{n=0}^{\infty} ar^n = a + ar + ar^2 + \cdots$
- The rule is clean: the series **converges** to $S = \dfrac{a}{1-r}$ when $|r| < 1$, and **diverges** when $|r| \geq 1$.
- Geometric series are the primary tool for computing sums; reindexing or multiplying by constants can transform related series into geometric form.

### 10.3 The $n$th Term Test for Divergence
- If the terms of a series do not approach zero, the partial sums cannot settle down to a finite value:
  $$\lim_{n \to \infty} a_n \neq 0 \implies \sum a_n \text{ diverges}$$
- The converse is **false**: $a_n \to 0$ does not guarantee convergence. The harmonic series $\sum \frac{1}{n}$ diverges even though its terms go to zero — this is the single most important cautionary example in the whole unit.
- The $n$th Term Test can only prove divergence, never convergence.

### 10.4 Integral Test for Convergence
- When $f$ is continuous, positive, and strictly decreasing for $x \geq N$, and $a_n = f(n)$, the series and the improper integral share the same convergence fate:
  $$\sum_{n=N}^{\infty} a_n \text{ and } \int_N^{\infty} f(x)\,dx \text{ either both converge or both diverge.}$$
- The Integral Test tells you whether the series converges — it does not compute what the series converges *to*.

### 10.5 Harmonic Series and $p$-Series
- A **$p$-series** has the form $\sum_{n=1}^{\infty} \frac{1}{n^p}$. The cutoff is at $p = 1$:
  - Converges when $p > 1$
  - Diverges when $p \leq 1$
- The **harmonic series** ($p = 1$) diverges — slowly, but unmistakably.
- Quick examples: $\sum \frac{1}{n^2}$ converges ($p = 2 > 1$); $\sum \frac{1}{\sqrt{n}}$ diverges ($p = \frac{1}{2} \leq 1$).

### 10.6 Comparison Tests for Convergence
- When a series is not in a standard form, compare it to one whose behavior is known.
- **Direct Comparison Test:** For $0 \leq a_n \leq b_n$:
  - If the bigger series $\sum b_n$ converges, so does $\sum a_n$.
  - If the smaller series $\sum a_n$ diverges, so does $\sum b_n$.
- **Limit Comparison Test:** If $a_n > 0$, $b_n > 0$, and $\lim_{n \to \infty} \frac{a_n}{b_n} = L$ with $0 < L < \infty$, then $\sum a_n$ and $\sum b_n$ either both converge or both diverge.
- The comparison target is almost always a $p$-series or geometric series.

### 10.7 Alternating Series Test for Convergence
- An alternating series whose terms shrink monotonically to zero is guaranteed to converge. Specifically, $\sum_{n=1}^{\infty} (-1)^{n+1} b_n$ converges when all three conditions hold:
  1. $b_n > 0$ for all $n$
  2. $b_{n+1} \leq b_n$ (terms are non-increasing in size)
  3. $\lim_{n \to \infty} b_n = 0$
- The alternating harmonic series $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n}$ is the go-to example: it converges to $\ln 2$, even though the corresponding all-positive series diverges.

### 10.8 Ratio Test for Convergence
- The Ratio Test measures how quickly consecutive terms shrink by examining their ratio in the limit:
  $$L = \lim_{n \to \infty} \left|\frac{a_{n+1}}{a_n}\right|$$
  - $L < 1$: series **converges absolutely**
  - $L > 1$ or $L = \infty$: series **diverges**
  - $L = 1$: test gives **no information** — try a different test
- This test shines when factorials, exponentials, or $n$th powers appear in the terms.

### 10.9 Determining Absolute or Conditional Convergence
- A series **converges absolutely** if $\sum |a_n|$ converges. Absolute convergence is the stronger condition, and it implies ordinary convergence.
- A series **converges conditionally** if it converges but $\sum |a_n|$ diverges — the alternating signs are doing essential work.
- Example: $\sum \frac{(-1)^n}{n}$ converges conditionally because the alternating harmonic series converges, yet $\sum \frac{1}{n}$ diverges.

### 10.10 Alternating Series Error Bound
- When a series satisfies the Alternating Series Test conditions and we stop at the $N$th partial sum $S_N$, the actual error is no larger than the first omitted term:
  $$|S - S_N| \leq b_{N+1}$$
- This gives a concrete way to ask "how many terms do I need?" — keep adding terms until $b_{N+1}$ drops below the desired tolerance.

### 10.11 Finding Taylor Polynomial Approximations of Functions
- A **Taylor polynomial** approximates a smooth function near a center point $a$ by matching the function's derivatives at that point:
  $$P_n(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!}(x - a)^k = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \cdots$$
- When $a = 0$, this is called a **Maclaurin polynomial**.
- Higher-degree polynomials hug the function more closely near $x = a$, but may diverge further away.

### 10.12 Lagrange Error Bound
- The Lagrange error bound quantifies how far a Taylor polynomial strays from the true function. If the $(n+1)$th derivative satisfies $|f^{(n+1)}(c)| \leq M$ for all $c$ between $a$ and $x$, then:
  $$|R_n(x)| = |f(x) - P_n(x)| \leq \frac{M}{(n+1)!}|x - a|^{n+1}$$
- Finding the bound $M$ requires estimating (or maximizing) the $(n+1)$th derivative on the relevant interval — this is usually the trickiest part of applying the formula.

### 10.13 Radius and Interval of Convergence of Power Series
- A **power series** centered at $a$ is $\sum_{n=0}^{\infty} c_n(x - a)^n$ — an infinite polynomial in powers of $(x - a)$.
- Every power series has a **radius of convergence** $R$: it converges for $|x - a| < R$ and diverges for $|x - a| > R$.
- Apply the Ratio Test to find $R$: $R = \lim_{n \to \infty} \left|\dfrac{c_n}{c_{n+1}}\right|$ when the limit exists.
- The **interval of convergence** is $(a - R,\, a + R)$, but the endpoints $x = a \pm R$ must be checked individually with other convergence tests.
- Edge cases: $R = 0$ means the series converges only at the center; $R = \infty$ means it converges everywhere.

### 10.14 Finding Taylor or Maclaurin Series for a Function
- The full **Taylor series** of $f$ centered at $a$ is the infinite-degree version:
  $$\sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!}(x - a)^n$$
- Five Maclaurin series worth internalizing:
  - $e^x = \sum_{n=0}^{\infty} \dfrac{x^n}{n!} = 1 + x + \dfrac{x^2}{2!} + \dfrac{x^3}{3!} + \cdots$ (all $x$)
  - $\sin x = \sum_{n=0}^{\infty} \dfrac{(-1)^n x^{2n+1}}{(2n+1)!} = x - \dfrac{x^3}{3!} + \dfrac{x^5}{5!} - \cdots$ (all $x$)
  - $\cos x = \sum_{n=0}^{\infty} \dfrac{(-1)^n x^{2n}}{(2n)!} = 1 - \dfrac{x^2}{2!} + \dfrac{x^4}{4!} - \cdots$ (all $x$)
  - $\dfrac{1}{1-x} = \sum_{n=0}^{\infty} x^n = 1 + x + x^2 + x^3 + \cdots$ ($|x| < 1$)
  - $\ln(1+x) = \sum_{n=1}^{\infty} \dfrac{(-1)^{n+1} x^n}{n} = x - \dfrac{x^2}{2} + \dfrac{x^3}{3} - \cdots$ ($-1 < x \leq 1$)

### 10.15 Representing Functions as Power Series
- Once you know a few key series, you can generate many more by algebraic manipulation within the interval of convergence:
  - **Substitution:** replace $x$ with an expression, e.g., $e^{-x^2} = \sum \dfrac{(-x^2)^n}{n!} = \sum \dfrac{(-1)^n x^{2n}}{n!}$
  - **Multiplication:** scale by $x^k$ or a constant
  - **Addition/Subtraction:** combine term by term
  - **Differentiation:** $\dfrac{d}{dx}\!\left[\sum c_n x^n\right] = \sum n c_n x^{n-1}$ — radius of convergence unchanged
  - **Integration:** $\displaystyle\int \!\left[\sum c_n x^n\right] dx = C + \sum \dfrac{c_n x^{n+1}}{n+1}$ — radius of convergence unchanged
- Example: $\dfrac{1}{1+x^2}$ comes from substituting $-x^2$ into $\dfrac{1}{1-x}$.

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
- The $n$th Term Test can only establish divergence — passing it ($a_n \to 0$) tells you nothing about whether the series converges.
- When the Ratio Test gives $L = 1$, it is genuinely uninformative; switching to another test is required.
- The radius of convergence $R$ describes an open interval; the endpoints $a \pm R$ sit right at the boundary and each needs its own convergence check.
- A Taylor series converges to $f(x)$ only within its interval of convergence — outside that interval, the partial sums can behave erratically.
- Differentiating or integrating a power series preserves the radius of convergence, but endpoint behavior can change.
- The Lagrange error bound gives a worst-case **upper bound** on the error, not the actual error — the true error could be much smaller.
