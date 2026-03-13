# Unit 2: Differentiation: Definition and Fundamental Properties
> AB Exam Weight: 10–12% | BC Exam Weight: 4–7% | ~13–14 Class Periods

## Big Ideas: CHA, LIM, FUN

---

## Topics

### 2.1 Defining Average and Instantaneous Rate of Change at a Point
- **Learning Objective (CHA-1.A):** Interpret the rate of change at an instant in terms of average rates of change over intervals containing that instant.
- **Essential Knowledge:**
  - Average rate of change of $f$ on $[a, b]$: $\frac{f(b) - f(a)}{b - a}$
  - Instantaneous rate of change at $x = a$: $\lim_{h \to 0} \frac{f(a + h) - f(a)}{h}$
  - The instantaneous rate of change is the limit of average rates of change as the interval shrinks to zero.

### 2.2 Defining the Derivative of a Function and Using Derivative Notation
- **Learning Objective (CHA-2.A):** Define the derivative of a function at a point.
- **Essential Knowledge:**
  - **Limit definition of derivative:**
    - $f'(a) = \lim_{h \to 0} \frac{f(a + h) - f(a)}{h}$
    - $f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$
  - The derivative at a point is the slope of the tangent line at that point.
  - **Tangent line equation** at $(a, f(a))$: $y - f(a) = f'(a)(x - a)$
  - Notation: $f'(x)$, $\frac{dy}{dx}$, $\frac{d}{dx}[f(x)]$, $y'$, $D_x[y]$

### 2.3 Estimating Derivatives of a Function at a Point
- **Learning Objective (CHA-2.B):** Estimate derivatives.
- **Essential Knowledge:**
  - The derivative can be estimated from tables, graphs, or technology.
  - Using a table: approximate $f'(a) \approx \frac{f(a + h) - f(a - h)}{2h}$ (symmetric difference quotient).
  - From a graph: estimate the slope of the tangent line.

### 2.4 Connecting Differentiability and Continuity
- **Learning Objective (FUN-2.A):** Determine whether a function is continuous and/or differentiable at a point.
- **Essential Knowledge:**
  - **If $f$ is differentiable at $x = c$, then $f$ is continuous at $x = c$.**
  - The converse is NOT true: continuity does not imply differentiability.
  - A function is NOT differentiable where it has:
    - A corner or cusp (e.g., $f(x) = |x|$ at $x = 0$)
    - A vertical tangent
    - A discontinuity
  - Common misconception: Continuous functions are always differentiable. (Counterexample: $|x|$ at $x = 0$.)

### 2.5 Applying the Power Rule
- **Learning Objective (FUN-3.A):** Calculate derivatives of elementary functions.
- **Essential Knowledge:**
  - **Power Rule:** $\frac{d}{dx}[x^n] = nx^{n-1}$ for any real number $n$.
  - Works for integer, fractional, and negative exponents.
  - Example: $\frac{d}{dx}[\sqrt{x}] = \frac{d}{dx}[x^{1/2}] = \frac{1}{2}x^{-1/2}$

### 2.6 Derivative Rules: Constant, Sum, Difference, and Constant Multiple
- **Learning Objective (FUN-3.A):** Calculate derivatives of elementary functions.
- **Essential Knowledge:**
  - **Constant Rule:** $\frac{d}{dx}[c] = 0$
  - **Constant Multiple Rule:** $\frac{d}{dx}[cf(x)] = c \cdot f'(x)$
  - **Sum Rule:** $\frac{d}{dx}[f(x) + g(x)] = f'(x) + g'(x)$
  - **Difference Rule:** $\frac{d}{dx}[f(x) - g(x)] = f'(x) - g'(x)$

### 2.7 Derivatives of $\cos x$, $\sin x$, $e^x$, and $\ln x$
- **Learning Objective (FUN-3.A):** Calculate derivatives of elementary functions.
- **Essential Knowledge:**
  - $\frac{d}{dx}[\sin x] = \cos x$
  - $\frac{d}{dx}[\cos x] = -\sin x$
  - $\frac{d}{dx}[e^x] = e^x$
  - $\frac{d}{dx}[\ln x] = \frac{1}{x}$ (for $x > 0$)

### 2.8 The Product Rule
- **Learning Objective (FUN-3.B):** Calculate derivatives of products and quotients.
- **Essential Knowledge:**
  - **Product Rule:** $\frac{d}{dx}[f(x) \cdot g(x)] = f'(x) \cdot g(x) + f(x) \cdot g'(x)$
  - Common misconception: The derivative of a product is the product of the derivatives.

### 2.9 The Quotient Rule
- **Learning Objective (FUN-3.B):** Calculate derivatives of products and quotients.
- **Essential Knowledge:**
  - **Quotient Rule:** $\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{[g(x)]^2}$
  - Mnemonic: "Low d-high minus high d-low, over the square of what's below."
  - Common misconception: Forgetting to square the denominator, or confusing the order of subtraction.

### 2.10 Finding the Derivatives of Tangent, Cotangent, Secant, and Cosecant Functions
- **Learning Objective (FUN-3.A):** Calculate derivatives of elementary functions.
- **Essential Knowledge:**
  - $\frac{d}{dx}[\tan x] = \sec^2 x$
  - $\frac{d}{dx}[\cot x] = -\csc^2 x$
  - $\frac{d}{dx}[\sec x] = \sec x \tan x$
  - $\frac{d}{dx}[\csc x] = -\csc x \cot x$
  - These can be derived using the quotient rule applied to $\sin x$ and $\cos x$.

---

## Key Formulas Summary

| Function $f(x)$ | Derivative $f'(x)$ |
|-----------------|-------------------|
| $c$ (constant) | $0$ |
| $x^n$ | $nx^{n-1}$ |
| $\sin x$ | $\cos x$ |
| $\cos x$ | $-\sin x$ |
| $\tan x$ | $\sec^2 x$ |
| $\cot x$ | $-\csc^2 x$ |
| $\sec x$ | $\sec x \tan x$ |
| $\csc x$ | $-\csc x \cot x$ |
| $e^x$ | $e^x$ |
| $\ln x$ | $\frac{1}{x}$ |
| $a^x$ | $a^x \ln a$ |
| $\log_a x$ | $\frac{1}{x \ln a}$ |

## Common Misconceptions
- Believing continuity implies differentiability.
- Applying the power rule incorrectly to exponential functions (e.g., treating $2^x$ like $x^2$).
- Multiplying derivatives instead of using the product rule: $[f \cdot g]' \neq f' \cdot g'$.
- Forgetting the negative sign in $\frac{d}{dx}[\cos x] = -\sin x$.
- Confusing $\frac{d}{dx}[e^x] = e^x$ with $\frac{d}{dx}[x^e] = ex^{e-1}$.
