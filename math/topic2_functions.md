# Topic 2: Functions

> SL: 21 hours | HL: 32 hours

## SL Content

### 2.1 Function Concepts
- **Function**: a relation where each input has exactly one output
- Domain and range
- Function notation: $f(x)$, $f: x \mapsto ...$
- Vertical line test for functions

### 2.2 Graphs of Functions
- Sketching and interpreting graphs
- Key features: intercepts, asymptotes, maxima/minima, symmetry
- Using technology (GDC) to graph and analyze functions

### 2.3 Transformations
- Translations: $f(x - h) + k$ shifts right $h$, up $k$
- Reflections: $-f(x)$ reflects in $x$-axis; $f(-x)$ reflects in $y$-axis
- Stretches: $af(x)$ vertical stretch by factor $a$; $f(bx)$ horizontal stretch by factor $1/b$
- Composite transformations

### 2.4 Composite and Inverse Functions
- **Composite function**: $(f \circ g)(x) = f(g(x))$
- **Inverse function**: $f^{-1}(x)$; found by swapping $x$ and $y$ and solving
  - $f(f^{-1}(x)) = x$
  - Graph of $f^{-1}$ is reflection of $f$ in line $y = x$
  - Domain of $f^{-1}$ = range of $f$

### 2.5 Quadratic Functions
- $f(x) = ax^2 + bx + c$ (standard form)
- $f(x) = a(x - h)^2 + k$ (vertex form): vertex at $(h, k)$
- $f(x) = a(x - p)(x - q)$ (factored form): roots at $p$ and $q$
- **Discriminant**: $\Delta = b^2 - 4ac$
  - $\Delta > 0$: two distinct real roots
  - $\Delta = 0$: one repeated root
  - $\Delta < 0$: no real roots (two complex roots at HL)
- **Quadratic formula**: $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
- Axis of symmetry: $x = -b/(2a)$

### 2.6 Exponential and Logarithmic Functions
- $f(x) = a^x$ and $f(x) = e^x$: exponential growth/decay
- $f(x) = \log_a x$ and $f(x) = \ln x$: inverse of exponential
- Solving equations involving exponentials and logarithms
- Modeling with exponential functions (population, decay, compound interest)

## HL Extension

### 2.7 Rational Functions
- $f(x) = \frac{p(x)}{q(x)}$ where $p, q$ are polynomials
- Vertical asymptotes: where $q(x) = 0$ (and $p(x) \neq 0$)
- Horizontal asymptotes: determined by degrees of $p$ and $q$
- Oblique asymptotes (when degree of $p$ = degree of $q$ + 1)

### 2.8 Odd and Even Functions
- Even: $f(-x) = f(x)$ (symmetric about $y$-axis)
- Odd: $f(-x) = -f(x)$ (rotational symmetry about origin)

### 2.9 Factor and Remainder Theorems
- Factor theorem: $(x - a)$ is a factor of $p(x)$ iff $p(a) = 0$
- Remainder theorem: when $p(x)$ is divided by $(x-a)$, remainder = $p(a)$
- Polynomial division and finding roots

### 2.10 Partial Fractions
- Decomposing rational expressions into simpler fractions
- Used in integration (Topic 5)

### 2.11 Self-Inverse Functions
- $f(f(x)) = x$; function is its own inverse
- Example: $f(x) = \frac{1}{x}$

## Key Equations

| Equation | Description |
|----------|-------------|
| $x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$ | Quadratic formula |
| $\Delta = b^2 - 4ac$ | Discriminant |
| $(f \circ g)(x) = f(g(x))$ | Composite function |

## Common Misconceptions

1. **"All functions have inverses"** -- Only one-to-one (injective) functions have inverses; otherwise the domain must be restricted.
2. **"$f^{-1}(x) = 1/f(x)$"** -- $f^{-1}$ is the inverse function, not the reciprocal.
3. **"Asymptotes are never crossed"** -- Horizontal asymptotes can be crossed; vertical asymptotes cannot.
4. **"The discriminant tells you the roots"** -- It tells you the nature of the roots (real/complex, distinct/repeated), not their values.

## Comparison with AP Mathematics

- AP Pre-Calculus covers function concepts, transformations, and compositions similarly
- IB HL includes partial fractions and factor/remainder theorems; AP Calculus BC uses partial fractions in integration
- IB AA emphasizes function properties (odd/even, self-inverse) more explicitly
