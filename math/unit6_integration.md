# Unit 6: Integration and Accumulation of Change
> AB Exam Weight: 17–20% | BC Exam Weight: 17–20% | ~18–20 Class Periods

## Big Ideas: CHA, LIM, FUN

---

## Topics

### 6.1 Exploring Accumulations of Change
- **Learning Objective (CHA-4.A):** Interpret the meaning of a definite integral as accumulation.
- **Essential Knowledge:**
  - A definite integral represents the accumulation of change over an interval.
  - If $r(t)$ is a rate of change, then $\int_a^b r(t)\,dt$ gives the net change from $t = a$ to $t = b$.
  - Example: If $v(t)$ is velocity, $\int_a^b v(t)\,dt$ is the net displacement.

### 6.2 Approximating Areas with Riemann Sums
- **Learning Objective (LIM-5.A):** Approximate definite integrals using Riemann sums.
- **Essential Knowledge:**
  - **Left Riemann Sum:** $\sum_{i=0}^{n-1} f(x_i) \Delta x$
  - **Right Riemann Sum:** $\sum_{i=1}^{n} f(x_i) \Delta x$
  - **Midpoint Riemann Sum:** $\sum_{i=1}^{n} f\left(\frac{x_{i-1}+x_i}{2}\right) \Delta x$
  - **Trapezoidal Sum:** $\sum_{i=1}^{n} \frac{f(x_{i-1})+f(x_i)}{2} \Delta x$
  - For increasing functions: Left sum is underestimate, Right sum is overestimate.
  - For decreasing functions: Left sum is overestimate, Right sum is underestimate.

### 6.3 Riemann Sums, Summation Notation, and Definite Integral Notation
- **Learning Objective (LIM-5.A):** Connect Riemann sums to definite integrals.
- **Essential Knowledge:**
  - **Definite integral as a limit of Riemann sums:**
    $$\int_a^b f(x)\,dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*) \Delta x$$
    where $\Delta x = \frac{b-a}{n}$
  - The definite integral exists if $f$ is continuous on $[a, b]$ (and for some discontinuous functions).

### 6.4 The Fundamental Theorem of Calculus and Accumulation Functions
- **Learning Objective (FUN-5.A):** Apply the Fundamental Theorem of Calculus (Part 1).
- **Essential Knowledge:**
  - **FTC Part 1:** If $f$ is continuous on $[a, b]$, then $g(x) = \int_a^x f(t)\,dt$ is differentiable and:
    $$\frac{d}{dx}\left[\int_a^x f(t)\,dt\right] = f(x)$$
  - With chain rule: $\frac{d}{dx}\left[\int_a^{u(x)} f(t)\,dt\right] = f(u(x)) \cdot u'(x)$
  - This establishes that differentiation and integration are inverse processes.

### 6.5 Interpreting the Behavior of Accumulation Functions Involving Area
- **Learning Objective (FUN-5.A):** Analyze accumulation functions.
- **Essential Knowledge:**
  - $g(x) = \int_a^x f(t)\,dt$ is increasing where $f(x) > 0$ and decreasing where $f(x) < 0$.
  - $g$ has a local max where $f$ changes from positive to negative.
  - $g$ has a local min where $f$ changes from negative to positive.
  - $g$ is concave up where $f$ is increasing; concave down where $f$ is decreasing.

### 6.6 Applying Properties of Definite Integrals
- **Learning Objective (FUN-6.A):** Apply properties of definite integrals.
- **Essential Knowledge:**
  - $\int_a^a f(x)\,dx = 0$
  - $\int_a^b f(x)\,dx = -\int_b^a f(x)\,dx$
  - $\int_a^b [f(x) \pm g(x)]\,dx = \int_a^b f(x)\,dx \pm \int_a^b g(x)\,dx$
  - $\int_a^b kf(x)\,dx = k\int_a^b f(x)\,dx$
  - $\int_a^b f(x)\,dx = \int_a^c f(x)\,dx + \int_c^b f(x)\,dx$

### 6.7 The Fundamental Theorem of Calculus and Definite Integrals
- **Learning Objective (FUN-6.B):** Apply the Fundamental Theorem of Calculus (Part 2).
- **Essential Knowledge:**
  - **FTC Part 2:** If $f$ is continuous on $[a, b]$ and $F$ is any antiderivative of $f$, then:
    $$\int_a^b f(x)\,dx = F(b) - F(a)$$
  - This provides a method to evaluate definite integrals using antiderivatives.
  - Net change: $\int_a^b f'(x)\,dx = f(b) - f(a)$

### 6.8 Finding Antiderivatives and Indefinite Integrals: Basic Rules and Notation
- **Learning Objective (FUN-6.C):** Find antiderivatives.
- **Essential Knowledge:**
  - $\int x^n\,dx = \frac{x^{n+1}}{n+1} + C$ (for $n \neq -1$)
  - $\int \frac{1}{x}\,dx = \ln|x| + C$
  - $\int e^x\,dx = e^x + C$
  - $\int a^x\,dx = \frac{a^x}{\ln a} + C$
  - $\int \sin x\,dx = -\cos x + C$
  - $\int \cos x\,dx = \sin x + C$
  - $\int \sec^2 x\,dx = \tan x + C$
  - $\int \csc^2 x\,dx = -\cot x + C$
  - $\int \sec x \tan x\,dx = \sec x + C$
  - $\int \csc x \cot x\,dx = -\csc x + C$
  - $\int \frac{1}{\sqrt{1-x^2}}\,dx = \arcsin x + C$
  - $\int \frac{1}{1+x^2}\,dx = \arctan x + C$
  - Always include $+ C$ for indefinite integrals.

