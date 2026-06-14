# Unit 8: Applications of Integration
> AB Exam Weight: 10–15% | BC Exam Weight: 6–9% | ~12–13 Class Periods

---

## Topics

### 8.1 Finding the Average Value of a Function on an Interval
- The **average value** of $f$ on $[a, b]$ spreads the total accumulated area evenly across the interval width:
  $$f_{\text{avg}} = \frac{1}{b - a}\int_a^b f(x)\,dx$$
- Geometrically, $f_{\text{avg}}$ is the height of a rectangle with base $(b - a)$ whose area matches $\int_a^b f(x)\,dx$.
- The **Mean Value Theorem for Integrals** guarantees that if $f$ is continuous, there is at least one $c \in [a, b]$ where $f$ actually attains this average value: $f(c) = f_{\text{avg}}$.

### 8.2 Connecting Position, Velocity, and Acceleration of Functions Using Integrals
- Integration reverses differentiation, so it reconstructs quantities from their rates:
  - **Displacement** (signed net change): $\int_a^b v(t)\,dt = s(b) - s(a)$
  - **Total distance traveled:** $\int_a^b |v(t)|\,dt$ — use the absolute value to count backward motion positively
  - **Position at time $t$:** $s(t) = s(a) + \int_a^t v(\tau)\,d\tau$
  - **Velocity from acceleration:** $v(t) = v(a) + \int_a^t a(\tau)\,d\tau$
- Displacement and total distance are equal only when the particle never reverses direction; otherwise displacement can be much smaller.

### 8.3 Using Accumulation Functions and Definite Integrals in Applied Contexts
- Whenever a rate $R(t)$ is given (gallons per minute, dollars per day, etc.), $\int_a^b R(t)\,dt$ gives the total quantity accumulated over $[a, b]$ — with appropriate units carried through.
- The **net change formula** summarizes this idea: $f(b) = f(a) + \int_a^b f'(t)\,dt$.
- Always interpret answers in context: a pure number without units or a verbal explanation is incomplete.

### 8.4 Finding the Area Between Curves Expressed as Functions of $x$
- When two curves $f(x)$ and $g(x)$ bound a region with $f(x) \geq g(x)$ throughout $[a, b]$, their enclosed area is:
  $$A = \int_a^b [f(x) - g(x)]\,dx$$
- The integrand is always (top function) minus (bottom function) — setting it up the wrong way around gives a negative result.
- Find intersection points by solving $f(x) = g(x)$ to determine the correct limits.

### 8.5 Finding the Area Between Curves Expressed as Functions of $y$
- Sometimes it is more natural to integrate horizontally. For curves $x = f(y)$ and $x = g(y)$ with $f(y) \geq g(y)$ (right minus left) on $[c, d]$:
  $$A = \int_c^d [f(y) - g(y)]\,dy$$
- This approach often simplifies regions that would require splitting into multiple $x$-integrals.

### 8.6 Finding the Area Between Curves That Intersect at More Than Two Points
- When curves cross more than twice, the "top" and "bottom" roles swap at each crossing. Split the total interval at every intersection point and write a separate integral for each sub-region.
- In principle $A = \int_a^b |f(x) - g(x)|\,dx$ gives the total area, but in practice you remove the absolute value by checking which function dominates on each piece.

### 8.7 Volumes with Cross Sections: Squares and Rectangles
- For a solid whose cross sections perpendicular to the $x$-axis are known shapes, integrate the cross-sectional area:
  $$V = \int_a^b A(x)\,dx$$
- **Square cross sections:** $A(x) = [f(x) - g(x)]^2$, where $f(x) - g(x)$ is the side length.
- **Rectangular cross sections:** the height is usually given as a specified function of the base $f(x) - g(x)$.

### 8.8 Volumes with Cross Sections: Triangles and Semicircles
- The same slice-and-integrate framework applies to other cross-sectional shapes; only the area formula $A(x)$ changes:
  - **Equilateral triangle** (side $s$): $A = \frac{\sqrt{3}}{4}s^2$
  - **Isosceles right triangle** (legs equal the base $s$): $A = \frac{1}{2}s^2$
  - **Semicircle** (diameter $s$): $A = \frac{\pi}{8}s^2$
- In all cases, $s = f(x) - g(x)$, the width of the base region at each $x$.

### 8.9 Volume with Disc Method: Revolving Around the $x$- or $y$-Axis
- Rotating a region bounded by one curve around an axis generates a solid of revolution. Each cross section is a circular disc with area $\pi r^2$:
  - **Around the $x$-axis:** $V = \pi\int_a^b [f(x)]^2\,dx$
  - **Around the $y$-axis:** $V = \pi\int_c^d [g(y)]^2\,dy$
- Use the disc method only when the region touches the axis of revolution with no gap.

### 8.10 Volume with Disc Method: Revolving Around Other Axes
- When the axis of revolution is a horizontal line $y = k$ or a vertical line $x = k$, the radius is the distance from the curve to that line:
  - Around $y = k$: $V = \pi\int_a^b [f(x) - k]^2\,dx$
  - Around $x = k$: $V = \pi\int_c^d [g(y) - k]^2\,dy$
- The key adjustment: always measure the radius as a distance, which may require thinking about whether the curve is above or below (left or right of) the axis.

### 8.11 Volume with Washer Method: Revolving Around the $x$- or $y$-Axis
- When there is a gap between the region and the axis — i.e., two curves bound the region — each cross section is a washer (a disc with a hole punched out):
  $$V = \pi\int_a^b \left([R(x)]^2 - [r(x)]^2\right)\,dx$$
  where $R(x)$ is the outer radius (farther curve to axis) and $r(x)$ is the inner radius (closer curve to axis).
- The outer and inner radii are squared **separately**, then subtracted — a common mistake is to square the difference $(R - r)^2$ instead, which is incorrect.

### 8.12 Volume with Washer Method: Revolving Around Other Axes
- For non-standard axes, redefine the radii as distances from each curve to the axis:
  - Around $y = k$: $R(x) = |f(x) - k|$ (outer), $r(x) = |g(x) - k|$ (inner)
  - Around $x = k$: rewrite curves as functions of $y$ and measure horizontal distances
- Drawing a labeled diagram is essentially mandatory here — it is very easy to mix up which curve is outer and which is inner without a picture.

### 8.13 The Arc Length of a Smooth, Planar Curve and Distance Traveled (BC Only)
- The length of a smooth curve $y = f(x)$ from $x = a$ to $x = b$ is found by summing infinitely many tiny straight-line segments:
  $$L = \int_a^b \sqrt{1 + [f'(x)]^2}\,dx$$
- For a parametric path $(x(t), y(t))$, the same idea gives total distance traveled:
  $$D = \int_a^b \sqrt{[x'(t)]^2 + [y'(t)]^2}\,dt$$
- Integrating with respect to $y$ is also possible: $L = \int_c^d \sqrt{1 + [g'(y)]^2}\,dy$.

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
- Conflating displacement (signed, can be small or zero) with total distance traveled (always non-negative and at least as large).
- In the washer method, writing $\pi\int [R(x) - r(x)]^2\,dx$ instead of $\pi\int ([R(x)]^2 - [r(x)]^2)\,dx$ — these are not equal.
- Forgetting the $\pi$ factor entirely in disc and washer formulas.
- Misidentifying the outer vs. inner radius when the axis of revolution is not a coordinate axis.
- Integrating with respect to the wrong variable — the variable should match the direction perpendicular to the axis of revolution.
- Not splitting the area integral at intersection points when curves switch which is on top, leading to cancellation that produces an area that is too small.
