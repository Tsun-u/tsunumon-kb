# Unit 2: Differentiation: Definition and Fundamental Properties
> AB Exam Weight: 10–12% | BC Exam Weight: 4–7% | ~13–14 Class Periods

---

## Topics

### 2.1 Defining Average and Instantaneous Rate of Change at a Point
- Average rate of change of $f$ on $[a, b]$: $\frac{f(b) - f(a)}{b - a}$
- Instantaneous rate of change at $x = a$: $\lim_{h \to 0} \frac{f(a + h) - f(a)}{h}$
- The instantaneous rate is what you get when you shrink the averaging interval all the way down to a single point.

### 2.2 Defining the Derivative of a Function and Using Derivative Notation
- The derivative at a point is defined by two equivalent limit forms:
  - $f'(a) = \lim_{h \to 0} \frac{f(a + h) - f(a)}{h}$
  - $f'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}$
- Geometrically, $f'(a)$ is the slope of the tangent line to the graph at the point $(a, f(a))$.
- **Tangent line equation** at $(a, f(a))$: $y - f(a) = f'(a)(x - a)$
- Common notations: $f'(x)$, $\frac{dy}{dx}$, $\frac{d}{dx}[f(x)]$, $y'$, $D_x[y]$

### 2.3 Estimating Derivatives of a Function at a Point
- When an exact formula isn't available, the derivative can be approximated from a table or a graph.
- From a table: the symmetric difference quotient $\frac{f(a + h) - f(a - h)}{2h}$ typically gives a better estimate than the one-sided version.
- From a graph: estimate the slope of the line tangent to the curve at the point in question.

### 2.4 Connecting Differentiability and Continuity
- Differentiability implies continuity: if $f$ is differentiable at $x = c$, it must be continuous there.
- The converse fails — a function can be continuous at a point but fail to be differentiable.
- A function is not differentiable wherever it has:
  - A corner or cusp (e.g., $f(x) = |x|$ at $x = 0$)
  - A vertical tangent
  - A discontinuity

### 2.5 Applying the Power Rule
- **Power Rule:** $\frac{d}{dx}[x^n] = nx^{n-1}$ for any real number $n$.
- This works for integer, fractional, and negative exponents — not just whole numbers.
- Example: $\frac{d}{dx}[\sqrt{x}] = \frac{d}{dx}[x^{1/2}] = \frac{1}{2}x^{-1/2}$

### 2.6 Derivative Rules: Constant, Sum, Difference, and Constant Multiple
- **Constant Rule:** $\frac{d}{dx}[c] = 0$
- **Constant Multiple Rule:** $\frac{d}{dx}[cf(x)] = c \cdot f'(x)$
- **Sum Rule:** $\frac{d}{dx}[f(x) + g(x)] = f'(x) + g'(x)$
- **Difference Rule:** $\frac{d}{dx}[f(x) - g(x)] = f'(x) - g'(x)$

### 2.7 Derivatives of $\cos x$, $\sin x$, $e^x$, and $\ln x$
- $\frac{d}{dx}[\sin x] = \cos x$
- $\frac{d}{dx}[\cos x] = -\sin x$
- $\frac{d}{dx}[e^x] = e^x$
- $\frac{d}{dx}[\ln x] = \frac{1}{x}$ (for $x > 0$)

### 2.8 The Product Rule
- When differentiating the product of two functions, neither factor can be ignored:
  - **Product Rule:** $\frac{d}{dx}[f(x) \cdot g(x)] = f'(x) \cdot g(x) + f(x) \cdot g'(x)$
- A common mistake is treating the derivative of a product like the product of the derivatives — that's wrong.

### 2.9 The Quotient Rule
- **Quotient Rule:** $\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{[g(x)]^2}$
- Mnemonic: "Low d-high minus high d-low, over the square of what's below."
- Watch the order of subtraction in the numerator — it matters, and it's easy to flip.

### 2.10 Finding the Derivatives of Tangent, Cotangent, Secant, and Cosecant Functions
- These all follow from applying the quotient rule to $\sin x$ and $\cos x$:
  - $\frac{d}{dx}[\tan x] = \sec^2 x$
  - $\frac{d}{dx}[\cot x] = -\csc^2 x$
  - $\frac{d}{dx}[\sec x] = \sec x \tan x$
  - $\frac{d}{dx}[\csc x] = -\csc x \cot x$

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
