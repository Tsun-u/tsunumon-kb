# Unit 6: Energy and Momentum of Rotating Systems

> Exam Weight: 5--8% | ~8--12 Class Periods
>
> **CRITICAL TOPIC: Angular Momentum** -- This unit is particularly important for competition questions. Angular momentum conservation appears frequently in exam problems.

## Topics

### 6.1 Rotational Kinetic Energy
- Rotational kinetic energy: $K_{rot} = \frac{1}{2}I\omega^2$
- Analogous to translational $K = \frac{1}{2}mv^2$
- Total kinetic energy of a rolling object: $K_{total} = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$
- Energy conservation applies to systems with rotation:
  $$K_i + U_i = K_f + U_f$$
  where $K$ includes both translational and rotational components

### 6.2 Torque and Work
- Work done by torque: $W = \tau \Delta\theta$ (for constant torque)
- Analogous to $W = F \Delta x$
- Work-energy theorem for rotation: $W_{net} = \Delta K_{rot} = \frac{1}{2}I\omega_f^2 - \frac{1}{2}I\omega_i^2$
- Power delivered by torque: $P = \tau\omega$

### 6.3 Angular Momentum and Angular Impulse
- **Angular momentum of a rigid body: $L = I\omega$**
- **Angular momentum of a point particle: $L = mvr\sin\theta = mvr_\perp$**
  - where $r_\perp$ is the perpendicular distance from the axis to the line of motion
  - equivalently: $L = pr_\perp = mvr_\perp$
- Angular momentum is a vector:
  - CCW rotation $\Rightarrow$ positive $L$ (by right-hand rule convention)
  - CW rotation $\Rightarrow$ negative $L$
- **Angular impulse**: $\Delta L = \tau_{avg} \Delta t$
- Newton's second law in angular momentum form: $\tau_{net} = \frac{\Delta L}{\Delta t}$
- Total angular momentum of a system: $L_{sys} = \sum L_i = \sum I_i\omega_i$

### 6.4 Conservation of Angular Momentum
- **If the net external torque on a system is zero, the total angular momentum is conserved:**
$$L_i = L_f$$
$$I_i\omega_i = I_f\omega_f$$
- This is one of the fundamental conservation laws in physics
- Classic examples:
  - **Figure skater pulling arms in**: $I$ decreases, $\omega$ increases (spins faster)
  - **Neutron star formation**: collapsing star decreases $I$, dramatically increases $\omega$
  - **Person on rotating platform catching a ball**: system $L$ is conserved
  - **Satellite in elliptical orbit**: at periapsis $r$ is small so $v$ is large; at apoapsis $r$ is large so $v$ is small ($L = mvr$ = constant for central force)
- **KEY DISTINCTION**: Angular momentum is conserved when $\tau_{ext} = 0$, even if external FORCES exist (e.g., gravity as a central force produces zero torque about the center)

### 6.5 Rolling Motion
- Rolling without slipping condition: $v_{cm} = R\omega$
- For rolling down an incline, energy conservation gives:
  $$mgh = \frac{1}{2}mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$$
- Objects with smaller $I$ (relative to $mR^2$) roll faster down inclines
- Ranking for rolling down incline (fastest to slowest): sliding block > solid sphere > solid cylinder > hollow sphere > hollow cylinder (hoop)
- Static friction provides the torque for rolling (without doing work, since contact point has zero velocity)

### 6.6 Orbiting and Kepler's Laws (connection)
- For a satellite in orbit, gravitational force provides centripetal force
- Angular momentum is conserved for orbiting bodies (gravity exerts zero torque about the center)
- $L = mvr$ is constant at all points in the orbit
- This leads to Kepler's second law: equal areas swept in equal times

## Learning Objectives

- Calculate rotational kinetic energy for spinning and rolling objects
- Apply energy conservation including rotational kinetic energy
- Calculate work done by a torque
- **Define and calculate angular momentum for rigid bodies ($L = I\omega$) and point particles ($L = mvr_\perp$)**
- **Apply conservation of angular momentum to predict changes in angular velocity when moment of inertia changes**
- Determine whether angular momentum is conserved in a given scenario by analyzing external torques
- Analyze rolling motion using energy methods
- Solve problems involving objects rolling down inclines
- Connect angular momentum conservation to orbital mechanics

