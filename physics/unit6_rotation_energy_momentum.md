# Unit 6: Energy and Momentum of Rotating Systems

> Exam Weight: 5--8% | ~8--12 Class Periods
>
> **CRITICAL TOPIC: Angular Momentum** -- This unit is particularly important for competition questions. Angular momentum conservation appears frequently in exam problems.

## Topics

### 6.1 Rotational Kinetic Energy
- Rotational kinetic energy: $K_{rot} = \frac{1}{2}I\omega^2$
- Mirrors the translational form $K = \frac{1}{2}mv^2$, with $I$ replacing $m$ and $\omega$ replacing $v$
- A rolling object carries two independent kinetic energy contributions: $K_{total} = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$
- The work-energy theorem extends naturally to rotating systems:
  $$K_i + U_i = K_f + U_f$$
  where $K$ must include every form of kinetic energy present, both translational and rotational

### 6.2 Torque and Work
- Work done by torque: $W = \tau \Delta\theta$ (for constant torque)
- This parallels $W = F \Delta x$: angular displacement replaces linear displacement, torque replaces force
- Work-energy theorem for rotation: $W_{net} = \Delta K_{rot} = \frac{1}{2}I\omega_f^2 - \frac{1}{2}I\omega_i^2$
- Power delivered by torque: $P = \tau\omega$

### 6.3 Angular Momentum and Angular Impulse
- **Angular momentum of a rigid body: $L = I\omega$**
- **Angular momentum of a point particle: $L = mvr\sin\theta = mvr_\perp$**
  - $r_\perp$ is the perpendicular distance from the chosen axis to the particle's line of motion
  - equivalently: $L = pr_\perp = mvr_\perp$
- Angular momentum carries a sign based on the direction of rotation:
  - CCW rotation $\Rightarrow$ positive $L$ (by right-hand rule convention)
  - CW rotation $\Rightarrow$ negative $L$
- **Angular impulse** describes how a torque acting over time alters angular momentum: $\Delta L = \tau_{avg} \Delta t$
- The generalized form of Newton's second law in angular terms: $\tau_{net} = \frac{\Delta L}{\Delta t}$
- The angular momentum of a multi-body system is the sum of each part's contribution: $L_{sys} = \sum L_i = \sum I_i\omega_i$

### 6.4 Conservation of Angular Momentum
- **When the net external torque on a system is zero, total angular momentum cannot change:**
$$L_i = L_f$$
$$I_i\omega_i = I_f\omega_f$$
- Angular momentum conservation ranks among the most broadly applicable principles in physics
- Illustrative scenarios:
  - **Figure skater pulling arms in**: reducing $I$ forces $\omega$ to increase so that $L$ stays constant
  - **Neutron star formation**: gravitational collapse shrinks $I$ dramatically, causing the star to spin orders of magnitude faster
  - **Person on a rotating platform catching a ball**: the total angular momentum of person + ball + platform is unchanged throughout
  - **Satellite in elliptical orbit**: $L = mvr$ remains fixed at every point because gravity, a central force, produces no torque about the orbital center
- **Critical distinction**: angular momentum is conserved whenever $\tau_{ext} = 0$ — external forces alone are not sufficient to change $L$ unless they produce a net torque (e.g., gravity toward a central body exerts no torque about that center)

### 6.5 Rolling Motion
- Rolling without slipping condition: $v_{cm} = R\omega$
- Applying energy conservation to an object rolling from rest down a slope:
  $$mgh = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$$
- Objects whose rotational inertia is a smaller fraction of $mR^2$ convert more potential energy into translational motion, so they roll faster
- Speed ranking at the bottom of an incline (fastest to slowest): sliding block > solid sphere > solid cylinder > hollow sphere > hollow cylinder (hoop)
- Static friction at the contact point supplies the torque that sustains rolling; because the contact point is instantaneously at rest, static friction does no work

### 6.6 Orbiting and Kepler's Laws (connection)
- Orbital motion is sustained because gravity continuously redirects the satellite's velocity toward the central body, acting as the centripetal force
- Because gravity points through the orbital center, it exerts zero torque there, so angular momentum is conserved throughout the orbit
- $L = mvr$ holds constant at every orbital position
- This constancy directly explains Kepler's second law: an orbiting body sweeps out equal areas in equal time intervals

## Skills to Master

- Determine the rotational kinetic energy of spinning objects and of objects that both roll and translate
- Use energy conservation in scenarios where rotational kinetic energy must be included
- Find the work contributed by a torque acting through an angular displacement
- **Evaluate angular momentum for a spinning rigid body ($L = I\omega$) and for a point particle in motion ($L = mvr_\perp$)**
- **Predict how angular velocity changes when the moment of inertia shifts, using conservation of angular momentum**
- Decide whether a given situation conserves angular momentum by identifying any external torques
- Tackle rolling-motion problems through energy methods
- Find the speed of an object reaching the base of an incline while rolling without slipping
- Relate orbital behavior to angular momentum conservation and trace the connection to Kepler's second law

## Core Concepts

1. A spinning object stores rotational kinetic energy equal to $\frac{1}{2}I\omega^2$; when an object rolls, it carries both this rotational term and a translational term simultaneously
2. A torque performing work over an angular displacement contributes energy equal to $\tau\Delta\theta$
3. **Angular momentum ($L = I\omega$ for rigid bodies) occupies the same position in rotational physics that linear momentum ($p = mv$) occupies in translational physics**
4. **A torque sustained over a time interval delivers an angular impulse equal to $\tau\Delta t$, producing a corresponding change in angular momentum — exactly analogous to how linear impulse changes linear momentum**
5. **In the absence of a net external torque, a system's total angular momentum remains unchanged**
6. **If rotational inertia decreases while no external torque acts, the angular velocity must increase proportionally to hold $L$ constant — and vice versa**
7. Rolling without slipping requires the geometric constraint $v_{cm} = R\omega$; static friction at the contact point generates the torque needed without dissipating energy
8. Orbiting bodies conserve angular momentum because the central gravitational force always passes through the reference point, contributing zero torque
9. **Angular momentum conservation and energy conservation are separate, independent laws** — an inelastic rotational collision, for example, preserves angular momentum while allowing kinetic energy to decrease

