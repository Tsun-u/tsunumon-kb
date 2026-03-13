# Unit 8: Applications of Integration
> AB Exam Weight: 10–15% | BC Exam Weight: 6–9% | ~12–13 Class Periods

## Big Ideas: CHA, FUN

---

## Topics

### 8.1 Finding the Average Value of a Function on an Interval
- **Learning Objective (CHA-4.B):** Find the average value of a function.
- **Essential Knowledge:**
  - **Average value of $f$ on $[a, b]$:**
    $$f_{\text{avg}} = \frac{1}{b - a}\int_a^b f(x)\,dx$$
  - **Mean Value Theorem for Integrals:** If $f$ is continuous on $[a, b]$, there exists $c \in [a, b]$ such that $f(c) = f_{\text{avg}}$.
  - The average value can be interpreted as the height of a rectangle with base $(b - a)$ that has the same area as $\int_a^b f(x)\,dx$.

### 8.2 Connecting Position, Velocity, and Acceleration of Functions Using Integrals
- **Learning Objective (CHA-4.C):** Find position, velocity, displacement using integrals.
- **Essential Knowledge:**
  - **Displacement** (net change in position): $\int_a^b v(t)\,dt = s(b) - s(a)$
  - **Total distance traveled:** $\int_a^b |v(t)|\,dt$
  - **Position at time $t$:** $s(t) = s(a) + \int_a^t v(\tau)\,d\tau$
  - **Velocity from acceleration:** $v(t) = v(a) + \int_a^t a(\tau)\,d\tau$
  - Common misconception: Displacement equals total distance. (Correct: they are equal only if the particle never changes direction.)

### 8.3 Using Accumulation Functions and Definite Integrals in Applied Contexts
- **Learning Objective (CHA-4.D):** Apply definite integrals to real-world accumulation problems.
- **Essential Knowledge:**
  - If $R(t)$ is a rate (e.g., gallons per minute), then $\int_a^b R(t)\,dt$ is the total quantity accumulated over $[a, b]$.
  - Net change: $f(b) = f(a) + \int_a^b f'(t)\,dt$
  - Students must interpret results in context with appropriate units.

### 8.4 Finding the Area Between Curves Expressed as Functions of $x$
- **Learning Objective (CHA-5.A):** Set up and evaluate area integrals.
- **Essential Knowledge:**
  - **Area between $f(x)$ and $g(x)$** on $[a, b]$ where $f(x) \geq g(x)$:
    $$A = \int_a^b [f(x) - g(x)]\,dx$$
  - The integrand is always (top function) $-$ (bottom function).
  - Find intersection points to determine the limits of integration.

### 8.5 Finding the Area Between Curves Expressed as Functions of $y$
- **Learning Objective (CHA-5.A):** Set up area integrals with respect to $y$.
- **Essential Knowledge:**
  - **Area between $x = f(y)$ and $x = g(y)$** on $[c, d]$ where $f(y) \geq g(y)$:
    $$A = \int_c^d [f(y) - g(y)]\,dy$$
  - The integrand is (right function) $-$ (left function).
  - Sometimes integrating with respect to $y$ is simpler than with respect to $x$.

### 8.6 Finding the Area Between Curves That Intersect at More Than Two Points
- **Learning Objective (CHA-5.A):** Handle area problems with multiple intersection points.
- **Essential Knowledge:**
  - Split the integral at each intersection point where the top/bottom relationship changes.
  - $A = \int_a^b |f(x) - g(x)|\,dx$ always gives the total area.
  - In practice, split into subintervals and determine which function is on top in each.

### 8.7 Volumes with Cross Sections: Squares and Rectangles
- **Learning Objective (CHA-5.B):** Calculate volumes using cross-sectional areas.
- **Essential Knowledge:**
  - **Volume by cross sections:**
    $$V = \int_a^b A(x)\,dx$$
    where $A(x)$ is the area of the cross section at position $x$.
  - **Square cross sections:** $A(x) = [f(x) - g(x)]^2$
  - **Rectangular cross sections:** Height is typically given as a function of the base.

### 8.8 Volumes with Cross Sections: Triangles and Semicircles
- **Learning Objective (CHA-5.B):** Calculate volumes with various cross-sectional shapes.
- **Essential Knowledge:**
  - **Equilateral triangle cross sections:** $A = \frac{\sqrt{3}}{4}s^2$ where $s = f(x) - g(x)$
  - **Isosceles right triangle cross sections:** $A = \frac{1}{2}s^2$ (legs = base)
  - **Semicircle cross sections:** $A = \frac{\pi}{8}s^2$ where $s$ is the diameter
  - The base of each cross section is typically the distance between two curves.

