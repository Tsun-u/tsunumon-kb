# Unit 5: Torque and Rotational Dynamics

> Exam Weight: 10--15% | ~12--17 Class Periods

## Topics

### 5.1 Rotational Kinematics
- Angular position: $\theta$ (in radians)
- Angular displacement: $\Delta\theta = \theta_f - \theta_i$
- Angular velocity: $\omega = \frac{\Delta\theta}{\Delta t}$ (rad/s)
- Angular acceleration: $\alpha = \frac{\Delta\omega}{\Delta t}$ (rad/s$^2$)
- Rotational kinematic equations (constant $\alpha$):
  - $\omega = \omega_0 + \alpha t$
  - $\theta = \theta_0 + \omega_0 t + \frac{1}{2}\alpha t^2$
  - $\omega^2 = \omega_0^2 + 2\alpha(\theta - \theta_0)$
- Sign convention: counterclockwise (CCW) is typically positive

### 5.2 Connecting Linear and Rotational Motion
- Arc length: $s = r\theta$
- Tangential velocity: $v = r\omega$
- Tangential acceleration: $a_t = r\alpha$
- Centripetal (radial) acceleration: $a_c = \frac{v^2}{r} = \omega^2 r$
- Points farther from the axis have greater linear speed but the same angular velocity

### 5.3 Torque
- Torque: $\tau = rF\sin\theta$ where $\theta$ is the angle between $\vec{r}$ and $\vec{F}$
- Equivalently: $\tau = r_\perp F = r F_\perp$ (lever arm method)
- $r_\perp$ (lever arm): perpendicular distance from axis to line of action of force
- Torque is a vector; CCW torque is positive, CW torque is negative (by convention)
- SI unit: N$\cdot$m (not joules, even though same dimensions)
- Torque depends on: magnitude of force, distance from axis, and angle of application

### 5.4 Rotational Inertia (Moment of Inertia)
- Rotational inertia (moment of inertia): $I = \sum m_i r_i^2$ (for discrete masses)
- Analogous to mass in linear motion; resistance to angular acceleration
- Depends on mass distribution relative to the axis of rotation
- Common moments of inertia (provided on exam):
  - Point mass: $I = mr^2$
  - Thin rod (center): $I = \frac{1}{12}mL^2$
  - Thin rod (end): $I = \frac{1}{3}mL^2$
  - Solid sphere: $I = \frac{2}{5}mR^2$
  - Hollow sphere (thin shell): $I = \frac{2}{3}mR^2$
  - Solid cylinder/disk: $I = \frac{1}{2}mR^2$
  - Hollow cylinder (thin hoop): $I = mR^2$
- Parallel axis theorem: $I = I_{cm} + Md^2$

### 5.5 Rotational Equilibrium and Newton's First Law in Rotational Form
- Rotational equilibrium: $\sum \tau = 0$
- An object in rotational equilibrium has zero angular acceleration ($\alpha = 0$)
- For full static equilibrium: both $\sum \vec{F} = 0$ AND $\sum \tau = 0$
- Choice of pivot point is arbitrary for equilibrium problems (any point gives $\sum \tau = 0$)

### 5.6 Newton's Second Law in Rotational Form
- $\sum \tau = I\alpha$
- Net torque produces angular acceleration proportional to torque and inversely proportional to moment of inertia
- Analogous to $\sum F = ma$ for translational motion

## Learning Objectives

- Describe rotational motion using angular position, velocity, and acceleration
- Apply rotational kinematic equations to solve problems with constant angular acceleration
- Relate linear and angular quantities ($v = r\omega$, $a_t = r\alpha$, $s = r\theta$)
- Calculate torque given force, position, and angle
- Determine the moment of inertia for systems of point masses
- Apply the parallel axis theorem
- Analyze systems in rotational equilibrium ($\sum \tau = 0$)
- Apply Newton's second law for rotation ($\sum \tau = I\alpha$)
- Solve combined translational and rotational problems (e.g., Atwood machine with pulley)

## Essential Knowledge

1. Angular quantities ($\theta$, $\omega$, $\alpha$) are analogous to linear quantities ($x$, $v$, $a$)
2. Linear and angular quantities are connected through the radius: $v = r\omega$, $a_t = r\alpha$
3. Torque is the rotational equivalent of force; it causes angular acceleration
4. The effectiveness of a force at producing rotation depends on the force magnitude, the distance from the axis, and the angle of application
5. Rotational inertia depends on both the mass and its distribution relative to the axis
6. Newton's second law for rotation: $\sum \tau = I\alpha$
7. An object in rotational equilibrium has zero net torque
8. The parallel axis theorem allows calculation of moment of inertia about any axis parallel to one through the center of mass

