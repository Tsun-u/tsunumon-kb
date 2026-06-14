# Unit 7: Differential Equations
> AB Exam Weight: 6–12% | BC Exam Weight: 6–9% | ~8–9 Class Periods

---

## Topics

### 7.1 Modeling Situations with Differential Equations
- A differential equation connects a quantity to its own rate of change — it tells a story about how something evolves rather than specifying a static relationship.
- For example, saying "a population grows at a rate proportional to its current size" translates directly into $\frac{dP}{dt} = kP$, where the population and its rate appear together in the same equation.

### 7.2 Verifying Solutions for Differential Equations
- To check whether a proposed function actually solves a differential equation, substitute it and its derivative(s) back in and confirm the equation holds identically.
- A **general solution** carries an arbitrary constant $C$, representing the whole family of solutions. A **particular solution** pins down $C$ by satisfying one additional initial condition.

### 7.3 Sketching Slope Fields
- A **slope field** draws a short segment at each lattice point $(x, y)$ with slope equal to $f(x, y)$, the right-hand side of $\frac{dy}{dx} = f(x, y)$.
- Stepping back from the field as a whole reveals how solution curves must behave — even without ever solving the equation algebraically.

### 7.4 Reasoning Using Slope Fields
- Solution curves flow along the slope field: at every point, they run parallel to the local segment.
- Wherever $f(x, y) = 0$, solution curves are flat — those are points of horizontal tangency.
- Straight horizontal bands of segments signal **equilibrium solutions**, where the population (or quantity) stabilizes at a constant level.
- Starting at an initial point and tracing the direction indicated by surrounding segments sketches the particular solution through that point.

### 7.5 Approximating Solutions Using Euler's Method (BC Only)
- When an exact formula is out of reach, Euler's method marches forward in small steps using the tangent line as a local guide:
  $$x_{n+1} = x_n + \Delta x, \qquad y_{n+1} = y_n + f(x_n, y_n) \cdot \Delta x$$
- Each step replaces the true curve with a short linear piece — smaller $\Delta x$ means more steps and less accumulated error.
- The approximation trends low when the solution curves upward (concave up) and trends high when the solution curves downward (concave down), because the tangent line consistently undercuts or overshoots the curve.

### 7.6 Finding General Solutions Using Separation of Variables
- A **separable** differential equation can be rearranged so all $y$ terms (with $dy$) sit on one side and all $x$ terms (with $dx$) sit on the other:
  $$g(y)\,dy = f(x)\,dx$$
- Integrate both sides independently, include $+ C$ on one side, and solve for $y$ when possible.
- Example: $\frac{dy}{dx} = xy \implies \frac{dy}{y} = x\,dx \implies \ln|y| = \frac{x^2}{2} + C$.

### 7.7 Finding Particular Solutions Using Initial Conditions and Separation of Variables
- Once the general solution is in hand, plug in the initial condition $(x_0, y_0)$ to find the specific value of $C$.
- Solve for $C$ before simplifying the rest of the expression — rushing algebraic steps can introduce domain errors or drop valid branches.
- The particular solution must remain continuous on an interval that contains the initial condition point.

### 7.8 Exponential Models with Differential Equations
- When growth or decay is proportional to the current amount, the governing equation is $\frac{dy}{dt} = ky$, whose solution is:
  $$y(t) = y_0 e^{kt}, \quad \text{where } y_0 = y(0)$$
- $k > 0$ gives exponential growth; $k < 0$ gives exponential decay.
- Two useful derived quantities:
  - **Half-life** (decay): $t_{1/2} = \dfrac{\ln 2}{|k|}$
  - **Doubling time** (growth): $t_d = \dfrac{\ln 2}{k}$
- Real-world appearances include population growth, radioactive decay, Newton's Law of Cooling, and continuously compounded interest.

### 7.9 Logistic Models with Differential Equations (BC Only)
- Real populations hit limits. The logistic model introduces a ceiling $L$ (carrying capacity) that brakes growth as the population approaches it:
  $$\frac{dP}{dt} = kP\!\left(1 - \frac{P}{L}\right)$$
- The exact solution takes the form:
  $$P(t) = \frac{L}{1 + Ae^{-kt}}, \quad A = \frac{L - P_0}{P_0}$$
- Key structural features:
  - $P = 0$ and $P = L$ are both equilibrium solutions (neither grows nor shrinks).
  - Growth is fastest when $P = \frac{L}{2}$ — the inflection point of the solution curve.
  - As $t \to \infty$, $P(t) \to L$ regardless of initial population.

---

## Key Formulas Summary

| Concept | Formula |
|---------|---------|
| Exponential growth/decay | $\frac{dy}{dt} = ky \implies y = y_0 e^{kt}$ |
| Half-life | $t_{1/2} = \frac{\ln 2}{\|k\|}$ |
| Euler's method (BC) | $y_{n+1} = y_n + f(x_n, y_n)\Delta x$ |
| Logistic equation (BC) | $\frac{dP}{dt} = kP(1 - \frac{P}{L})$ |
| Logistic solution (BC) | $P(t) = \frac{L}{1 + Ae^{-kt}}$ |

## Common Misconceptions
- Failing to move every $y$ term (including denominator factors) to the correct side before integrating — a single stray term invalidates separation.
- Dropping the constant of integration or losing it during algebra, which collapses a family of solutions into just one.
- Substituting the initial condition too late in the process, after algebraic simplification has already changed the domain.
- Treating the general solution and the particular solution as interchangeable — the constant $C$ is genuinely free until an initial condition pins it.
- In Euler's method, computing the slope using the updated point $(x_{n+1}, y_{n+1})$ rather than the current point $(x_n, y_n)$.
- In logistic growth, mixing up $L$ (the long-run limit) with $P_0$ (where the population starts).
- Believing that exponential decay eventually drives a quantity to exactly zero in finite time — it only approaches zero asymptotically.
