# Topic 5: Calculus

> SL: 28 hours | HL: 55 hours

## SL Content

### 5.1 Limits and Derivatives (Introduction)
- Informal concept of a limit
- Derivative as the gradient of the tangent to a curve at a point
- Derivative from first principles: $f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$
- Derivative as rate of change

### 5.2 Differentiation Rules
- Power rule: $\frac{d}{dx}(x^n) = nx^{n-1}$
- Constant multiple rule and sum/difference rule
- Derivatives of standard functions:
  - $\frac{d}{dx}(\sin x) = \cos x$, $\frac{d}{dx}(\cos x) = -\sin x$
  - $\frac{d}{dx}(e^x) = e^x$, $\frac{d}{dx}(\ln x) = \frac{1}{x}$
  - $\frac{d}{dx}(\tan x) = \sec^2 x$

### 5.3 Chain Rule
- $\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$
- Applications to composite functions

### 5.4 Applications of Differentiation
- Tangent lines and normal lines
- **Increasing/decreasing functions**: $f'(x) > 0$ (increasing), $f'(x) < 0$ (decreasing)
- **Stationary points**: $f'(x) = 0$
  - Local maximum: $f'(x)$ changes from + to - (or $f''(x) < 0$)
  - Local minimum: $f'(x)$ changes from - to + (or $f''(x) > 0$)
  - Point of inflection (where applicable)
- Optimization problems (maximum/minimum in context)

### 5.5 Integration
- Integration as anti-differentiation (reverse of differentiation)
- $\int x^n dx = \frac{x^{n+1}}{n+1} + C$ (for $n \neq -1$)
- Standard integrals:
  - $\int \sin x \, dx = -\cos x + C$
  - $\int \cos x \, dx = \sin x + C$
  - $\int e^x dx = e^x + C$
  - $\int \frac{1}{x} dx = \ln|x| + C$

### 5.6 Definite Integrals and Areas
- $\int_a^b f(x)\,dx = F(b) - F(a)$
- Area between curve and $x$-axis (taking absolute values for areas below axis)
- Area between two curves: $\int_a^b [f(x) - g(x)]\,dx$

### 5.7 Kinematics
- Displacement: $s(t) = \int v(t)\,dt$
- Velocity: $v(t) = \frac{ds}{dt} = \int a(t)\,dt$
- Acceleration: $a(t) = \frac{dv}{dt}$
- Distance traveled: $\int_a^b |v(t)|\,dt$

## HL Extension

### 5.8 Product and Quotient Rules
- Product rule: $\frac{d}{dx}[f(x)g(x)] = f'(x)g(x) + f(x)g'(x)$
- Quotient rule: $\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}$

### 5.9 Related Rates and Implicit Differentiation
- **Implicit differentiation**: differentiating equations not explicitly solved for $y$
  - e.g., $x^2 + y^2 = r^2 \Rightarrow 2x + 2y\frac{dy}{dx} = 0$
- Related rates: applying chain rule to connected rates of change

### 5.10 Integration Techniques (HL)
- Integration by substitution ($u$-substitution)
- Integration by parts: $\int u\,dv = uv - \int v\,du$
- Partial fractions (with Topic 2 connection)

### 5.11 Differential Equations (HL)
- **Separable ODEs**: $\frac{dy}{dx} = f(x)g(y) \Rightarrow \int \frac{1}{g(y)}\,dy = \int f(x)\,dx$
- First-order linear ODEs with integrating factor
- Modeling with differential equations:
  - Exponential growth/decay: $\frac{dy}{dt} = ky$, solution $y = y_0 e^{kt}$
  - Logistic growth: $\frac{dy}{dt} = ky(1 - y/L)$

### 5.12 Maclaurin Series (HL)
- $f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3 + ...$
- Standard series:
  - $e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + ...$
  - $\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - ...$
  - $\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - ...$
  - $\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - ...$ (for $-1 < x \leq 1$)

### 5.13 Limits (HL)
- L'Hopital's rule: $\lim_{x \to a}\frac{f(x)}{g(x)} = \lim_{x \to a}\frac{f'(x)}{g'(x)}$ (when both → 0 or both → ∞)
- Evaluating indeterminate forms

## Key Equations

| Equation | Description |
|----------|-------------|
| $f'(x) = \lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$ | Derivative from first principles |
| $\frac{d}{dx}(x^n) = nx^{n-1}$ | Power rule |
| $\int_a^b f(x)dx = F(b) - F(a)$ | Fundamental theorem of calculus |
| $\int u\,dv = uv - \int v\,du$ | Integration by parts (HL) |
| $f(x) = \sum_{n=0}^{\infty}\frac{f^{(n)}(0)}{n!}x^n$ | Maclaurin series (HL) |

## Common Misconceptions

1. **"The derivative is the same as the slope of the secant"** -- The derivative is the slope of the tangent (instantaneous rate), not the secant (average rate).
2. **"Integration always gives area"** -- Definite integrals can give signed area; for total area, take absolute values of regions below the axis.
3. **"$\int \frac{1}{x}dx = \frac{x^0}{0}$"** -- The power rule does not apply when $n = -1$; the integral is $\ln|x| + C$.
4. **"If $f'(x) = 0$, there is always a maximum or minimum"** -- It could be a point of inflection (e.g., $f(x) = x^3$ at $x = 0$).
5. **"Maclaurin series converge everywhere"** -- Each series has a radius of convergence; $\ln(1+x)$ only converges for $-1 < x \leq 1$.

## Comparison with AP Mathematics

- IB AA SL calculus covers roughly the same content as AP Calculus AB
- IB AA HL extends with Maclaurin series, differential equations, and L'Hopital's rule
- AP Calculus BC covers Taylor/Maclaurin series in more depth (convergence tests, error bounds)
- IB HL covers differential equations more extensively than AP BC (especially modeling applications)
- AP Calculus uses the notation $\frac{d}{dx}$ and Leibniz notation; IB uses both $f'(x)$ and $\frac{dy}{dx}$