## Key Equations

### Rotational Kinematics (Constant $\alpha$)

$$\omega = \omega_0 + \alpha t$$

$$\theta = \theta_0 + \omega_0 t + \frac{1}{2}\alpha t^2$$

$$\omega^2 = \omega_0^2 + 2\alpha(\theta - \theta_0)$$

### Linear-Angular Relationships

$$s = r\theta, \quad v = r\omega, \quad a_t = r\alpha$$

### Torque

$$\tau = rF\sin\theta$$

$$\tau = r_\perp F \quad \text{(lever arm method)}$$

### Rotational Inertia

$$I = \sum m_i r_i^2 \quad \text{(point masses)}$$

$$I = I_{cm} + Md^2 \quad \text{(parallel axis theorem)}$$

### Newton's Second Law for Rotation

$$\sum \tau = I\alpha$$

## Linear-Rotational Analogy Table

| Linear | Rotational |
|--------|-----------|
| Position $x$ | Angle $\theta$ |
| Displacement $\Delta x$ | Angular displacement $\Delta\theta$ |
| Velocity $v$ | Angular velocity $\omega$ |
| Acceleration $a$ | Angular acceleration $\alpha$ |
| Mass $m$ | Moment of inertia $I$ |
| Force $F$ | Torque $\tau$ |
| $F = ma$ | $\tau = I\alpha$ |
| Momentum $p = mv$ | Angular momentum $L = I\omega$ |
| Impulse $J = F\Delta t$ | Angular impulse $\tau \Delta t$ |
| KE $= \frac{1}{2}mv^2$ | KE$_{rot} = \frac{1}{2}I\omega^2$ |

## Key Terminology

| Term | Definition |
|------|-----------|
| **Angular position ($\theta$)** | Angle of rotation from a reference direction; measured in radians |
| **Angular velocity ($\omega$)** | Rate of change of angular position; rad/s |
| **Angular acceleration ($\alpha$)** | Rate of change of angular velocity; rad/s$^2$ |
| **Torque ($\tau$)** | Tendency of a force to cause rotation about an axis |
| **Lever arm ($r_\perp$)** | Perpendicular distance from the rotation axis to the line of action of a force |
| **Moment of inertia ($I$)** | Measure of an object's resistance to angular acceleration; depends on mass distribution |
| **Parallel axis theorem** | $I = I_{cm} + Md^2$; relates moment of inertia about any axis to that about the CM |
| **Rotational equilibrium** | Net torque about any axis is zero; $\sum \tau = 0$ |
| **Tangential acceleration** | Component of linear acceleration along the direction of motion at a point on a rotating object |
| **Radial (centripetal) acceleration** | Acceleration directed toward the center of rotation |

## Common Misconceptions

1. **Torque and force are the same thing** -- No. A large force applied at the axis of rotation produces zero torque. Torque depends on where and at what angle the force is applied.
2. **N$\cdot$m (torque) is the same as joules (energy)** -- They have the same dimensions but are conceptually different. Torque is a vector-like quantity; energy is a scalar.
3. **Heavier objects always have larger moments of inertia** -- Not necessarily. Mass distribution matters. A hollow cylinder has $I = mR^2$ while a solid cylinder has $I = \frac{1}{2}mR^2$ for the same mass and radius.
4. **Angular velocity is the same as tangential velocity** -- No. $\omega$ is the same for all points on a rigid body; $v = r\omega$ varies with distance from the axis.
5. **The pivot point matters for equilibrium** -- For an object in equilibrium, $\sum \tau = 0$ about ANY chosen pivot. Choose the most convenient one (usually where unknown forces act).
6. **Moment of inertia is a fixed property** -- It depends on the axis of rotation. The same object has different $I$ about different axes.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Angular position | rad (radian) | dimensionless |
| Angular velocity | rad/s | [T]$^{-1}$ |
| Angular acceleration | rad/s$^2$ | [T]$^{-2}$ |
| Torque | N$\cdot$m | [M][L]$^2$[T]$^{-2}$ |
| Moment of inertia | kg$\cdot$m$^2$ | [M][L]$^2$ |
