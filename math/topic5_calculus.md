# Topic 5: Calculus

> SL: 28 hours | HL: 55 hours

## SL Content

### 5.1 Limits and Derivatives (Introduction)
- A limit describes what value a function approaches as its input gets arbitrarily close to a target — the function need not actually reach that value
- The derivative at a point equals the slope of the tangent line drawn to the curve at that point
- Derivative from first principles — the formal definition via a limiting process: $f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$
- Interpreting the derivative as an instantaneous rate of change is just as important as calculating it

### 5.2 Differentiation Rules
- Power rule: $\frac{d}{dx}(x^n) = nx^{n-1}$
- Constant multiple rule and sum/difference rule allow differentiation term by term
- Derivatives of standard functions:
  - $\frac{d}{dx}(\sin x) = \cos x$, $\frac{d}{dx}(\cos x) = -\sin x$
  - $\frac{d}{dx}(e^x) = e^x$, $\frac{d}{dx}(\ln x) = \frac{1}{x}$
  - $\frac{d}{dx}(\tan x) = \sec^2 x$

### 5.3 Chain Rule
- $\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$
- Think of it as "derivative of the outside evaluated at the inside, times derivative of the inside" — essential for any composition of functions

### 5.4 Applications of Differentiation
- The tangent line at a point uses the derivative as its slope; the normal line is perpendicular, so its slope is the negative reciprocal
- **Increasing/decreasing functions**: $f'(x) > 0$ means the function is rising; $f'(x) < 0$ means it is falling
- **Stationary points** occur where $f'(x) = 0$; the second derivative or sign analysis reveals their nature:
  - Local maximum: $f'(x)$ changes from positive to negative (or $f''(x) < 0$)
  - Local minimum: $f'(x)$ changes from negative to positive (or $f''(x) > 0$)
  - Point of inflection: curvature changes sign without creating a turning point
- Optimisation problems ask you to find the maximum or minimum of some real-world quantity; set the derivative to zero and interpret the solution in context

### 5.5 Integration
- Integration reverses differentiation: if differentiating $F(x)$ gives $f(x)$, then $\int f(x)\,dx = F(x) + C$
- $\int x^n dx = \frac{x^{n+1}}{n+1} + C$ (for $n \neq -1$)
- Standard integrals to remember:
  - $\int \sin x \, dx = -\cos x + C$
  - $\int \cos x \, dx = \sin x + C$
  - $\int e^x dx = e^x + C$
  - $\int \frac{1}{x} dx = \ln|x| + C$

### 5.6 Definite Integrals and Areas
- The fundamental theorem links differentiation and integration: $\int_a^b f(x)\,dx = F(b) - F(a)$
- A definite integral computes signed area; regions below the $x$-axis contribute negatively, so finding total geometric area requires taking absolute values of each region separately
- Area between two curves: $\int_a^b [f(x) - g(x)]\,dx$ where $f$ is the upper curve over the interval

### 5.7 Kinematics
- Displacement: $s(t) = \int v(t)\,dt$
- Velocity: $v(t) = \frac{ds}{dt} = \int a(t)\,dt$
- Acceleration: $a(t) = \frac{dv}{dt}$
- Total distance traveled accounts for direction changes: $\int_a^b |v(t)|\,dt$

## HL Extension

### 5.8 Product and Quotient Rules
- Product rule: $\frac{d}{dx}[f(x)g(x)] = f'(x)g(x) + f(x)g'(x)$
- Quotient rule: $\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2}$

### 5.9 Related Rates and Implicit Differentiation
- **Implicit differentiation** handles equations where $y$ is not isolated — differentiate both sides with respect to $x$, treating $y$ as a function of $x$ and applying the chain rule wherever $y$ appears
  - e.g., $x^2 + y^2 = r^2 \Rightarrow 2x + 2y\frac{dy}{dx} = 0$
- Related rates problems connect two or more quantities that change together; write an equation relating them and differentiate with respect to time

