# Unit 3: Differentiation: Composite, Implicit, and Inverse Functions
> AB Exam Weight: 9–13% | BC Exam Weight: 4–7% | ~10–11 Class Periods

---

## Topics

### 3.1 The Chain Rule
- When one function is nested inside another, the derivative picks up a multiplicative factor from the inner function.
- **Chain Rule:** If $y = f(g(x))$, then $\frac{dy}{dx} = f'(g(x)) \cdot g'(x)$
- Leibniz notation: If $y = f(u)$ and $u = g(x)$, then $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$
- Chains can nest deeper: $\frac{d}{dx}[f(g(h(x)))] = f'(g(h(x))) \cdot g'(h(x)) \cdot h'(x)$
- Common applications:
  - $\frac{d}{dx}[e^{g(x)}] = e^{g(x)} \cdot g'(x)$
  - $\frac{d}{dx}[\ln(g(x))] = \frac{g'(x)}{g(x)}$
  - $\frac{d}{dx}[\sin(g(x))] = \cos(g(x)) \cdot g'(x)$
  - $\frac{d}{dx}[[g(x)]^n] = n[g(x)]^{n-1} \cdot g'(x)$

### 3.2 Implicit Differentiation
- When an equation mixes $x$ and $y$ without isolating $y$ (e.g., $x^2 + y^2 = 25$), differentiate both sides with respect to $x$ directly.
- Any term involving $y$ requires the chain rule, which introduces a factor of $\frac{dy}{dx}$.
- After differentiating, collect all $\frac{dy}{dx}$ terms and solve algebraically.
- The result will often contain both $x$ and $y$.
- Example: $x^2 + y^2 = 25 \implies 2x + 2y\frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{x}{y}$

### 3.3 Differentiating Inverse Functions
- If $g$ is the inverse of $f$, then $g'(x) = \frac{1}{f'(g(x))}$, provided $f'(g(x)) \neq 0$.
- Equivalently: if $f(a) = b$, then $(f^{-1})'(b) = \frac{1}{f'(a)}$
- The key idea is that slopes on inverse function graphs are reciprocals of each other, evaluated at the reflected point.
- The graphs of $f$ and $f^{-1}$ are reflections over $y = x$.

### 3.4 Differentiating Inverse Trigonometric Functions
- $\frac{d}{dx}[\arcsin x] = \frac{1}{\sqrt{1 - x^2}}$, for $|x| < 1$
- $\frac{d}{dx}[\arccos x] = -\frac{1}{\sqrt{1 - x^2}}$, for $|x| < 1$
- $\frac{d}{dx}[\arctan x] = \frac{1}{1 + x^2}$
- The chain rule extends these: $\frac{d}{dx}[\arctan(g(x))] = \frac{g'(x)}{1 + [g(x)]^2}$

### 3.5 Selecting Procedures for Calculating Derivatives
- Before differentiating, look at the overall structure of the expression to decide which rules apply.
- Many expressions require combining multiple rules — power rule with chain rule, product rule with chain rule, and so on.
- Working through the structure from the outside in is usually the most reliable strategy.

### 3.6 Calculating Higher-Order Derivatives
- The second derivative $f''(x)$ is the derivative of $f'(x)$ — that is, differentiate twice.
- Notation: $f''(x)$, $\frac{d^2y}{dx^2}$, $y''$; for higher orders: $f^{(n)}(x)$, $\frac{d^n y}{dx^n}$
- In implicit differentiation, finding $\frac{d^2y}{dx^2}$ requires substituting the already-found $\frac{dy}{dx}$ expression back in.
- Physical interpretation: if $s(t)$ is position, $s'(t) = v(t)$ is velocity and $s''(t) = a(t)$ is acceleration.

---

## Key Formulas Summary

| Derivative | Formula |
|-----------|---------|
| Chain Rule | $\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$ |
| Inverse function | $(f^{-1})'(b) = \frac{1}{f'(f^{-1}(b))}$ |
| $\arcsin x$ | $\frac{1}{\sqrt{1-x^2}}$ |
| $\arccos x$ | $-\frac{1}{\sqrt{1-x^2}}$ |
| $\arctan x$ | $\frac{1}{1+x^2}$ |
| $\text{arccot } x$ | $-\frac{1}{1+x^2}$ |
| $\text{arcsec } x$ | $\frac{1}{|x|\sqrt{x^2-1}}$ |
| $\text{arccsc } x$ | $-\frac{1}{|x|\sqrt{x^2-1}}$ |

## Common Misconceptions
- Forgetting the "inner derivative" when applying the chain rule (e.g., writing $\frac{d}{dx}[\sin(3x)] = \cos(3x)$ instead of $3\cos(3x)$).
- In implicit differentiation, forgetting to apply the chain rule to $y$ terms.
- Confusing $\frac{d}{dx}[f^{-1}(x)]$ with $\frac{1}{f(x)}$ or $[f(x)]^{-1}$.
- Believing the second derivative is $(f')^2$ rather than the derivative of $f'$.
