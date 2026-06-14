# Unit 6: Integration and Accumulation of Change
> AB Exam Weight: 17–20% | BC Exam Weight: 17–20% | ~18–20 Class Periods

---

## Topics

### 6.1 Exploring Accumulations of Change
- Integration measures how quantities accumulate over time: if $r(t)$ is a rate of change, then $\int_a^b r(t)\,dt$ gives the net change from $t = a$ to $t = b$.
- When velocity $v(t)$ is the rate, $\int_a^b v(t)\,dt$ tells you net displacement — positive regions add up, negative regions subtract out.

### 6.2 Approximating Areas with Riemann Sums
- Before computing exact integrals, we can estimate area under a curve by dividing $[a, b]$ into $n$ equal-width strips and adding up rectangle areas.
- **Left Riemann Sum:** $\sum_{i=0}^{n-1} f(x_i) \Delta x$ — uses left edge of each strip
- **Right Riemann Sum:** $\sum_{i=1}^{n} f(x_i) \Delta x$ — uses right edge of each strip
- **Midpoint Riemann Sum:** $\sum_{i=1}^{n} f\!\left(\frac{x_{i-1}+x_i}{2}\right) \Delta x$ — uses midpoint; often more accurate
- **Trapezoidal Sum:** $\sum_{i=1}^{n} \frac{f(x_{i-1})+f(x_i)}{2} \Delta x$ — averages the two edges, connecting corners with a straight line
- For an **increasing** function, the left sum underestimates and the right sum overestimates; the pattern flips for a **decreasing** function.

### 6.3 Riemann Sums, Summation Notation, and Definite Integral Notation
- As $n \to \infty$, the Riemann sums converge to the exact area. The formal definition is:
  $$\int_a^b f(x)\,dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_i^*) \Delta x, \quad \Delta x = \frac{b-a}{n}$$
- This limit exists whenever $f$ is continuous on $[a, b]$ — and even for some functions with a finite number of jump discontinuities.

### 6.4 The Fundamental Theorem of Calculus and Accumulation Functions
- **FTC Part 1** links differentiation and integration: if $f$ is continuous on $[a, b]$, then the accumulation function $g(x) = \int_a^x f(t)\,dt$ is differentiable, and:
  $$\frac{d}{dx}\left[\int_a^x f(t)\,dt\right] = f(x)$$
- When the upper limit is a composed function, the chain rule kicks in:
  $$\frac{d}{dx}\left[\int_a^{u(x)} f(t)\,dt\right] = f(u(x)) \cdot u'(x)$$
- In plain terms: differentiation undoes integration, and integration undoes differentiation.

### 6.5 Interpreting the Behavior of Accumulation Functions Involving Area
- For $g(x) = \int_a^x f(t)\,dt$, the sign of $f$ directly controls the shape of $g$:
  - $g$ increases where $f(x) > 0$; decreases where $f(x) < 0$.
  - $g$ has a local max where $f$ changes from positive to negative; a local min where $f$ changes from negative to positive.
  - $g$ is concave up where $f$ is increasing; concave down where $f$ is decreasing.

### 6.6 Applying Properties of Definite Integrals
- These algebraic rules follow directly from the geometry of signed area:
  - $\int_a^a f(x)\,dx = 0$ (zero-width interval)
  - $\int_a^b f(x)\,dx = -\int_b^a f(x)\,dx$ (reversing limits flips sign)
  - $\int_a^b [f(x) \pm g(x)]\,dx = \int_a^b f(x)\,dx \pm \int_a^b g(x)\,dx$
  - $\int_a^b kf(x)\,dx = k\int_a^b f(x)\,dx$
  - $\int_a^b f(x)\,dx = \int_a^c f(x)\,dx + \int_c^b f(x)\,dx$ (splitting at any interior point)

### 6.7 The Fundamental Theorem of Calculus and Definite Integrals
- **FTC Part 2** gives a practical evaluation method: if $F$ is any antiderivative of $f$, then:
  $$\int_a^b f(x)\,dx = F(b) - F(a)$$
- This is why finding antiderivatives matters — once you have one, evaluating a definite integral is just arithmetic.
- Net change interpretation: $\int_a^b f'(x)\,dx = f(b) - f(a)$.

