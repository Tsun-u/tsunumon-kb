# Unit 9: Parametric Equations, Polar Coordinates, and Vector-Valued Functions
> BC Only | BC Exam Weight: 11–12% | ~10–11 Class Periods

## Big Ideas: CHA, FUN

---

## Topics

### 9.1 Defining and Differentiating Parametric Equations
- **Learning Objective (CHA-6.A):** Calculate derivatives of parametric functions.
- **Essential Knowledge:**
  - A parametric curve is defined by $x = f(t)$, $y = g(t)$ for $t$ in some interval.
  - **First derivative:**
    $$\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{g'(t)}{f'(t)}, \quad \text{provided } f'(t) \neq 0$$
  - This gives the slope of the tangent line to the parametric curve at parameter value $t$.
  - Horizontal tangent: $\frac{dy}{dt} = 0$ and $\frac{dx}{dt} \neq 0$.
  - Vertical tangent: $\frac{dx}{dt} = 0$ and $\frac{dy}{dt} \neq 0$.

### 9.2 Second Derivatives of Parametric Equations
- **Learning Objective (CHA-6.B):** Calculate second derivatives of parametric functions.
- **Essential Knowledge:**
  - **Second derivative:**
    $$\frac{d^2y}{dx^2} = \frac{\frac{d}{dt}\left(\frac{dy}{dx}\right)}{\frac{dx}{dt}}$$
  - Take the derivative with respect to $t$ of the first derivative $\frac{dy}{dx}$, then divide by $\frac{dx}{dt}$.
  - Used to determine concavity of the parametric curve.
  - Common misconception: $\frac{d^2y}{dx^2} = \frac{d^2y/dt^2}{d^2x/dt^2}$. This is WRONG.

### 9.3 Finding Arc Lengths of Curves Given by Parametric Equations
- **Learning Objective (CHA-6.C):** Calculate arc length for parametric curves.
- **Essential Knowledge:**
  - **Arc length** of parametric curve from $t = a$ to $t = b$:
    $$L = \int_a^b \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2}\,dt$$
  - The integrand represents the speed $\frac{ds}{dt}$ of a particle traveling along the curve.

### 9.4 Defining and Differentiating Vector-Valued Functions
- **Learning Objective (FUN-8.A):** Define and differentiate vector-valued functions.
- **Essential Knowledge:**
  - A vector-valued function: $\vec{r}(t) = \langle x(t), y(t) \rangle$ or $\vec{r}(t) = x(t)\,\hat{i} + y(t)\,\hat{j}$
  - **Derivative:** $\vec{r}'(t) = \langle x'(t), y'(t) \rangle$
  - The derivative vector is tangent to the curve at each point.
  - **Velocity vector:** $\vec{v}(t) = \vec{r}'(t) = \langle x'(t), y'(t) \rangle$
  - **Acceleration vector:** $\vec{a}(t) = \vec{v}'(t) = \langle x''(t), y''(t) \rangle$

### 9.5 Integrating Vector-Valued Functions
- **Learning Objective (FUN-8.B):** Integrate vector-valued functions.
- **Essential Knowledge:**
  - $\int \vec{r}(t)\,dt = \left\langle \int x(t)\,dt, \int y(t)\,dt \right\rangle$
  - **Position from velocity:** $\vec{r}(t) = \vec{r}(a) + \int_a^t \vec{v}(\tau)\,d\tau$
  - Each component is integrated independently.

### 9.6 Solving Motion Problems Using Parametric and Vector-Valued Functions
- **Learning Objective (CHA-6.D):** Analyze motion using parametric/vector functions.
- **Essential Knowledge:**
  - **Speed** (scalar): $|\vec{v}(t)| = \sqrt{[x'(t)]^2 + [y'(t)]^2}$
  - **Total distance traveled:** $\int_a^b |\vec{v}(t)|\,dt = \int_a^b \sqrt{[x'(t)]^2 + [y'(t)]^2}\,dt$
  - **Displacement vector:** $\vec{r}(b) - \vec{r}(a) = \int_a^b \vec{v}(t)\,dt$
  - A particle is at rest when $\vec{v}(t) = \langle 0, 0 \rangle$ (both components zero).

