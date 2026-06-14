# IB Math AI — Topic 2: Functions

> SL: 31 hours | HL: 42 hours

## SL Content

### SL 2.1 Straight Lines
- Equations of a line: $y = mx + c$, $ax + by + d = 0$, $y - y_1 = m(x - x_1)$
- Gradient and intercepts
- Parallel lines share the same gradient: $m_1 = m_2$; perpendicular lines satisfy $m_1 \cdot m_2 = -1$

### SL 2.2 Function Concepts
- A function maps each input in its domain to exactly one output in its range
- Notation $f(x)$; the inverse as a mapping that "undoes" the original
- Graph of $f^{-1}(x)$ as a reflection of $f(x)$ across the line $y = x$

### SL 2.3 Graphing Functions
- Producing graphs of $y = f(x)$ from information, context, or a rule
- Using technology to graph and explore functions, including sums and differences

### SL 2.4 Key Features of Graphs
- Identifying local maxima and minima; $x$- and $y$-intercepts; axes of symmetry; vertex; zeros
- Vertical and horizontal asymptotes
- Finding intersection points of two graphs using technology

### SL 2.5 Modelling with Functions
- **Linear models**: $f(x) = mx + c$
- **Quadratic models**: $f(x) = ax^2 + bx + c$; axis of symmetry, vertex, zeros, intercepts
- **Exponential growth and decay**: $f(x) = ka^x + c$, $f(x) = ke^{rx} + c$; horizontal asymptote
- **Direct and inverse variation**: $f(x) = ax^n$, $n \in \mathbb{Z}$
- **Cubic models**: $f(x) = ax^3 + bx^2 + cx + d$
- **Sinusoidal models**: $f(x) = a\sin(bx) + d$, $f(x) = a\cos(bx) + d$; amplitude, period $\frac{360°}{b}$

### SL 2.6 Modelling Skills
- The modelling cycle: identify a real-world problem → build a mathematical model → test and reflect → apply
- Choosing a model family based on context; fitting parameters to data
- Recognizing where a model is valid and where it breaks down

## HL Extension

### AHL 2.7 Composite and Inverse Functions
- Composite functions: $(f \circ g)(x) = f(g(x))$
- Inverse functions $f^{-1}$, including restricting the domain to ensure the function is invertible

### AHL 2.8 Transformations of Graphs
- Vertical translation $y = f(x) + b$, horizontal translation $y = f(x - a)$
- Reflections in both axes; vertical stretch $y = pf(x)$; horizontal stretch $y = f(qx)$
- Combining multiple transformations

### AHL 2.9 Further Modelling
- **Natural logarithm models**: $f(x) = a\ln x + b$ and natural exponential variations
- **Logistic models**: $f(x) = \frac{L}{1 + Ce^{-kx}}$, $L, C, k > 0$; carrying capacity $L$ is the upper horizontal asymptote — useful when growth is bounded
- **Piecewise models**: different rules apply over different parts of the domain

### AHL 2.10 Scaling and Linearization
- Using logarithms to handle very large or very small quantities
- **Log-log graphs**: power models $y = ax^n$ linearize as $\log y = \log a + n\log x$
- **Semi-log graphs**: exponential models $y = ka^x$ linearize as $\log y = \log k + x\log a$
- Reading gradient and intercept from the linearized graph to estimate parameters

## Key Equations

| Equation | Description |
|----------|-------------|
| $m_1 m_2 = -1$ | Perpendicular gradients |
| $f(x) = ka^x + c$ | Exponential model |
| $f(x) = a\sin(bx) + d$ | Sinusoidal model (period $360°/b$) |
| $f(x) = \frac{L}{1+Ce^{-kx}}$ | Logistic model (HL) |
| $\log y = \log a + n \log x$ | Log-log linearization of $y = ax^n$ (HL) |

## Common Misconceptions

1. **Period of a sinusoidal function** — The period of $a\sin(bx)+d$ is $\frac{360°}{b}$ (or $\frac{2\pi}{b}$ radians), not $b$ itself.
2. **Exponential functions can decrease** — With $0 < a < 1$ or $r < 0$, the model decays rather than grows.
3. **Logistic growth has a ceiling** — The function approaches the carrying capacity $L$ and does not grow indefinitely.
4. **Not every curve is exponential** — Power models ($y = ax^n$) also produce curves. Distinguish them: power models linearize on log-log axes, exponential on semi-log axes.

## Comparison with Other Courses

- The modelling-first approach is central to AI; AA Topic 2 emphasizes algebraic structure (rational functions, factor and remainder theorem at HL)
- Logistic models appear in AI HL and AP Calculus BC (Unit 7) — in BC they arise from differential equations, whereas in AI they are treated as a function family to fit to data
- Log-log and semi-log linearization are features unique to AI among these courses
