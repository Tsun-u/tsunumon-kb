# IB Math AI — Topic 5: Calculus

> SL: 19 hours | HL: 41 hours

## SL Content

### SL 5.1 Limits and the Derivative Concept
- Intuitive introduction to limits through tables and graphs
- Formal limit laws are not part of this syllabus — numerical and graphical estimation is sufficient at SL
- The derivative understood as a gradient function (slope at a point) and as a rate of change

### SL 5.2 Increasing and Decreasing Functions
- Using the sign of $f'(x)$ to determine where a function is increasing ($f'(x) > 0$), stationary ($f'(x) = 0$), or decreasing ($f'(x) < 0$)

### SL 5.3 Derivative of Polynomials
- Power rule: $f(x) = ax^n \Rightarrow f'(x) = anx^{n-1}$, $n \in \mathbb{Z}$
- Derivatives of sums and constant multiples

### SL 5.4 Tangents and Normals
- Finding equations of tangent lines and normal lines at a given point, both analytically and with technology

### SL 5.5 Introduction to Integration
- Integration as the reverse of differentiation for $f(x) = ax^n + \ldots$, $n \in \mathbb{Z}, n \neq -1$
- Definite integrals computed with technology; area between a curve and the x-axis (above the axis)
- The constant of integration; using a boundary condition to determine $+c$

### SL 5.6 Stationary Points
- Points where the gradient equals zero; identifying local maxima and minima
- Solving $f'(x) = 0$ to locate stationary points

### SL 5.7 Optimisation in Context
- Applying derivatives to real-world problems: maximizing profit, minimizing cost, area and volume optimization

### SL 5.8 Trapezoidal Rule
- Approximating the area under a curve using the **trapezoidal rule**, from data tables or function values

## HL Extension

### AHL 5.9 Further Differentiation
- Derivatives of $\sin x$, $\cos x$, $\tan x$, $e^x$, $\ln x$, $x^n$ ($n \in \mathbb{Q}$)
- **Chain rule, product rule, quotient rule**
- Related rates of change

### AHL 5.10 Second Derivative
- Notation $\frac{d^2y}{dx^2}$, $f''(x)$
- Using the second derivative to classify stationary points and determine concavity; identifying points of inflexion

### AHL 5.11 Further Integration
- Integrating $x^n$ ($n \in \mathbb{Q}$), $\sin x$, $\cos x$, $\frac{1}{x}$, $e^x$ — both definite and indefinite
- Integration by inspection or by substitution of the form $\int f(g(x))g'(x)\,dx$

### AHL 5.12 Areas and Volumes
- Area enclosed between a curve and an axis; area between two curves
- **Volumes of revolution** about the x- or y-axis: $V = \int \pi y^2\,dx$

### AHL 5.13 Kinematics
- Relationships: $v = \frac{ds}{dt}$, $a = \frac{dv}{dt} = v\frac{dv}{ds}$
- Displacement over an interval: $\int_{t_1}^{t_2} v(t)\,dt$; total distance: $\int_{t_1}^{t_2} |v(t)|\,dt$
- Speed is the magnitude of velocity (always non-negative)

### AHL 5.14 Differential Equations: Setup and Separation
- Translating a real-world context into a differential equation
- Solving by **separation of variables**

### AHL 5.15 Slope Fields
- Drawing and interpreting slope field diagrams; sketching solution curves that match the field

### AHL 5.16 Euler's Method
- **Euler's method**: $y_{n+1} = y_n + h \cdot f(x_n, y_n)$ — a first-order numerical approach to solving $\frac{dy}{dx} = f(x, y)$
- Numerical solution of coupled systems using technology

### AHL 5.17 Coupled Systems and Phase Portraits
- Phase portraits for solutions of coupled linear systems $\frac{dx}{dt} = ax + by$, $\frac{dy}{dt} = cx + dy$
- Qualitative behaviour from **eigenvalues**: real distinct (saddle or node), complex (spiral), and stability
- Sketching trajectories; identifying equilibrium points

### AHL 5.18 Second Order Differential Equations
- Solving $\frac{d^2x}{dt^2} = f(x, \frac{dx}{dt}, t)$ numerically by reducing it to a coupled first-order system and applying Euler's method

## Key Equations

| Equation | Description |
|----------|-------------|
| $f(x) = ax^n \Rightarrow f'(x) = anx^{n-1}$ | Power rule |
| Trapezoidal rule: $\approx \frac{h}{2}(y_0 + y_n + 2(y_1 + \cdots + y_{n-1}))$ | Area approximation |
| $V = \int \pi y^2\,dx$ | Volume of revolution (HL) |
| $y_{n+1} = y_n + h f(x_n, y_n)$ | Euler's method (HL) |
| Total distance $= \int \|v(t)\|\,dt$ | Kinematics (HL) |

## Common Misconceptions

1. **Accuracy of the trapezoidal rule** — This is an approximation: it overestimates for concave-up functions and underestimates for concave-down ones.
2. **Displacement vs. distance** — Displacement integrates $v(t)$ and can be negative; total distance integrates $|v(t)|$ and is always non-negative.
3. **Stationary points and extrema** — $f'(x) = 0$ locates a stationary point but does not guarantee a max or min; it could be a stationary point of inflexion. Test the sign of $f'$ on either side, or use $f''$.
4. **Step size in Euler's method** — Halving the step size $h$ roughly halves the accumulated global error; smaller steps improve accuracy at the cost of more computation.

## Comparison with Other Courses

- AI SL calculus covers a light subset of AP Calculus AB: no formal limit laws, no Fundamental Theorem of Calculus development, and no chain rule at SL
- AI HL overlaps with AP Calculus AB/BC on differentiation techniques, kinematics, Euler's method, and separable differential equations — but omits series entirely (BC Unit 10) and L'Hôpital's rule
- Phase portraits and coupled systems (AHL 5.17) extend beyond AP Calculus BC into territory more typical of a first university ODE course
- AA HL includes integration by parts and Maclaurin series; AI HL does not
