# Unit 5: Torque and Rotational Dynamics

> Exam Weight: 10--15% | ~12--17 Class Periods

## Topics

### 5.1 Rotational Kinematics
- Angular position $\theta$ specifies orientation in radians relative to a reference direction
- Angular displacement: $\Delta\theta = \theta_f - \theta_i$
- Angular velocity: $\omega = \frac{\Delta\theta}{\Delta t}$ (rad/s)
- Angular acceleration: $\alpha = \frac{\Delta\omega}{\Delta t}$ (rad/s$^2$)
- When $\alpha$ is constant, three kinematic equations apply (mirrors of the linear set):
  - $\omega = \omega_0 + \alpha t$
  - $\theta = \theta_0 + \omega_0 t + \frac{1}{2}\alpha t^2$
  - $\omega^2 = \omega_0^2 + 2\alpha(\theta - \theta_0)$
- Standard sign convention: counterclockwise (CCW) rotations are taken as positive

### 5.2 Connecting Linear and Rotational Motion
- Arc length: $s = r\theta$
- Tangential velocity: $v = r\omega$
- Tangential acceleration: $a_t = r\alpha$
- Centripetal (radial) acceleration: $a_c = \frac{v^2}{r} = \omega^2 r$
- All points on a rigid body share the same $\omega$, but those farther from the axis sweep through greater linear distances and move at higher tangential speeds

### 5.3 Torque
- Torque: $\tau = rF\sin\theta$ where $\theta$ is the angle between $\vec{r}$ and $\vec{F}$
- Equivalently: $\tau = r_\perp F = r F_\perp$ (lever arm method)
- $r_\perp$ (lever arm): shortest distance from the rotation axis to the line along which the force acts
- Torque has directional sense: CCW is positive and CW is negative by the standard convention
- SI unit: N$\cdot$m — same dimensional form as joules but a physically distinct quantity
- Three factors govern the torque a force produces: its magnitude, its distance from the axis, and its angle of application

### 5.4 Rotational Inertia (Moment of Inertia)
- Rotational inertia (moment of inertia): $I = \sum m_i r_i^2$ (for discrete masses)
- Plays the role of inertial mass in rotation — greater $I$ means more torque is needed to produce the same angular acceleration
- Shifting mass farther from the rotation axis raises $I$; the geometry of the distribution matters as much as the total mass
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
- When net torque is zero, angular acceleration is zero — the object either stays stationary or rotates at a steady rate
- Complete static equilibrium requires both conditions: $\sum \vec{F} = 0$ (no translational acceleration) and $\sum \tau = 0$ (no angular acceleration)
- The pivot point used to calculate torques is a free choice; any selection will satisfy $\sum \tau = 0$ for a body in true equilibrium

### 5.6 Newton's Second Law in Rotational Form
- $\sum \tau = I\alpha$
- A net torque generates angular acceleration in the same direction; doubling the torque doubles $\alpha$, while doubling the moment of inertia halves $\alpha$
- This is the direct rotational counterpart of $\sum F = ma$ for linear dynamics

## Skills to Master

- Express rotational motion in terms of angular position, velocity, and acceleration
- Use rotational kinematic equations to find unknown quantities under constant angular acceleration
- Convert between linear and angular quantities using $v = r\omega$, $a_t = r\alpha$, and $s = r\theta$
- Compute torque from a given force, its point of application, and its angle relative to the moment arm
- Find the moment of inertia for a collection of point masses
- Use the parallel axis theorem to shift the rotation axis away from the center of mass
- Establish whether a system satisfies rotational equilibrium ($\sum \tau = 0$)
- Use Newton's second law in rotational form ($\sum \tau = I\alpha$) to predict angular acceleration
- Handle problems where translational and rotational motion are coupled (e.g., a pulley with mass)

## Core Concepts

1. The angular quantities $\theta$, $\omega$, and $\alpha$ play the same roles in rotational motion that $x$, $v$, and $a$ play in linear motion
2. A rigid body's angular and linear quantities are tied together through the radius: $v = r\omega$ and $a_t = r\alpha$
3. Torque is what drives angular acceleration, just as net force drives linear acceleration
4. How effectively a force can rotate an object depends on three factors: the magnitude of that force, how far it acts from the axis, and the angle at which it is applied
5. An object's resistance to changes in rotation — its rotational inertia — depends not just on total mass but on how that mass is arranged around the axis
6. The rotational version of Newton's second law states $\sum \tau = I\alpha$
7. A system in rotational equilibrium experiences zero net torque, so its angular velocity remains unchanged
8. The parallel axis theorem, $I = I_{cm} + Md^2$, lets you find the rotational inertia about any axis that runs parallel to one passing through the center of mass

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
| **Angular position ($\theta$)** | How far an object has rotated from its reference orientation, expressed in radians |
| **Angular velocity ($\omega$)** | How quickly the angular position is changing; units of rad/s |
| **Angular acceleration ($\alpha$)** | How quickly the angular velocity is changing; units of rad/s$^2$ |
| **Torque ($\tau$)** | The rotational influence of a force — its ability to start, stop, or change rotation about an axis |
| **Lever arm ($r_\perp$)** | The shortest distance from the rotation axis to the line along which a force acts |
| **Moment of inertia ($I$)** | A body's rotational inertia — how strongly it resists angular acceleration; larger when mass is farther from the axis |
| **Parallel axis theorem** | $I = I_{cm} + Md^2$; shifts the known center-of-mass rotational inertia to any parallel axis a distance $d$ away |
| **Rotational equilibrium** | State in which the net torque on an object about any axis equals zero; $\sum \tau = 0$ |
| **Tangential acceleration** | The component of a point's linear acceleration that acts tangent to its circular path |
| **Radial (centripetal) acceleration** | The component of a point's linear acceleration that points toward the center of its circular path |

## Common Misconceptions

1. **Torque and force are interchangeable** -- They are not. A very large force applied exactly at the axis produces zero torque; what matters is the force's moment arm and angle, not just its magnitude.
2. **N$\cdot$m for torque equals joules for energy** -- The units share the same dimensions, but torque and energy are fundamentally different physical quantities. Torque has directional character; energy is a scalar.
3. **A more massive object always has a greater moment of inertia** -- Not always. How the mass is distributed around the axis is what counts. A hollow cylinder ($I = mR^2$) has twice the rotational inertia of a solid cylinder ($I = \frac{1}{2}mR^2$) even with identical mass and radius.
4. **Angular velocity and tangential velocity mean the same thing** -- They do not. Every point on a spinning rigid body shares the same $\omega$, but tangential speed $v = r\omega$ grows with distance from the axis.
5. **Choosing a different pivot changes whether equilibrium holds** -- If an object is truly in equilibrium, $\sum \tau = 0$ regardless of which pivot you select. Pick whichever point eliminates the most unknowns (often where an unknown force is applied).
6. **Moment of inertia is an intrinsic, fixed property of an object** -- It changes with the axis of rotation. The same object has different values of $I$ about different axes.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Angular position | rad (radian) | dimensionless |
| Angular velocity | rad/s | [T]$^{-1}$ |
| Angular acceleration | rad/s$^2$ | [T]$^{-2}$ |
| Torque | N$\cdot$m | [M][L]$^2$[T]$^{-2}$ |
| Moment of inertia | kg$\cdot$m$^2$ | [M][L]$^2$ |
