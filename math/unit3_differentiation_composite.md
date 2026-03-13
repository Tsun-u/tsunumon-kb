# Unit 3: Differentiation: Composite, Implicit, and Inverse Functions
> AB Exam Weight: 9–13% | BC Exam Weight: 4–7% | ~10–11 Class Periods

## Big Ideas: FUN

---

## Topics

### 3.1 The Chain Rule
- **Learning Objective (FUN-3.C):** Calculate derivatives of compositions of differentiable functions.
- **Essential Knowledge:**
  - **Chain Rule:** If $y = f(g(x))$, then $\frac{dy}{dx} = f'(g(x)) \cdot g'(x)$
  - Leibniz notation: If $y = f(u)$ and $u = g(x)$, then $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$
  - Extends to multiple compositions: $\frac{d}{dx}[f(g(h(x)))] = f'(g(h(x))) \cdot g'(h(x)) \cdot h'(x)$
  - Key applications:
    - $\frac{d}{dx}[e^{g(x)}] = e^{g(x)} \cdot g'(x)$
    - $\frac{d}{dx}[\ln(g(x))] = \frac{g'(x)}{g(x)}$
    - $\frac{d}{dx}[\sin(g(x))] = \cos(g(x)) \cdot g'(x)$
    - $\frac{d}{dx}[[g(x)]^n] = n[g(x)]^{n-1} \cdot g'(x)$

### 3.2 Implicit Differentiation
- **Learning Objective (FUN-3.D):** Calculate derivatives of implicitly defined functions.
- **Essential Knowledge:**
  - Used when $y$ is not isolated as a function of $x$ (e.g., $x^2 + y^2 = 25$).
  - Differentiate both sides with respect to $x$, applying the chain rule to terms involving $y$ (multiply by $\frac{dy}{dx}$).
  - Solve the resulting equation for $\frac{dy}{dx}$.
  - The result may contain both $x$ and $y$.
  - Example: $x^2 + y^2 = 25 \implies 2x + 2y\frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{x}{y}$

### 3.3 Differentiating Inverse Functions
- **Learning Objective (FUN-3.E):** Calculate derivatives of inverse functions.
- **Essential Knowledge:**
  - If $g$ is the inverse of $f$, then $g'(x) = \frac{1}{f'(g(x))}$, provided $f'(g(x)) \neq 0$.
  - Equivalently: if $f(a) = b$, then $(f^{-1})'(b) = \frac{1}{f'(a)}$
  - The graphs of $f$ and $f^{-1}$ are reflections over $y = x$.
  - Common misconception: $\frac{d}{dx}[f^{-1}(x)] = \frac{1}{f'(x)}$. (Correct: it is $\frac{1}{f'(f^{-1}(x))}$.)

### 3.4 Differentiating Inverse Trigonometric Functions
- **Learning Objective (FUN-3.E):** Calculate derivatives of inverse trigonometric functions.
- **Essential Knowledge:**
  - $\frac{d}{dx}[\arcsin x] = \frac{1}{\sqrt{1 - x^2}}$, for $|x| < 1$
  - $\frac{d}{dx}[\arccos x] = -\frac{1}{\sqrt{1 - x^2}}$, for $|x| < 1$
  - $\frac{d}{dx}[\arctan x] = \frac{1}{1 + x^2}$
  - With chain rule: $\frac{d}{dx}[\arctan(g(x))] = \frac{g'(x)}{1 + [g(x)]^2}$

### 3.5 Selecting Procedures for Calculating Derivatives
- **Learning Objective (FUN-3.F):** Select appropriate derivative rules and techniques.
- **Essential Knowledge:**
  - Students must identify which rule(s) to apply: power rule, product rule, quotient rule, chain rule, implicit differentiation, or inverse function derivatives.
  - Multiple rules may be needed in combination (e.g., product rule + chain rule).
  - Strategy: analyze the structure of the expression before differentiating.

### 3.6 Calculating Higher-Order Derivatives
- **Learning Objective (FUN-3.F):** Calculate higher-order derivatives.
- **Essential Knowledge:**
  - The second derivative $f''(x)$ is the derivative of $f'(x)$.
  - Notation: $f''(x)$, $\frac{d^2y}{dx^2}$, $y''$
  - Higher orders: $f'''(x)$, $f^{(4)}(x)$, $\frac{d^n y}{dx^n}$
  - For implicit differentiation, the second derivative may involve substituting the expression for $\frac{dy}{dx}$.
  - Physical interpretation: if $s(t)$ is position, then $s'(t) = v(t)$ (velocity) and $s''(t) = a(t)$ (acceleration).

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
- Forgetting the "inner derivative" when applying the chain rule (e.g., $\frac{d}{dx}[\sin(3x)] = \cos(3x)$ instead of $3\cos(3x)$).
- In implicit differentiation, forgetting to apply the chain rule to $y$ terms.
- Confusing $\frac{d}{dx}[f^{-1}(x)]$ with $\frac{1}{f(x)}$ or $[f(x)]^{-1}$.
- Believing the second derivative is $(f')^2$ rather than the derivative of $f'$.
