# Unit 9: Parametric Equations, Polar Coordinates, and Vector-Valued Functions
> BC Only | BC Exam Weight: 11–12% | ~10–11 Class Periods

---

## Topics

### 9.1 Defining and Differentiating Parametric Equations
- A parametric curve describes a path through the plane by expressing both $x$ and $y$ as separate functions of a third variable $t$: $x = f(t)$, $y = g(t)$.
- The slope of the tangent line at parameter value $t$ comes from dividing the rate of $y$-change by the rate of $x$-change:
  $$\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{g'(t)}{f'(t)}, \quad f'(t) \neq 0$$
- **Horizontal tangent:** $\frac{dy}{dt} = 0$ with $\frac{dx}{dt} \neq 0$.
- **Vertical tangent:** $\frac{dx}{dt} = 0$ with $\frac{dy}{dt} \neq 0$.

### 9.2 Second Derivatives of Parametric Equations
- The second derivative tests concavity for a parametric curve. The rule is: differentiate $\frac{dy}{dx}$ with respect to $t$, then divide by $\frac{dx}{dt}$:
  $$\frac{d^2y}{dx^2} = \frac{\dfrac{d}{dt}\!\left(\dfrac{dy}{dx}\right)}{\dfrac{dx}{dt}}$$
- A critical misconception: $\frac{d^2y}{dx^2} \neq \frac{y''(t)}{x''(t)}$. The second $x$-derivative cannot simply replace $\frac{dx}{dt}$ in the denominator.

### 9.3 Finding Arc Lengths of Curves Given by Parametric Equations
- To find the total arc length of a parametric curve from $t = a$ to $t = b$, integrate the speed (rate of change of arc length) over $t$:
  $$L = \int_a^b \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2}\,dt$$
- The integrand $\sqrt{(dx/dt)^2 + (dy/dt)^2}$ is the instantaneous speed of a particle tracing the curve.

### 9.4 Defining and Differentiating Vector-Valued Functions
- A **vector-valued function** packages the parametric coordinates into a single vector: $\vec{r}(t) = \langle x(t), y(t) \rangle$.
- Differentiating component-by-component gives:
  - **Velocity vector:** $\vec{v}(t) = \vec{r}'(t) = \langle x'(t), y'(t) \rangle$ — tangent to the path, pointing in the direction of motion
  - **Acceleration vector:** $\vec{a}(t) = \vec{v}'(t) = \langle x''(t), y''(t) \rangle$

### 9.5 Integrating Vector-Valued Functions
- Integration of a vector-valued function also happens component-by-component:
  $$\int \vec{r}(t)\,dt = \left\langle \int x(t)\,dt,\; \int y(t)\,dt \right\rangle$$
- **Recovering position from velocity:** $\vec{r}(t) = \vec{r}(a) + \int_a^t \vec{v}(\tau)\,d\tau$, provided an initial position is known.

### 9.6 Solving Motion Problems Using Parametric and Vector-Valued Functions
- **Speed** is the magnitude (length) of the velocity vector — a scalar, always non-negative:
  $$|\vec{v}(t)| = \sqrt{[x'(t)]^2 + [y'(t)]^2}$$
- **Total distance traveled** integrates speed over time:
  $$D = \int_a^b |\vec{v}(t)|\,dt = \int_a^b \sqrt{[x'(t)]^2 + [y'(t)]^2}\,dt$$
- **Displacement vector** is the net vector change in position: $\vec{r}(b) - \vec{r}(a) = \int_a^b \vec{v}(t)\,dt$.
- A particle is momentarily at rest only when **both** component velocities equal zero simultaneously.

### 9.7 Defining Polar Coordinates and Differentiating in Polar Form
- Polar coordinates locate a point by its distance from the origin $r$ and angle from the positive $x$-axis $\theta$:
  - Converting to rectangular: $x = r\cos\theta$, $y = r\sin\theta$
  - Converting back: $r^2 = x^2 + y^2$, $\tan\theta = \frac{y}{x}$
- For a polar curve $r = f(\theta)$, write $x$ and $y$ as functions of $\theta$, then apply the parametric slope formula:
  $$\frac{dy}{dx} = \frac{f'(\theta)\sin\theta + f(\theta)\cos\theta}{f'(\theta)\cos\theta - f(\theta)\sin\theta}$$

### 9.8 Finding the Area of a Polar Region or the Area Bounded by a Single Polar Curve
- Polar area is built from infinitely thin wedge-shaped sectors rather than rectangular strips. The area swept from $\theta = \alpha$ to $\theta = \beta$ by the curve $r = f(\theta)$ is:
  $$A = \frac{1}{2}\int_{\alpha}^{\beta} [f(\theta)]^2\,d\theta$$
- Choose limits so the curve traces the region exactly once — for periodic curves like cardioids and rose curves, using symmetry helps avoid double-counting.

### 9.9 Finding the Area of the Region Bounded by Two Polar Curves
- To find the area between an outer curve $r_1 = f(\theta)$ and an inner curve $r_2 = g(\theta)$:
  $$A = \frac{1}{2}\int_{\alpha}^{\beta} \left([f(\theta)]^2 - [g(\theta)]^2\right)\,d\theta$$
- Finding the limits requires solving $f(\theta) = g(\theta)$ for intersection angles, and also checking whether curves pass through the origin $r = 0$ at different angles — those are intersections that the algebraic equation misses.
- If the outer and inner roles switch over the interval, split the integral at those crossover angles.

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
- Computing the parametric second derivative as $\frac{y''(t)}{x''(t)}$ — this is wrong; the correct formula involves differentiating $dy/dx$ with respect to $t$, not computing second derivatives of $x$ and $y$ separately.
- Confusing **displacement** (a vector pointing from start to finish) with **distance** (a scalar that adds up all path length regardless of direction).
- In polar area, omitting the $\frac{1}{2}$ factor or forgetting to square $r$ — both of these lead to answers that are off by a constant.
- Writing the area between polar curves as $\frac{1}{2}\int [r_1 - r_2]^2\,d\theta$ instead of $\frac{1}{2}\int [r_1^2 - r_2^2]\,d\theta$.
- Missing intersection points of polar curves that occur at the origin but at different $\theta$ values — the equation $r_1 = r_2$ alone does not catch these.
- Losing track of the sign of $r$ when interpreting direction of motion in polar coordinates.
