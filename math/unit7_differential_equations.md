# Unit 7: Differential Equations
> AB Exam Weight: 6–12% | BC Exam Weight: 6–9% | ~8–9 Class Periods

## Big Ideas: FUN, CHA

---

## Topics

### 7.1 Modeling Situations with Differential Equations
- **Learning Objective (FUN-7.A):** Write differential equations to describe situations.
- **Essential Knowledge:**
  - A differential equation is an equation involving a derivative: e.g., $\frac{dy}{dx} = f(x, y)$.
  - Differential equations model relationships between a quantity and its rate of change.
  - Example: "The rate of change of a population is proportional to the population" $\Rightarrow$ $\frac{dP}{dt} = kP$.

### 7.2 Verifying Solutions for Differential Equations
- **Learning Objective (FUN-7.B):** Verify solutions to differential equations.
- **Essential Knowledge:**
  - To verify, substitute the proposed solution into the differential equation and check that it satisfies the equation.
  - A general solution contains an arbitrary constant $C$; a particular solution satisfies an initial condition.

### 7.3 Sketching Slope Fields
- **Learning Objective (FUN-7.C):** Create slope fields.
- **Essential Knowledge:**
  - A **slope field** is a graphical representation of a differential equation $\frac{dy}{dx} = f(x, y)$.
  - At each point $(x, y)$, draw a short line segment with slope $f(x, y)$.
  - Slope fields show the general behavior of solutions without solving the equation.

### 7.4 Reasoning Using Slope Fields
- **Learning Objective (FUN-7.C):** Interpret slope fields.
- **Essential Knowledge:**
  - Solution curves follow the direction indicated by the slope field.
  - Where $f(x, y) = 0$, solution curves have horizontal tangents.
  - Patterns in slope fields can indicate equilibrium solutions, stability, and general behavior.
  - A particular solution curve can be sketched by starting at an initial point and following the slope field.

### 7.5 Approximating Solutions Using Euler's Method (BC Only)
- **Learning Objective (FUN-7.D):** Use Euler's method to approximate solutions.
- **Essential Knowledge:**
  - **Euler's Method:** Given $\frac{dy}{dx} = f(x, y)$, initial point $(x_0, y_0)$, and step size $\Delta x$:
    $$x_{n+1} = x_n + \Delta x$$
    $$y_{n+1} = y_n + f(x_n, y_n) \cdot \Delta x$$
  - This is a numerical approximation — smaller step sizes generally yield better accuracy.
  - Euler's method uses the tangent line to step forward incrementally.
  - If the solution is concave up, Euler's method underestimates; if concave down, it overestimates.

### 7.6 Finding General Solutions Using Separation of Variables
- **Learning Objective (FUN-7.E):** Solve separable differential equations.
- **Essential Knowledge:**
  - A **separable differential equation** can be written as $g(y)\,dy = f(x)\,dx$.
  - Strategy:
    1. Separate variables: all $y$ terms (and $dy$) on one side, all $x$ terms (and $dx$) on the other.
    2. Integrate both sides.
    3. Solve for $y$ if possible (include $+C$).
  - Example: $\frac{dy}{dx} = xy \implies \frac{dy}{y} = x\,dx \implies \ln|y| = \frac{x^2}{2} + C$

### 7.7 Finding Particular Solutions Using Initial Conditions and Separation of Variables
- **Learning Objective (FUN-7.E):** Find particular solutions using initial conditions.
- **Essential Knowledge:**
  - After finding the general solution, substitute the initial condition $(x_0, y_0)$ to solve for $C$.
  - Important: Solve for $C$ before simplifying the expression for $y$ (to avoid domain errors).
  - Domain of the particular solution must contain the initial condition and be continuous.

### 7.8 Exponential Models with Differential Equations
- **Learning Objective (FUN-7.F):** Solve exponential growth/decay problems.
- **Essential Knowledge:**
  - **Exponential growth/decay:** $\frac{dy}{dt} = ky$, where $k$ is a constant.
  - **Solution:** $y(t) = y_0 e^{kt}$, where $y_0 = y(0)$.
  - $k > 0$: exponential growth.
  - $k < 0$: exponential decay.
  - **Half-life:** $t_{1/2} = \frac{\ln 2}{|k|}$ (for decay).
  - **Doubling time:** $t_d = \frac{\ln 2}{k}$ (for growth).
  - Applications: population growth, radioactive decay, Newton's Law of Cooling, continuously compounded interest.

### 7.9 Logistic Models with Differential Equations (BC Only)
- **Learning Objective (FUN-7.G):** Solve logistic differential equations.
- **Essential Knowledge:**
  - **Logistic differential equation:** $\frac{dP}{dt} = kP\left(1 - \frac{P}{L}\right)$
    where $L$ is the carrying capacity and $k$ is the growth rate constant.
  - **Solution:** $P(t) = \frac{L}{1 + Ae^{-kt}}$ where $A = \frac{L - P_0}{P_0}$
  - Key features:
    - $P = 0$ and $P = L$ are equilibrium solutions.
    - Maximum growth rate occurs at $P = \frac{L}{2}$.
    - Inflection point (in the solution curve) occurs when $P = \frac{L}{2}$.
    - As $t \to \infty$, $P(t) \to L$.

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
- Forgetting to separate ALL $y$ terms to one side (including factors in the denominator).
- Not including the constant of integration or losing it during algebraic manipulation.
- Applying the initial condition at the wrong step.
- Confusing the general solution (with $C$) and particular solution (specific $C$).
- In Euler's method, using the wrong point to calculate the slope for the next step.
- In logistic growth, confusing the carrying capacity $L$ with the initial population $P_0$.
- Thinking exponential decay means the quantity becomes zero in finite time.
