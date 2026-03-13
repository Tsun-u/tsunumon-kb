# A.4: Rigid Body Mechanics

> Theme A: Space, Time and Motion | HL only

## Key Concepts

### Torque
- **Torque** ($\tau$): rotational equivalent of force
- $\tau = Fr\sin\theta$ where $r$ is the distance from the pivot and $\theta$ is the angle between force and position vector
- SI unit: N·m (not joules, even though dimensionally equivalent)
- Net torque causes angular acceleration: $\tau_{net} = I\alpha$

### Moment of Inertia
- **Moment of inertia** ($I$): rotational equivalent of mass; resistance to angular acceleration
- For point masses: $I = \sum m_i r_i^2$
- Depends on mass distribution relative to the axis of rotation
- Common shapes (provided in data booklet):
  - Solid sphere: $I = \frac{2}{5}mr^2$
  - Hollow sphere: $I = \frac{2}{3}mr^2$
  - Solid cylinder/disk: $I = \frac{1}{2}mr^2$
  - Thin rod (center): $I = \frac{1}{12}mL^2$
  - Thin rod (end): $I = \frac{1}{3}mL^2$

### Rotational Kinematics
- Angular displacement: $\theta$ (rad)
- Angular velocity: $\omega = \frac{d\theta}{dt}$ (rad/s)
- Angular acceleration: $\alpha = \frac{d\omega}{dt}$ (rad/s²)
- Rotational kinematic equations (analogous to linear):
  - $\omega = \omega_0 + \alpha t$
  - $\theta = \omega_0 t + \frac{1}{2}\alpha t^2$
  - $\omega^2 = \omega_0^2 + 2\alpha\theta$

### Rolling Motion
- Rolling without slipping: $v = \omega r$
- Total kinetic energy = translational + rotational: $E_k = \frac{1}{2}mv^2 + \frac{1}{2}I\omega^2$

### Angular Momentum
- $L = I\omega$ (for rotation about a fixed axis)
- Conservation of angular momentum: if no external torque, $I\omega = \text{constant}$
- Examples: ice skater spinning, collapsing star

### Equilibrium
- Static equilibrium: $\sum F = 0$ and $\sum \tau = 0$
- Conditions: no net force (translational) and no net torque (rotational)

## Key Equations

| Equation | Description |
|----------|-------------|
| $\tau = Fr\sin\theta$ | Torque |
| $\tau_{net} = I\alpha$ | Newton's second law for rotation |
| $I = \sum m_i r_i^2$ | Moment of inertia |
| $L = I\omega$ | Angular momentum |
| $E_{rot} = \frac{1}{2}I\omega^2$ | Rotational kinetic energy |
| $v = \omega r$ | Linear-angular velocity relationship |

## Common Misconceptions

1. **"Torque and force are the same"** -- Torque depends on both force and the distance from the pivot; the same force can produce different torques.
2. **"Heavier objects always have larger moments of inertia"** -- Moment of inertia depends on mass distribution, not just total mass.
3. **"Angular momentum is always conserved"** -- Only when no external torque acts on the system.
4. **"Rolling objects and sliding objects have the same speed at the bottom of a ramp"** -- Rolling objects are slower because energy is split between translational and rotational KE.

## Comparison with AP Physics

- AP Physics 1 covers rotational dynamics in **Units 5 and 6** with similar scope
- IB HL covers rigid body mechanics as a single integrated topic
- Both curricula cover torque, moment of inertia, and angular momentum conservation
- IB provides moment of inertia formulas in the data booklet; AP provides them on the equation sheet
