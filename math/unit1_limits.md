# Unit 1: Limits and Continuity
> AB Exam Weight: 10–12% | BC Exam Weight: 4–7% | ~22–23 Class Periods

---

## Topics

### 1.1 Introducing Calculus: Can Change Occur at an Instant?
- Calculus grew from the question of whether change can be measured at a single moment, not just over an interval.
- Average rate of change on $[a, b]$: $\frac{f(b) - f(a)}{b - a}$
- This formula breaks down when the interval has zero width — that's exactly the problem limits are designed to solve.
- Instantaneous rate of change is defined as the limiting value of average rates as the interval shrinks to zero.

### 1.2 Defining Limits and Using Limit Notation
- $\lim_{x \to c} f(x) = L$ means we can make $f(x)$ as close to $L$ as we like by choosing $x$ close enough to $c$ — the value of $f(c)$ itself is irrelevant.
- A limit describes the behavior of a function near a point, not at that point.
- The same limit concept can be expressed through a graph, a table of values, or an algebraic expression — all three ways convey the same underlying idea.

### 1.3 Estimating Limit Values from Graphs
- Reading a limit from a graph means watching where $f(x)$ is heading as $x$ approaches a value from both sides.
- A graph can suggest a limit strongly without proving it; visual evidence should be treated as an estimate, not a guarantee.

### 1.4 Estimating Limit Values from Tables
- A table of values can give a strong numerical hint about a limit by showing what $f(x)$ approaches as $x$ closes in on a target from the left and right.
- Numerical patterns are suggestive, not conclusive — a table can agree on the wrong answer if the function behaves unexpectedly between the sampled points.

### 1.5 Determining Limits Using Algebraic Properties of Limits
- When individual limits exist, the limit of a combined expression obeys predictable rules:
  - **Sum Rule:** $\lim_{x \to c}[f(x) + g(x)] = \lim_{x \to c} f(x) + \lim_{x \to c} g(x)$
  - **Difference Rule:** $\lim_{x \to c}[f(x) - g(x)] = \lim_{x \to c} f(x) - \lim_{x \to c} g(x)$
  - **Product Rule:** $\lim_{x \to c}[f(x) \cdot g(x)] = \lim_{x \to c} f(x) \cdot \lim_{x \to c} g(x)$
  - **Quotient Rule:** $\lim_{x \to c}\frac{f(x)}{g(x)} = \frac{\lim_{x \to c} f(x)}{\lim_{x \to c} g(x)}$, provided the denominator limit is not zero
  - **Constant Multiple Rule:** $\lim_{x \to c}[k \cdot f(x)] = k \cdot \lim_{x \to c} f(x)$
  - **Power Rule:** $\lim_{x \to c}[f(x)]^n = [\lim_{x \to c} f(x)]^n$

### 1.6 Determining Limits Using Algebraic Manipulation
- When direct substitution produces $\frac{0}{0}$, the expression is indeterminate and must be rewritten first — by factoring, multiplying by a conjugate, or applying trigonometric identities.
- Two standard limits worth memorizing:
  - $\lim_{x \to 0} \frac{\sin x}{x} = 1$
  - $\lim_{x \to 0} \frac{1 - \cos x}{x} = 0$

### 1.7 Selecting Procedures for Determining Limits
- Choosing the right technique — direct substitution, factoring, rationalizing, or a trig identity — depends on recognizing the form of the expression first.
- A common pitfall is jumping straight to direct substitution without checking whether the form is actually determinate.

### 1.8 Determining Limits Using the Squeeze Theorem
- **Squeeze Theorem:** If $g(x) \leq f(x) \leq h(x)$ near $c$ and $\lim_{x \to c} g(x) = \lim_{x \to c} h(x) = L$, then $\lim_{x \to c} f(x) = L$.
- This theorem is useful when a function oscillates in a way that's hard to evaluate directly, but can be trapped between two simpler functions with the same limit.
- Classic application: $\lim_{x \to 0} x \sin\left(\frac{1}{x}\right) = 0$

### 1.9 Connecting Multiple Representations of Limits
- The same limit can appear as a formula, a graph, or a table — being comfortable with all three and translating between them is a core calculus skill.
- Understanding a limit concept fully means being able to recognize and work with it regardless of which representation is presented.