## Essential Knowledge

1. Rotational kinetic energy is $\frac{1}{2}I\omega^2$; a rolling object has both translational and rotational KE
2. Work done by a torque equals $\tau\Delta\theta$
3. **Angular momentum ($L = I\omega$) is the rotational analog of linear momentum ($p = mv$)**
4. **Angular impulse ($\tau\Delta t$) changes angular momentum, just as linear impulse changes linear momentum**
5. **When no net external torque acts on a system, angular momentum is conserved**
6. **When $I$ changes in a system with no external torque, $\omega$ changes inversely to keep $L$ constant**
7. For rolling without slipping, $v_{cm} = R\omega$ and static friction acts at the contact point
8. Angular momentum is conserved for objects in orbit around a central body (gravity produces no torque about the center)
9. **Angular momentum conservation is INDEPENDENT of energy conservation** -- energy may not be conserved (e.g., inelastic rotational collision) while angular momentum IS conserved

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
| **Angular momentum ($L$)** | Rotational analog of linear momentum; $L = I\omega$ for rigid bodies, $L = mvr_\perp$ for point particles |
| **Angular impulse** | Product of torque and time interval; equals change in angular momentum |
| **Rotational kinetic energy** | Energy due to rotation; $K_{rot} = \frac{1}{2}I\omega^2$ |
| **Rolling without slipping** | Condition where $v_{cm} = R\omega$; no relative sliding at contact point |
| **Conservation of angular momentum** | Total angular momentum remains constant when no net external torque acts |
| **Right-hand rule** | Convention: curl fingers in direction of rotation; thumb points in direction of $\vec{L}$ and $\vec{\omega}$ |
| **Central force** | Force directed along the line connecting two objects; produces zero torque about the center |
| **Periapsis / Apoapsis** | Closest / farthest point in an elliptical orbit |

## Common Misconceptions

1. **Angular momentum and linear momentum are the same conservation law** -- No. They are independent. A system can conserve one without conserving the other.
2. **If angular momentum is conserved, energy must also be conserved** -- FALSE. Example: a figure skater pulls arms in (angular momentum conserved, but KE increases because internal muscular work is done).
3. **$L = I\omega$ always applies** -- Only for rigid bodies rotating about a fixed axis. For a point particle, use $L = mvr_\perp$.
4. **Angular momentum is only about rotation** -- A particle moving in a straight line has angular momentum about any point not on its line of motion! $L = mvr_\perp \neq 0$.
5. **Objects rolling down an incline reach the bottom at the same time as sliding objects** -- No. Rolling objects are slower because some potential energy goes to rotational KE.
6. **Friction always dissipates energy** -- Static friction in rolling does no work (contact point has zero velocity). It provides torque without dissipating energy.
7. **A net force always produces a torque** -- Only if the force has a component perpendicular to the position vector from the axis. A force directed through the axis produces zero torque.
8. **$I_i\omega_i = I_f\omega_f$ means $\omega$ always increases when $I$ decreases** -- Only when no external torque acts. If external torque exists, use $\tau = \frac{\Delta L}{\Delta t}$ instead.

## Angular Momentum Problem-Solving Strategy

1. **Define the system** clearly
2. **Identify the axis of rotation**
3. **Check for external torques** about that axis
   - If $\sum\tau_{ext} = 0$: angular momentum is conserved
   - If $\sum\tau_{ext} \neq 0$: use $\Delta L = \tau\Delta t$
4. **Calculate $L$ before and after** using appropriate formula ($I\omega$ or $mvr_\perp$)
5. **Set $L_i = L_f$** and solve for the unknown

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Angular momentum | kg$\cdot$m$^2$/s = N$\cdot$m$\cdot$s | [M][L]$^2$[T]$^{-1}$ |
| Angular impulse | N$\cdot$m$\cdot$s | [M][L]$^2$[T]$^{-1}$ |
| Rotational KE | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Work (rotational) | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Torque | N$\cdot$m | [M][L]$^2$[T]$^{-2}$ |
| Power | W (watt) | [M][L]$^2$[T]$^{-3}$ |