### 9.7 Defining Polar Coordinates and Differentiating in Polar Form
- **Learning Objective (FUN-8.C):** Convert between polar and rectangular; differentiate polar curves.
- **Essential Knowledge:**
  - Polar coordinates: $(r, \theta)$ where $x = r\cos\theta$, $y = r\sin\theta$.
  - Conversions: $r^2 = x^2 + y^2$, $\tan\theta = \frac{y}{x}$
  - For a polar curve $r = f(\theta)$:
    - $x = f(\theta)\cos\theta$, $y = f(\theta)\sin\theta$
    - **Slope of polar curve:**
      $$\frac{dy}{dx} = \frac{\frac{dy}{d\theta}}{\frac{dx}{d\theta}} = \frac{f'(\theta)\sin\theta + f(\theta)\cos\theta}{f'(\theta)\cos\theta - f(\theta)\sin\theta}$$

### 9.8 Finding the Area of a Polar Region or the Area Bounded by a Single Polar Curve
- **Learning Objective (CHA-5.D):** Calculate area in polar coordinates.
- **Essential Knowledge:**
  - **Area enclosed by $r = f(\theta)$** from $\theta = \alpha$ to $\theta = \beta$:
    $$A = \frac{1}{2}\int_{\alpha}^{\beta} [f(\theta)]^2\,d\theta$$
  - Careful: ensure the limits $\alpha$ and $\beta$ trace the region exactly once.
  - For curves like cardioids and rose curves, symmetry can simplify calculations.

### 9.9 Finding the Area of the Region Bounded by Two Polar Curves
- **Learning Objective (CHA-5.D):** Calculate area between polar curves.
- **Essential Knowledge:**
  - **Area between two polar curves** $r_1 = f(\theta)$ (outer) and $r_2 = g(\theta)$ (inner):
    $$A = \frac{1}{2}\int_{\alpha}^{\beta} \left([f(\theta)]^2 - [g(\theta)]^2\right)\,d\theta$$
  - Find intersection points by setting $f(\theta) = g(\theta)$ and also check $r = 0$.
  - May need to split into multiple integrals if which curve is "outer" changes.

---

## Key Formulas Summary

| Concept | Formula |
|---------|---------|
| Parametric $dy/dx$ | $\frac{dy/dt}{dx/dt}$ |
| Parametric $d^2y/dx^2$ | $\frac{d/dt(dy/dx)}{dx/dt}$ |
| Parametric arc length | $\int_a^b \sqrt{(dx/dt)^2 + (dy/dt)^2}\,dt$ |
| Speed | $\sqrt{[x'(t)]^2 + [y'(t)]^2}$ |
| Polar area | $\frac{1}{2}\int_\alpha^\beta [r(\theta)]^2\,d\theta$ |
| Polar area (between curves) | $\frac{1}{2}\int_\alpha^\beta ([r_1]^2 - [r_2]^2)\,d\theta$ |
| Polar to rectangular | $x = r\cos\theta$, $y = r\sin\theta$ |
| Rectangular to polar | $r = \sqrt{x^2+y^2}$, $\theta = \arctan(y/x)$ |

## Common Misconceptions
- Computing $\frac{d^2y}{dx^2}$ for parametric curves as $\frac{y''(t)}{x''(t)}$ instead of $\frac{d/dt(dy/dx)}{dx/dt}$.
- Confusing displacement (a vector) with distance (a scalar) in motion problems.
- In polar area, forgetting the $\frac{1}{2}$ factor or not squaring $r$.
- Using $\int [r_1 - r_2]^2$ instead of $\int [r_1^2 - r_2^2]$ for polar area between curves.
- Not accounting for all intersection points of polar curves (some may occur at $r = 0$ at different angles).
- Confusing the direction of motion with the sign of $r$ in polar coordinates.