### 8.9 Volume with Disc Method: Revolving Around the $x$- or $y$-Axis
- **Learning Objective (CHA-5.C):** Calculate volumes of solids of revolution using the disc method.
- **Essential Knowledge:**
  - **Disc method (revolution around $x$-axis):**
    $$V = \pi\int_a^b [f(x)]^2\,dx$$
  - **Disc method (revolution around $y$-axis):**
    $$V = \pi\int_c^d [g(y)]^2\,dy$$
  - Used when the region is bounded by one curve and the axis of revolution.

### 8.10 Volume with Disc Method: Revolving Around Other Axes
- **Learning Objective (CHA-5.C):** Apply disc method for non-standard axes of revolution.
- **Essential Knowledge:**
  - Revolving around $y = k$ (horizontal line): $V = \pi\int_a^b [f(x) - k]^2\,dx$
  - Revolving around $x = k$ (vertical line): $V = \pi\int_c^d [g(y) - k]^2\,dy$
  - Key: the radius is the distance from the curve to the axis of revolution.

### 8.11 Volume with Washer Method: Revolving Around the $x$- or $y$-Axis
- **Learning Objective (CHA-5.C):** Calculate volumes using the washer method.
- **Essential Knowledge:**
  - **Washer method** (revolution around $x$-axis, region between two curves):
    $$V = \pi\int_a^b \left([R(x)]^2 - [r(x)]^2\right)\,dx$$
    where $R(x)$ = outer radius, $r(x)$ = inner radius.
  - The outer radius is the distance from the axis to the farther curve; the inner radius to the closer curve.
  - Common misconception: $V = \pi\int [R(x) - r(x)]^2\,dx$. (Correct: square each radius separately, then subtract.)

### 8.12 Volume with Washer Method: Revolving Around Other Axes
- **Learning Objective (CHA-5.C):** Apply washer method for non-standard axes.
- **Essential Knowledge:**
  - Revolving around $y = k$:
    - $R(x) = |f(x) - k|$ (farther curve)
    - $r(x) = |g(x) - k|$ (closer curve)
  - Revolving around $x = k$:
    - Use functions of $y$ and adjust radii accordingly.
  - Always draw a diagram to identify outer and inner radii correctly.

### 8.13 The Arc Length of a Smooth, Planar Curve and Distance Traveled (BC Only)
- **Learning Objective (CHA-5.D):** Calculate arc length.
- **Essential Knowledge:**
  - **Arc length** of $y = f(x)$ from $x = a$ to $x = b$:
    $$L = \int_a^b \sqrt{1 + [f'(x)]^2}\,dx$$
  - **Distance traveled** by a particle with position $(x(t), y(t))$:
    $$D = \int_a^b \sqrt{[x'(t)]^2 + [y'(t)]^2}\,dt$$
  - For a function of $y$: $L = \int_c^d \sqrt{1 + [g'(y)]^2}\,dy$

---

## Key Formulas Summary

| Concept | Formula |
|---------|---------|
| Average value | $f_{\text{avg}} = \frac{1}{b-a}\int_a^b f(x)\,dx$ |
| Displacement | $\int_a^b v(t)\,dt$ |
| Total distance | $\int_a^b \|v(t)\|\,dt$ |
| Area between curves | $\int_a^b [f(x) - g(x)]\,dx$ |
| Volume (cross sections) | $\int_a^b A(x)\,dx$ |
| Disc method | $\pi\int_a^b [R(x)]^2\,dx$ |
| Washer method | $\pi\int_a^b ([R(x)]^2 - [r(x)]^2)\,dx$ |
| Arc length (BC) | $\int_a^b \sqrt{1 + [f'(x)]^2}\,dx$ |

## Common Misconceptions
- Confusing displacement and total distance traveled.
- In washer method, squaring the difference of radii instead of subtracting the squares: $(R - r)^2 \neq R^2 - r^2$.
- Forgetting to include $\pi$ in disc/washer formulas.
- Setting up the wrong radius when revolving around a non-standard axis.
- Integrating with respect to the wrong variable (should match the axis of revolution).
- Forgetting that area between curves requires the absolute value of the difference (or splitting at intersection points).