### 5.10 Integration Techniques (HL)
- Integration by substitution ($u$-substitution) simplifies an integral by substituting a new variable to reduce it to a standard form
- Integration by parts: $\int u\,dv = uv - \int v\,du$ — trades one integral for (hopefully) a simpler one
- Partial fractions (from Topic 2) allow rational functions to be integrated term by term

### 5.11 Differential Equations (HL)
- **Separable ODEs**: when the equation can be written as $\frac{dy}{dx} = f(x)g(y)$, separate variables and integrate each side independently: $\int \frac{1}{g(y)}\,dy = \int f(x)\,dx$
- First-order linear ODEs are handled by finding an integrating factor that makes the left-hand side a perfect derivative
- Modelling with differential equations:
  - Exponential growth/decay: $\frac{dy}{dt} = ky$, solution $y = y_0 e^{kt}$
  - Logistic growth levels off as the population approaches carrying capacity $L$: $\frac{dy}{dt} = ky(1 - y/L)$

### 5.12 Maclaurin Series (HL)
- Any sufficiently smooth function can be approximated near $x = 0$ by an infinite polynomial whose coefficients come from the function's derivatives at that point: $f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3 + ...$
- Standard series:
  - $e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + ...$
  - $\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - ...$
  - $\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - ...$
  - $\ln(1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} - ...$ (for $-1 < x \leq 1$)

### 5.13 Limits (HL)
- L'Hôpital's rule resolves indeterminate forms: $\lim_{x \to a}\frac{f(x)}{g(x)} = \lim_{x \to a}\frac{f'(x)}{g'(x)}$ — but only when both $f$ and $g$ tend to 0 or both tend to $\infty$
- Recognising an indeterminate form before applying the rule is half the battle

## Key Equations

| Equation | Description |
|----------|-------------|
| $f'(x) = \lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$ | Derivative from first principles |
| $\frac{d}{dx}(x^n) = nx^{n-1}$ | Power rule |
| $\int_a^b f(x)dx = F(b) - F(a)$ | Fundamental theorem of calculus |
| $\int u\,dv = uv - \int v\,du$ | Integration by parts (HL) |
| $f(x) = \sum_{n=0}^{\infty}\frac{f^{(n)}(0)}{n!}x^n$ | Maclaurin series (HL) |

## Common Misconceptions

1. **"The derivative is the same as the slope of the secant"** -- The secant slope is an average rate of change between two points; the derivative is the instantaneous rate at a single point, obtained by letting those two points merge.
2. **"Integration always gives area"** -- A definite integral gives signed area; parts of the region below the $x$-axis are subtracted. To get the total geometric area, you must split the integral at each zero and add up absolute values.
3. **"$\int \frac{1}{x}dx = \frac{x^0}{0}$"** -- The power rule for integration breaks down at $n = -1$ because division by zero is undefined; that special case gives $\ln|x| + C$ instead.
4. **"If $f'(x) = 0$, there is always a maximum or minimum"** -- A zero derivative only guarantees a stationary point; it could be a point of inflection where the curve flattens momentarily without turning (for example, $f(x) = x^3$ at $x = 0$).
5. **"Maclaurin series converge everywhere"** -- Every power series has a radius of convergence; beyond it, the partial sums diverge rather than approaching the function value. For $\ln(1+x)$, this radius is 1.

## Comparison with AP Mathematics

- IB AA SL calculus and AP Calculus AB cover broadly the same ground: limits, differentiation rules, and introductory integration
- IB AA HL extends into Maclaurin series, differential equations, and L'Hôpital's rule, matching AP Calculus BC in scope but with different emphases
- AP Calculus BC treats Taylor and Maclaurin series more thoroughly, including convergence tests and error bound estimation
- Differential equations — particularly logistic growth and first-order linear ODEs — receive more sustained attention in IB HL than in AP BC
- Both curricula accept Leibniz notation ($\frac{dy}{dx}$) and prime notation ($f'(x)$); IB problems tend to use both interchangeably, so fluency in either form is expected