## Key Equations

### Rotational Kinetic Energy

$$K_{rot} = \frac{1}{2}I\omega^2$$

$$K_{total} = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2 \quad \text{(rolling)}$$

### Work by Torque

$$W = \tau\Delta\theta$$

$$P = \tau\omega$$

### Angular Momentum

$$L = I\omega \quad \text{(rigid body about fixed axis)}$$

$$L = mvr\sin\theta = mvr_\perp \quad \text{(point particle)}$$

### Angular Impulse

$$\Delta L = \tau_{avg} \Delta t$$

$$\tau_{net} = \frac{\Delta L}{\Delta t}$$

### Conservation of Angular Momentum

$$L_i = L_f \quad \text{(when } \sum\tau_{ext} = 0\text{)}$$

$$I_i\omega_i = I_f\omega_f$$

### Rolling Without Slipping

$$v_{cm} = R\omega$$

$$a_{cm} = R\alpha$$

### Energy Conservation with Rotation

$$mgh = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2 \quad \text{(rolling from rest)}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Angular momentum ($L$)** | The rotational counterpart of linear momentum; computed as $L = I\omega$ for a rigid body or $L = mvr_\perp$ for a point particle |
| **Angular impulse** | The accumulated effect of a torque over a time interval; quantitatively equal to the resulting change in angular momentum |
| **Rotational kinetic energy** | The kinetic energy stored in rotational motion, given by $K_{rot} = \frac{1}{2}I\omega^2$ |
| **Rolling without slipping** | A mode of motion where the geometric constraint $v_{cm} = R\omega$ holds; the contact point between object and surface has zero instantaneous velocity |
| **Conservation of angular momentum** | The principle that total angular momentum of an isolated (zero-net-external-torque) system stays constant over time |
| **Right-hand rule** | A sign convention for rotational vectors: wrap the right hand's fingers in the rotation direction and the extended thumb indicates the direction of $\vec{L}$ and $\vec{\omega}$ |
| **Central force** | A force always directed along the line joining two objects; it exerts zero torque about the object it points toward |
| **Periapsis / Apoapsis** | The orbital point closest to / farthest from the central body in an elliptical orbit |

## Common Misconceptions

1. **Conservation of angular momentum and conservation of linear momentum are the same law** -- They are entirely independent principles. A system can satisfy one while violating the other, depending on the forces and torques present.
2. **Conserving angular momentum guarantees energy conservation** -- This is false. When a figure skater pulls her arms inward, angular momentum is conserved but kinetic energy rises because her muscles do internal work on the system.
3. **$L = I\omega$ is the universal formula for angular momentum** -- This expression applies only to rigid bodies spinning about a fixed axis. For a point particle in motion, the correct expression is $L = mvr_\perp$.
4. **Angular momentum requires something to be spinning** -- A particle traveling in a straight line possesses nonzero angular momentum about any reference point that does not lie on that line, since $L = mvr_\perp \neq 0$ whenever $r_\perp \neq 0$.
5. **A rolling object and a frictionless sliding object reach the bottom of a ramp together** -- Rolling objects are always slower at the bottom, because part of the initial gravitational potential energy is diverted into rotational kinetic energy rather than translational kinetic energy.
6. **Friction always removes mechanical energy from a system** -- Static friction acting at the contact point of a rolling object does zero work because that point has no instantaneous velocity; it supplies a torque without any energy cost.
7. **Every net force on an object produces a torque** -- A force generates torque only if it has a component perpendicular to the position vector from the chosen axis. A force aimed directly through the axis produces zero torque.
8. **$I_i\omega_i = I_f\omega_f$ always means $\omega$ rises when $I$ drops** -- This relationship holds only when no net external torque is present. If external torques act, the correct tool is $\tau_{net} = \frac{\Delta L}{\Delta t}$, and $\omega$ may change differently.

## Angular Momentum Problem-Solving Strategy

1. **Specify the system boundary** — decide which objects are inside the system before writing any equations
2. **Choose the axis of rotation** — pick an axis that simplifies the geometry, often where unknown forces act
3. **Assess net external torque** about the chosen axis
   - $\sum\tau_{ext} = 0$: angular momentum is conserved; proceed to step 4
   - $\sum\tau_{ext} \neq 0$: angular momentum changes; apply $\Delta L = \tau_{avg}\Delta t$
4. **Compute $L$ at each relevant instant** using the appropriate expression — $I\omega$ for a spinning rigid body, $mvr_\perp$ for a point particle
5. **Write the conservation equation $L_i = L_f$** and isolate the target unknown

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Angular momentum | kg$\cdot$m$^2$/s = N$\cdot$m$\cdot$s | [M][L]$^2$[T]$^{-1}$ |
| Angular impulse | N$\cdot$m$\cdot$s | [M][L]$^2$[T]$^{-1}$ |
| Rotational KE | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Work (rotational) | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Torque | N$\cdot$m | [M][L]$^2$[T]$^{-2}$ |
| Power | W (watt) | [M][L]$^2$[T]$^{-3}$ |
