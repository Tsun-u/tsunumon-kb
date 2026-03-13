# Unit 1: Limits and Continuity
> AB Exam Weight: 10–12% | BC Exam Weight: 4–7% | ~22–23 Class Periods

## Big Ideas: LIM, CHA

---

## Topics

### 1.1 Introducing Calculus: Can Change Occur at an Instant?
- **Learning Objective (CHA-1.A):** Interpret the rate of change at an instant in terms of average rates of change over intervals containing that instant.
- **Essential Knowledge:**
  - Calculus uses limits to understand and model dynamic change.
  - Average rate of change over $[a, b]$: $\frac{f(b) - f(a)}{b - a}$
  - The limit concept allows us to define instantaneous rate of change in terms of average rates of change.
  - Average rate of change is undefined at a point where the change in the independent variable would be zero.

### 1.2 Defining Limits and Using Limit Notation
- **Learning Objective (LIM-1.A):** Represent limits analytically using correct notation.
- **Learning Objective (LIM-1.B):** Interpret limits expressed in analytic notation.
- **Essential Knowledge:**
  - $\lim_{x \to c} f(x) = L$ means $f(x)$ can be made arbitrarily close to $L$ by taking $x$ sufficiently close to $c$ (but not equal to $c$).
  - A limit can be expressed numerically, graphically, and analytically.
  - The limit of $f(x)$ as $x$ approaches $c$ does not depend on the value of $f(c)$.

### 1.3 Estimating Limit Values from Graphs
- **Learning Objective (LIM-1.B):** Interpret limits expressed in analytic notation.
- **Essential Knowledge:**
  - Limits can be estimated from graphs by observing the behavior of $f(x)$ as $x$ approaches a value.
  - Graphical information may be incomplete or misleading; careful analysis is needed.

### 1.4 Estimating Limit Values from Tables
- **Learning Objective (LIM-1.C):** Estimate limits of functions.
- **Essential Knowledge:**
  - Limits can be estimated from tables of values by observing patterns as $x$ approaches a value from both sides.
  - Tables may not give complete information; numerical evidence alone is not sufficient to prove a limit exists.

### 1.5 Determining Limits Using Algebraic Properties of Limits
- **Learning Objective (LIM-1.D):** Determine the limits of functions using limit theorems.
- **Essential Knowledge:**
  - **Sum Rule:** $\lim_{x \to c}[f(x) + g(x)] = \lim_{x \to c} f(x) + \lim_{x \to c} g(x)$
  - **Difference Rule:** $\lim_{x \to c}[f(x) - g(x)] = \lim_{x \to c} f(x) - \lim_{x \to c} g(x)$
  - **Product Rule:** $\lim_{x \to c}[f(x) \cdot g(x)] = \lim_{x \to c} f(x) \cdot \lim_{x \to c} g(x)$
  - **Quotient Rule:** $\lim_{x \to c}\frac{f(x)}{g(x)} = \frac{\lim_{x \to c} f(x)}{\lim_{x \to c} g(x)}$, provided the denominator limit is not zero.
  - **Constant Multiple Rule:** $\lim_{x \to c}[k \cdot f(x)] = k \cdot \lim_{x \to c} f(x)$
  - **Power Rule:** $\lim_{x \to c}[f(x)]^n = [\lim_{x \to c} f(x)]^n$

### 1.6 Determining Limits Using Algebraic Manipulation
- **Learning Objective (LIM-1.E):** Determine the limits of functions using equivalent expressions.
- **Essential Knowledge:**
  - Simplify indeterminate forms $\frac{0}{0}$ by factoring, rationalizing (conjugates), or using trigonometric identities.
  - Key limits:
    - $\lim_{x \to 0} \frac{\sin x}{x} = 1$
    - $\lim_{x \to 0} \frac{1 - \cos x}{x} = 0$

### 1.7 Selecting Procedures for Determining Limits
- **Learning Objective (LIM-1.E):** Determine the limits of functions using equivalent expressions.
- **Essential Knowledge:**
  - Students must be able to select the appropriate strategy (direct substitution, factoring, rationalizing, trig identities) based on the form of the expression.
  - Common misconception: Assuming direct substitution always works before checking for indeterminate forms.