### 6.9 Integrating Using Substitution
- **Learning Objective (FUN-6.D):** Evaluate integrals using $u$-substitution.
- **Essential Knowledge:**
  - **$u$-substitution** reverses the chain rule: $\int f(g(x)) \cdot g'(x)\,dx = \int f(u)\,du$
  - For definite integrals, change the limits when substituting: $\int_a^b f(g(x))g'(x)\,dx = \int_{g(a)}^{g(b)} f(u)\,du$
  - Strategy: Look for a composite function and its inner derivative.

### 6.10 Integrating Functions Using Long Division and Completing the Square
- **Learning Objective (FUN-6.D):** Evaluate integrals by algebraic manipulation.
- **Essential Knowledge:**
  - When the degree of the numerator $\geq$ the degree of the denominator, use long division first.
  - Complete the square to put expressions in a form that matches inverse trig antiderivative formulas.
  - Example: $\int \frac{1}{x^2 + 4x + 8}\,dx$ — complete the square to get $\int \frac{1}{(x+2)^2 + 4}\,dx$, then use arctan.

### 6.11 Integrating Using Integration by Parts (BC Only)
- **Learning Objective (FUN-6.E):** Evaluate integrals using integration by parts.
- **Essential Knowledge:**
  - **Integration by Parts:** $\int u\,dv = uv - \int v\,du$
  - LIATE mnemonic for choosing $u$: Logarithmic, Inverse trig, Algebraic, Trigonometric, Exponential.
  - May need to apply multiple times.
  - Tabular method can speed up repeated application.

### 6.12 Integrating Using Linear Partial Fractions (BC Only)
- **Learning Objective (FUN-6.E):** Decompose rational functions for integration.
- **Essential Knowledge:**
  - Decompose $\frac{P(x)}{Q(x)}$ into partial fractions when $Q(x)$ has distinct linear factors.
  - Example: $\frac{1}{(x-1)(x+2)} = \frac{A}{x-1} + \frac{B}{x+2}$
  - Solve for constants $A$, $B$, etc., then integrate each term.

### 6.13 Evaluating Improper Integrals (BC Only)
- **Learning Objective (LIM-6.A):** Evaluate improper integrals.
- **Essential Knowledge:**
  - **Improper integral (infinite interval):** $\int_a^{\infty} f(x)\,dx = \lim_{b \to \infty} \int_a^b f(x)\,dx$
  - **Improper integral (discontinuity):** If $f$ has a discontinuity at $c \in [a, b]$, split and take limits.
  - An improper integral converges if the limit exists (is finite); otherwise it diverges.
  - Key result: $\int_1^{\infty} \frac{1}{x^p}\,dx$ converges if $p > 1$ and diverges if $p \leq 1$.

### 6.14 Selecting Techniques for Antidifferentiation
- **Learning Objective (FUN-6.D):** Select appropriate integration techniques.
- **Essential Knowledge:**
  - Students must identify the best technique: basic rules, $u$-substitution, long division, completing the square, integration by parts (BC), or partial fractions (BC).
  - Strategy: analyze the structure of the integrand before integrating.

---

## Key Formulas Summary

| Integral | Result |
|----------|--------|
| $\int x^n\,dx$ | $\frac{x^{n+1}}{n+1} + C$ ($n \neq -1$) |
| $\int \frac{1}{x}\,dx$ | $\ln\|x\| + C$ |
| $\int e^x\,dx$ | $e^x + C$ |
| $\int \sin x\,dx$ | $-\cos x + C$ |
| $\int \cos x\,dx$ | $\sin x + C$ |
| $\int \sec^2 x\,dx$ | $\tan x + C$ |
| $\int \frac{1}{\sqrt{1-x^2}}\,dx$ | $\arcsin x + C$ |
| $\int \frac{1}{1+x^2}\,dx$ | $\arctan x + C$ |
| FTC Part 1 | $\frac{d}{dx}\int_a^x f(t)\,dt = f(x)$ |
| FTC Part 2 | $\int_a^b f(x)\,dx = F(b) - F(a)$ |

## Common Misconceptions
- Forgetting the constant of integration $C$ in indefinite integrals.
- Confusing $\int_a^b f(x)\,dx$ (net signed area) with total area $\int_a^b |f(x)|\,dx$.
- Forgetting to change bounds when using $u$-substitution with definite integrals.
- Thinking $\int \frac{1}{x}\,dx = \frac{x^0}{0}$ instead of $\ln|x| + C$.
- Misapplying FTC Part 1 when the upper limit is a function: forgetting the chain rule factor.
- Confusing left/right Riemann sum overestimates/underestimates for increasing vs. decreasing functions.