### 1.10 Exploring Types of Discontinuities
- **Removable discontinuity (hole):** $\lim_{x \to c} f(x)$ exists but either $f(c)$ is undefined, or $f(c)$ doesn't match the limit.
- **Jump discontinuity:** The left-hand limit and right-hand limit both exist but are not equal: $\lim_{x \to c^-} f(x) \neq \lim_{x \to c^+} f(x)$
- **Infinite discontinuity:** $\lim_{x \to c} f(x) = \pm\infty$ — the function blows up near $c$.
- A function with a hole is discontinuous unless the hole is explicitly filled in by the function value.

### 1.11 Defining Continuity at a Point
- A function $f$ is continuous at $x = c$ when all three conditions hold:
  1. $f(c)$ is defined
  2. $\lim_{x \to c} f(x)$ exists
  3. $\lim_{x \to c} f(x) = f(c)$
- Polynomial functions are continuous everywhere; rational functions are continuous wherever the denominator is nonzero.

### 1.12 Confirming Continuity over an Interval
- A function is continuous on an open interval $(a, b)$ when it is continuous at every single point in that interval.
- Continuity on a closed interval $[a, b]$ adds right-continuity at $a$ and left-continuity at $b$ to the above requirement.

### 1.13 Removing Discontinuities
- A removable discontinuity can be patched by defining (or redefining) the function value at that point to match the limit.
- If $\lim_{x \to c} f(x) = L$, setting $f(c) = L$ makes the function continuous at $c$.

### 1.14 Connecting Infinite Limits and Vertical Asymptotes
- A vertical asymptote at $x = c$ occurs when $f(x)$ grows without bound as $x$ approaches $c$ from either side.
- Formally: if $\lim_{x \to c^+} f(x) = \pm\infty$ or $\lim_{x \to c^-} f(x) = \pm\infty$, then $x = c$ is a vertical asymptote.
- A vertical asymptote does not mean the function equals infinity — it means the function keeps growing without any upper (or lower) bound.

### 1.15 Connecting Limits at Infinity and Horizontal Asymptotes
- If $f(x)$ settles toward a fixed value $L$ as $x \to \infty$ or $x \to -\infty$, the line $y = L$ is a horizontal asymptote.
- For rational functions $\frac{p(x)}{q(x)}$, the end behavior depends on comparing degrees:
  - Degree of $p$ < degree of $q$: horizontal asymptote at $y = 0$
  - Degree of $p$ = degree of $q$: horizontal asymptote at $y = \frac{\text{leading coeff of } p}{\text{leading coeff of } q}$
  - Degree of $p$ > degree of $q$: no horizontal asymptote
- A function can cross its own horizontal asymptote — the asymptote only describes long-run behavior.

### 1.16 Working with the Intermediate Value Theorem (IVT)
- **Intermediate Value Theorem:** If $f$ is continuous on $[a, b]$ and $k$ is any value strictly between $f(a)$ and $f(b)$, then at least one $c$ in $(a, b)$ satisfies $f(c) = k$.
- The IVT is an existence guarantee — it tells you a solution must be somewhere in the interval, but not where exactly.
- The continuity condition on the closed interval is required and must be checked before applying the theorem.

---

## Key Formulas Summary

| Formula | Expression |
|---------|-----------|
| Average rate of change | $\frac{f(b) - f(a)}{b - a}$ |
| Limit of $\sin x / x$ | $\lim_{x \to 0} \frac{\sin x}{x} = 1$ |
| Limit of $(1-\cos x)/x$ | $\lim_{x \to 0} \frac{1 - \cos x}{x} = 0$ |
| Continuity at a point | $f(c)$ defined, $\lim_{x \to c} f(x)$ exists, $\lim_{x \to c} f(x) = f(c)$ |

## Common Misconceptions
- Confusing "limit exists" with "function is defined" at a point.
- Assuming a limit equals the function value without checking continuity.
- Thinking the Squeeze Theorem requires $f(x)$ to be bounded everywhere (it only needs to be bounded near $c$).
- Believing IVT gives an exact value rather than just guaranteeing existence.
- Using numerical/graphical evidence alone as proof that a limit exists or has a particular value.