### 1.8 Determining Limits Using the Squeeze Theorem
- **Learning Objective (LIM-1.F):** Determine the limits of functions using the squeeze theorem.
- **Essential Knowledge:**
  - **Squeeze Theorem:** If $g(x) \leq f(x) \leq h(x)$ for all $x$ near $c$ (except possibly at $c$), and $\lim_{x \to c} g(x) = \lim_{x \to c} h(x) = L$, then $\lim_{x \to c} f(x) = L$.
  - Classic application: $\lim_{x \to 0} x \sin\left(\frac{1}{x}\right) = 0$

### 1.9 Connecting Multiple Representations of Limits
- **Learning Objective (LIM-1.B):** Interpret limits expressed in analytic notation.
- **Essential Knowledge:**
  - Limits can be expressed and connected across graphical, numerical, and analytical representations.
  - A complete understanding involves being able to move fluently between representations.

### 1.10 Exploring Types of Discontinuities
- **Learning Objective (LIM-2.A):** Determine types of discontinuities.
- **Essential Knowledge:**
  - **Removable discontinuity (hole):** $\lim_{x \to c} f(x)$ exists but $\neq f(c)$, or $f(c)$ is undefined.
  - **Jump discontinuity:** $\lim_{x \to c^-} f(x) \neq \lim_{x \to c^+} f(x)$
  - **Infinite discontinuity:** $\lim_{x \to c} f(x) = \pm\infty$
  - Common misconception: A function with a hole is always discontinuous. (Correct: it is discontinuous unless the hole is "filled" by the function value.)

### 1.11 Defining Continuity at a Point
- **Learning Objective (LIM-2.A):** Determine continuity at a point.
- **Essential Knowledge:**
  - A function $f$ is continuous at $x = c$ if all three conditions hold:
    1. $f(c)$ is defined
    2. $\lim_{x \to c} f(x)$ exists
    3. $\lim_{x \to c} f(x) = f(c)$
  - Polynomial functions are continuous everywhere.
  - Rational functions are continuous on their domains.

### 1.12 Confirming Continuity over an Interval
- **Learning Objective (LIM-2.B):** Determine intervals over which a function is continuous.
- **Essential Knowledge:**
  - A function is continuous on an open interval $(a, b)$ if it is continuous at every point in the interval.
  - Continuity on a closed interval $[a, b]$ requires continuity on $(a, b)$ plus right-continuity at $a$ and left-continuity at $b$.

### 1.13 Removing Discontinuities
- **Learning Objective (LIM-2.A):** Determine types of discontinuities.
- **Essential Knowledge:**
  - A removable discontinuity can be "removed" by redefining the function value at that point to equal the limit.
  - If $\lim_{x \to c} f(x) = L$, define $f(c) = L$ to make $f$ continuous at $c$.

### 1.14 Connecting Infinite Limits and Vertical Asymptotes
- **Learning Objective (LIM-2.C):** Determine vertical asymptotes.
- **Essential Knowledge:**
  - If $\lim_{x \to c^+} f(x) = \pm\infty$ or $\lim_{x \to c^-} f(x) = \pm\infty$, then $x = c$ is a vertical asymptote.
  - Common misconception: A vertical asymptote means the function equals infinity. (Correct: the function increases or decreases without bound.)

### 1.15 Connecting Limits at Infinity and Horizontal Asymptotes
- **Learning Objective (LIM-2.D):** Determine limits at infinity and horizontal asymptotes.
- **Essential Knowledge:**
  - If $\lim_{x \to \infty} f(x) = L$ or $\lim_{x \to -\infty} f(x) = L$, then $y = L$ is a horizontal asymptote.
  - For rational functions $\frac{p(x)}{q(x)}$:
    - If degree of $p$ < degree of $q$: horizontal asymptote at $y = 0$
    - If degree of $p$ = degree of $q$: horizontal asymptote at $y = \frac{\text{leading coeff of } p}{\text{leading coeff of } q}$
    - If degree of $p$ > degree of $q$: no horizontal asymptote
  - A function can cross its horizontal asymptote.

### 1.16 Working with the Intermediate Value Theorem (IVT)
- **Learning Objective (FUN-1.A):** Apply the Intermediate Value Theorem.
- **Essential Knowledge:**
  - **Intermediate Value Theorem:** If $f$ is continuous on $[a, b]$ and $k$ is between $f(a)$ and $f(b)$, then there exists at least one $c$ in $(a, b)$ such that $f(c) = k$.
  - IVT guarantees existence but does not provide the value of $c$.
  - IVT requires continuity on the closed interval — this condition must be verified.
  - Common misconception: IVT tells you the exact location of $c$. (Correct: it only guarantees existence.)

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
