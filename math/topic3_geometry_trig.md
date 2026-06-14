# Topic 3: Geometry and Trigonometry

> SL: 25 hours | HL: 51 hours

## SL Content

### 3.1 3D Geometry
- Volume and surface area formulas for common 3D solids — prisms, cylinders, spheres, cones, and pyramids — extend the 2D ideas students already know
- Straight-line distance between two points in three dimensions: $d = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2 + (z_2-z_1)^2}$
- The midpoint between two 3D points averages each coordinate separately

### 3.2 Trigonometric Ratios
- Right-triangle trigonometry defines $\sin\theta$, $\cos\theta$, $\tan\theta$ as ratios of sides (SOH-CAH-TOA)
- Certain "special" angles — 0°, 30°, 45°, 60°, 90° — have exact trig values worth memorising
- Pythagorean identity: $\sin^2\theta + \cos^2\theta = 1$, a direct consequence of the unit circle definition

### 3.3 Non-Right Triangles
- **Sine rule**: $\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C}$ — connects a side to the sine of its opposite angle
  - The ambiguous case arises when given two sides and a non-included angle; two distinct triangles may both satisfy the given information
- **Cosine rule**: $c^2 = a^2 + b^2 - 2ab\cos C$ — generalises Pythagoras for oblique triangles
- **Area of triangle**: $A = \frac{1}{2}ab\sin C$ — useful when height is unknown but two sides and their included angle are given

### 3.4 Radian Measure
- $\pi$ radians = 180°; multiplying by $\frac{180}{\pi}$ converts radians to degrees, and by $\frac{\pi}{180}$ converts the other way
- Arc length along a circle: $s = r\theta$ (angle $\theta$ must be in radians)
- Area of a circular sector: $A = \frac{1}{2}r^2\theta$

### 3.5 Unit Circle and Trigonometric Functions
- Extending trig beyond right triangles: $\sin$ and $\cos$ are coordinates of a point on a unit circle as the angle sweeps from the positive $x$-axis
- Sign conventions in each quadrant follow the ASTC pattern (All positive, Sine, Tangent, Cosine)
- Periodic behavior: $\sin$ and $\cos$ repeat every $2\pi$; $\tan$ has the shorter period $\pi$
- Graphs of $\sin x$, $\cos x$, and $\tan x$ each have characteristic shapes worth sketching from memory
- Transformations shift, scale, or reflect these graphs: $f(x) = a\sin(b(x-c)) + d$ gives amplitude $|a|$, period $\frac{2\pi}{b}$, phase shift $c$, and vertical shift $d$

### 3.6 Trigonometric Equations
- Basic equations like $\sin x = k$ typically have multiple solutions; use the inverse trig function for the principal value, then apply symmetry and periodicity to find others
- More complex equations are tackled by substituting identities to reduce everything to a single trig function, then factoring or using the quadratic formula
- Always check which solutions fall inside the specified interval before writing the final answer

## HL Extension

### 3.7 Reciprocal and Inverse Trigonometric Functions
- Three reciprocal functions: $\sec\theta = 1/\cos\theta$, $\csc\theta = 1/\sin\theta$, $\cot\theta = 1/\tan\theta$
- Inverse functions $\arcsin$, $\arccos$, $\arctan$ recover the angle from a ratio, but each has a restricted domain to ensure a unique output
- Additional Pythagorean identities derived from dividing the basic one through by $\cos^2\theta$ or $\sin^2\theta$: $1 + \tan^2\theta = \sec^2\theta$, $1 + \cot^2\theta = \csc^2\theta$

### 3.8 Compound Angle Identities
- $\sin(A \pm B) = \sin A\cos B \pm \cos A\sin B$
- $\cos(A \pm B) = \cos A\cos B \mp \sin A\sin B$
- $\tan(A \pm B) = \frac{\tan A \pm \tan B}{1 \mp \tan A\tan B}$
- **Double angle formulas** are the special case $A = B$:
  - $\sin 2A = 2\sin A\cos A$
  - $\cos 2A = \cos^2 A - \sin^2 A = 2\cos^2 A - 1 = 1 - 2\sin^2 A$

### 3.9 Vectors (HL)
- Vectors in 2D and 3D carry both magnitude and direction: $\vec{v} = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$
- Magnitude (length of vector): $|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$
- A unit vector points in the same direction but has length 1: $\hat{v} = \frac{\vec{v}}{|\vec{v}|}$
- **Scalar (dot) product**: $\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}|\cos\theta = a_1b_1 + a_2b_2 + a_3b_3$ — gives a number and reveals the angle between two vectors
- **Vector (cross) product**: $\vec{a} \times \vec{b}$ produces a new vector perpendicular to both, with magnitude $|\vec{a}||\vec{b}|\sin\theta$; its direction follows the right-hand rule
- Lines in 3D are described parametrically: $\vec{r} = \vec{a} + t\vec{b}$ — a starting point plus a scalar multiple of a direction vector
- Planes can be written as $\vec{r} \cdot \vec{n} = d$ or equivalently $ax + by + cz = d$, where $\vec{n}$ is a normal vector to the plane
- Finding angles between two lines, two planes, or a line and a plane all use the dot product formula

## Key Equations

| Equation | Description |
|----------|-------------|
| $\frac{a}{\sin A} = \frac{b}{\sin B}$ | Sine rule |
| $c^2 = a^2 + b^2 - 2ab\cos C$ | Cosine rule |
| $A = \frac{1}{2}ab\sin C$ | Area of triangle |
| $s = r\theta$ | Arc length |
| $\sin^2\theta + \cos^2\theta = 1$ | Pythagorean identity |
| $\vec{a} \cdot \vec{b} = \|\vec{a}\|\|\vec{b}\|\cos\theta$ | Dot product (HL) |

## Common Misconceptions

1. **"Sine rule always gives one answer"** -- When two sides and a non-included angle are known, there can be two geometrically valid triangles; always check both possibilities before discarding one.
2. **"Radians and degrees are interchangeable without conversion"** -- Formulas such as $s = r\theta$ and $A = \frac{1}{2}r^2\theta$ are only valid when the angle is measured in radians; plugging in degrees gives wrong answers.
3. **"$\sin^{-1}$ is the same as $1/\sin$"** -- The notation $\sin^{-1}$ means the arcsine (inverse function), not the reciprocal; the reciprocal of $\sin x$ is $\csc x$.
4. **"Vectors and scalars can be freely mixed in arithmetic"** -- Vectors and scalars belong to different mathematical objects; you can scale a vector by a scalar, but you cannot add a vector and a scalar directly.

## Comparison with AP Mathematics

- Unit circle trigonometry, standard identities, and equation-solving overlap considerably between IB AA and AP Pre-Calculus
- IB HL's treatment of 3D vectors — including cross products, parametric lines, and plane equations — goes substantially further than AP Pre-Calculus and is more aligned with university-level multivariable calculus
- Compound angle identities appear in both curricula, though IB HL problems tend to require more creative manipulation
- AP Calculus does not typically include 3D vector geometry; students encounter that material later in courses like AP Physics or university multivariable calculus