### 6.8 Finding Antiderivatives and Indefinite Integrals: Basic Rules and Notation
- An antiderivative reverses differentiation. The full family of antiderivatives always includes $+ C$:
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
- Omitting $+ C$ in an indefinite integral is always wrong — it represents infinitely many valid antiderivatives.

### 6.9 Integrating Using Substitution
- $u$-substitution is the chain rule run in reverse: when the integrand looks like $f(g(x)) \cdot g'(x)$, set $u = g(x)$:
  $$\int f(g(x)) \cdot g'(x)\,dx = \int f(u)\,du$$
- For definite integrals, convert the limits to $u$-values right away:
  $$\int_a^b f(g(x))g'(x)\,dx = \int_{g(a)}^{g(b)} f(u)\,du$$
- The key skill is recognizing a composite function and spotting its inner derivative (or a constant multiple of it) already present in the integrand.

### 6.10 Integrating Functions Using Long Division and Completing the Square
- When the numerator degree is at least as large as the denominator degree, do polynomial long division first to get an integrable form.
- Completing the square converts quadratic denominators into forms that match the arctan or arcsin antiderivative templates.
- Example: $\int \frac{1}{x^2 + 4x + 8}\,dx$ — complete the square to get $\int \frac{1}{(x+2)^2 + 4}\,dx$, then use the arctan rule.

### 6.11 Integrating Using Integration by Parts (BC Only)
- Integration by parts is the product rule in reverse:
  $$\int u\,dv = uv - \int v\,du$$
- Choosing $u$ well is the whole game. The LIATE order is a useful guide: prefer Logarithmic, then Inverse trig, then Algebraic, then Trigonometric, then Exponential for $u$.
- Some integrals require applying the formula more than once; the tabular method organizes repeated application efficiently.

### 6.12 Integrating Using Linear Partial Fractions (BC Only)
- When a rational function has a denominator that factors into distinct linear pieces, break it apart before integrating:
  $$\frac{1}{(x-1)(x+2)} = \frac{A}{x-1} + \frac{B}{x+2}$$
- Solve for the constants $A$, $B$, etc. by substituting strategic values of $x$ or by matching coefficients, then integrate each simpler fraction using the $\ln|x|$ rule.

### 6.13 Evaluating Improper Integrals (BC Only)
- An integral is "improper" when a limit of integration is $\pm\infty$ or the integrand blows up inside the interval. In either case, replace the problematic boundary with a variable and take a limit:
  $$\int_a^{\infty} f(x)\,dx = \lim_{b \to \infty} \int_a^b f(x)\,dx$$
- The integral **converges** if the limit is a finite number; otherwise it **diverges**.
- Benchmark result: $\int_1^{\infty} \frac{1}{x^p}\,dx$ converges when $p > 1$ and diverges when $p \leq 1$.

### 6.14 Selecting Techniques for Antidifferentiation
- No single technique works for every integral. Before computing, look at the integrand's structure:
  - Is it a basic rule match? Use the table directly.
  - Is it composite with its inner derivative present? Try $u$-substitution.
  - Is the numerator degree too high? Do long division.
  - Does the quadratic denominator not factor nicely? Complete the square.
  - Is it a product of two unrelated function types? Try integration by parts (BC).
  - Is it a rational function with factorable denominator? Try partial fractions (BC).
- Pattern recognition, not memorized procedures, is the skill being developed here.

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
- Omitting the constant of integration $C$ in indefinite integrals — every indefinite integral has a family of answers.
- Treating $\int_a^b f(x)\,dx$ as total area when it actually gives net signed area; to get total area, integrate $|f(x)|$.
- Forgetting to update the limits of integration when applying $u$-substitution to a definite integral.
- Writing $\int \frac{1}{x}\,dx = \frac{x^0}{0}$ — the power rule breaks down at $n = -1$; the answer is $\ln|x| + C$.
- Forgetting the chain rule multiplier when differentiating an accumulation function $\int_a^{u(x)} f(t)\,dt$.
- Mixing up which Riemann sum overestimates vs. underestimates depending on whether the function is increasing or decreasing.
