# Topic 2: Functions

> SL: 21 hours | HL: 32 hours

## SL Content

### 2.1 Function Concepts
- **Function**: a mapping between two sets where every input value is paired with exactly one output value — no splitting allowed
- Domain refers to the set of permitted inputs; range refers to the set of actual outputs produced
- Function notation: $f(x)$ means "apply rule $f$ to input $x$"; the arrow notation $f: x \mapsto ...$ makes the mapping explicit
- The vertical line test determines whether a graph represents a function: if any vertical line crosses the graph more than once, it is not a function

### 2.2 Graphs of Functions
- Sketching graphs by hand and reading off their features is a core skill, supplemented by technology for accuracy
- Key features to identify: $x$- and $y$-intercepts, asymptotes, turning points, and any symmetry
- A graphing calculator (GDC) helps verify sketches and locate roots or intersections numerically

### 2.3 Transformations
- Translations: $f(x - h) + k$ moves the graph $h$ units right and $k$ units up
- Reflections: $-f(x)$ flips the graph over the $x$-axis; $f(-x)$ flips it over the $y$-axis
- Stretches: $af(x)$ scales vertically by factor $a$; $f(bx)$ compresses horizontally by factor $b$ (or stretches by $1/b$)
- Multiple transformations can be chained together; order matters when combining stretches with translations

### 2.4 Composite and Inverse Functions
- **Composite function**: apply $g$ first, then feed the result into $f$: $(f \circ g)(x) = f(g(x))$
- **Inverse function**: $f^{-1}(x)$ undoes what $f$ does; find it by swapping $x$ and $y$ and solving for $y$
  - $f(f^{-1}(x)) = x$
  - The graph of $f^{-1}$ is the mirror image of the graph of $f$ across the line $y = x$
  - The domain of $f^{-1}$ equals the range of $f$, and vice versa

### 2.5 Quadratic Functions
- $f(x) = ax^2 + bx + c$ (standard form): useful for reading off the $y$-intercept directly
- $f(x) = a(x - h)^2 + k$ (vertex form): vertex sits at $(h, k)$, making transformations transparent
- $f(x) = a(x - p)(x - q)$ (factored form): roots are immediately visible at $x = p$ and $x = q$
- **Discriminant**: $\Delta = b^2 - 4ac$ tells you what kind of roots to expect before solving
  - $\Delta > 0$: two distinct real roots
  - $\Delta = 0$: one repeated real root (the vertex touches the axis)
  - $\Delta < 0$: no real roots (two complex conjugate roots at HL)
- **Quadratic formula**: $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
- Axis of symmetry passes through the vertex: $x = -b/(2a)$

### 2.6 Exponential and Logarithmic Functions
- $f(x) = a^x$ and $f(x) = e^x$ model situations where a quantity grows or decays at a rate proportional to its current size
- $f(x) = \log_a x$ and $f(x) = \ln x$ are the inverses of the exponential functions, reflecting their graphs in $y = x$
- Equations mixing exponentials and logarithms can be solved by isolating the exponential part and then taking a logarithm
- Real-world applications include population dynamics, radioactive decay, and compound interest calculations

## HL Extension

### 2.7 Rational Functions
- $f(x) = \frac{p(x)}{q(x)}$ where $p, q$ are polynomials; the behavior is dominated by the denominator near its zeros
- Vertical asymptotes appear where $q(x) = 0$ (provided $p(x) \neq 0$ at the same point)
- Horizontal asymptotes are determined by comparing the degrees of $p$ and $q$ as $x \to \pm\infty$
- An oblique (slant) asymptote occurs when the degree of $p$ exceeds the degree of $q$ by exactly one; polynomial long division reveals it

### 2.8 Odd and Even Functions
- Even functions satisfy $f(-x) = f(x)$ for all $x$ — their graphs are symmetric about the $y$-axis
- Odd functions satisfy $f(-x) = -f(x)$ — their graphs have 180° rotational symmetry about the origin

### 2.9 Factor and Remainder Theorems
- Factor theorem: $(x - a)$ divides $p(x)$ exactly when $p(a) = 0$ — a quick root-testing tool
- Remainder theorem: dividing $p(x)$ by $(x - a)$ leaves a remainder equal to $p(a)$, skipping full long division
- Polynomial long division (or synthetic division) breaks a polynomial into quotient and remainder, helping to find all roots

### 2.10 Partial Fractions
- A rational expression with a factorable denominator can be split into a sum of simpler fractions
- This technique makes integration of rational functions tractable (revisited in Topic 5)

### 2.11 Self-Inverse Functions
- A function is its own inverse when $f(f(x)) = x$ for all $x$ in its domain
- A clean example: $f(x) = \frac{1}{x}$ — applying it twice returns you to where you started

## Key Equations

| Equation | Description |
|----------|-------------|
| $x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$ | Quadratic formula |
| $\Delta = b^2 - 4ac$ | Discriminant |
| $(f \circ g)(x) = f(g(x))$ | Composite function |

## Common Misconceptions

1. **"All functions have inverses"** -- Only one-to-one (injective) functions have valid inverses; when a function repeats output values, the inverse would be ambiguous unless the domain is first restricted.
2. **"$f^{-1}(x) = 1/f(x)$"** -- The superscript $-1$ on a function name denotes the inverse function, not the reciprocal; $1/f(x)$ is written as $[f(x)]^{-1}$.
3. **"Asymptotes are lines the graph never touches"** -- Vertical asymptotes truly cannot be crossed, but horizontal asymptotes describe long-run behavior and can be crossed at finite $x$ values.
4. **"The discriminant tells you the actual roots"** -- The discriminant only reveals the nature of the roots (real vs. complex, repeated vs. distinct); you still need the quadratic formula to find the root values themselves.

## Comparison with AP Mathematics

- Function concepts, transformations, and composition appear in both IB AA and AP Pre-Calculus with broadly similar coverage
- The factor and remainder theorems and partial fractions are present in IB HL; AP Calculus BC uses partial fractions specifically for integration but does not emphasize the theorems as standalone proof tools
- Odd and even function symmetry and self-inverse functions receive more explicit treatment in IB AA than in typical AP courses
