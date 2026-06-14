# Unit 7: Oscillations

> Exam Weight: 5--8% | ~8--12 Class Periods

## Topics

### 7.1 Defining Simple Harmonic Motion (SHM)
- Simple harmonic motion describes any oscillation in which the restoring force varies in direct proportion to how far the object has moved from its equilibrium point
- For a spring-mass system: $F = -k\Delta x$ (Hooke's Law as restoring force)
  - Leads to: $a = -\frac{k}{m}\Delta x$
- For a simple pendulum (small angle approximation $\sin\theta \approx \theta$):
  - Restoring force component: $F \approx -mg\theta = -\frac{mg}{L}s$
  - Leads to: $a \approx -\frac{g}{L}s$
- SHM requires two conditions: the restoring force must scale linearly with displacement and must always point back toward equilibrium
- When these conditions hold, the resulting motion traces out a sinusoidal pattern for position, velocity, and acceleration over time

### 7.2 Frequency and Period of SHM
- Period ($T$): the duration of one full oscillation cycle
- Frequency ($f$): how many complete cycles occur each second; $f = \frac{1}{T}$
- Angular frequency: $\omega = 2\pi f = \frac{2\pi}{T}$
- **Spring-mass system period**:
$$T_s = 2\pi\sqrt{\frac{m}{k}}$$
  - Set by the attached mass and the stiffness of the spring
  - Changing the amplitude or the local gravitational field has no effect on the period
- **Simple pendulum period** (small angle):
$$T_p = 2\pi\sqrt{\frac{L}{g}}$$
  - Controlled by the pendulum's length and the local value of $g$
  - Neither the bob's mass nor the swing amplitude (when small) alters the period

### 7.3 Representing and Analyzing SHM
- Position: $x(t) = A\cos(\omega t + \phi)$ or $x(t) = A\sin(\omega t + \phi)$
- Velocity: $v(t) = -A\omega\sin(\omega t + \phi)$; maximum at equilibrium: $v_{max} = A\omega$
- Acceleration: $a(t) = -A\omega^2\cos(\omega t + \phi)$; maximum at extremes: $a_{max} = A\omega^2$
- At the equilibrium point: $x = 0$, speed reaches its peak $|v| = v_{max}$, and $a = 0$
- At the turnaround points (amplitude): $x = \pm A$, the object momentarily stops ($v = 0$), and acceleration peaks at $|a| = a_{max}$
- Energy in SHM:
  - $E_{total} = \frac{1}{2}kA^2$ (constant, depends on amplitude)
  - At any position: $\frac{1}{2}kA^2 = \frac{1}{2}mv^2 + \frac{1}{2}k(\Delta x)^2$
  - Kinetic and potential energy exchange continuously, but mechanical energy as a whole stays fixed throughout the motion
  - KE peaks at equilibrium while PE peaks at the extremes of displacement

## Skills to Master

- Recognize the physical conditions that give rise to simple harmonic motion in a given system
- Articulate why a restoring force proportional to displacement leads to oscillatory behavior
- Compute period and frequency for spring-mass oscillators and small-angle pendulums
- Trace how position, velocity, and acceleration change as an object moves through one full cycle
- Use energy conservation principles to solve for unknowns in SHM problems
- Interpret and construct graphs of $x$, $v$, and $a$ as functions of time for oscillating systems
- Predict how altering mass, spring stiffness, string length, or oscillation amplitude shifts the period
- Leverage energy methods to derive peak speed or maximum displacement without kinematics equations

## Core Concepts

1. An oscillating system exhibits SHM whenever the net restoring force on it points toward equilibrium and its magnitude is directly proportional to the displacement
2. How quickly a spring-mass system oscillates is governed entirely by the mass and the spring constant — the size of the oscillation (amplitude) has no influence on the period
3. A simple pendulum's period is fixed by the string length and the local gravitational acceleration; changing the mass or the swing angle (within the small-angle regime) leaves the period unchanged
4. The kinematic quantities in SHM — position, velocity, and acceleration — all follow sinusoidal time dependence, with each one shifted a quarter-cycle relative to the next
5. For an ideal (undamped) oscillator, total mechanical energy remains constant throughout the motion and scales with the square of the amplitude
6. The oscillator moves fastest as it passes through equilibrium and reaches zero speed at the extremes; conversely, acceleration is greatest at the extremes and vanishes at equilibrium
7. SHM can be understood geometrically as the one-dimensional shadow of an object moving at constant speed around a circle

## Key Equations

### Period and Frequency

$$T = \frac{1}{f}, \quad \omega = 2\pi f = \frac{2\pi}{T}$$

### Spring-Mass System

$$T_s = 2\pi\sqrt{\frac{m}{k}}$$

$$f_s = \frac{1}{2\pi}\sqrt{\frac{k}{m}}$$

### Simple Pendulum (Small Angle)

$$T_p = 2\pi\sqrt{\frac{L}{g}}$$

$$f_p = \frac{1}{2\pi}\sqrt{\frac{g}{L}}$$

### Position, Velocity, Acceleration

$$x(t) = A\cos(\omega t + \phi)$$

$$v(t) = -A\omega\sin(\omega t + \phi), \quad v_{max} = A\omega$$

$$a(t) = -A\omega^2\cos(\omega t + \phi), \quad a_{max} = A\omega^2$$

### Energy in SHM

$$E_{total} = \frac{1}{2}kA^2 = \frac{1}{2}mv_{max}^2$$

$$\frac{1}{2}kA^2 = \frac{1}{2}mv^2 + \frac{1}{2}k(\Delta x)^2$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Simple harmonic motion** | Oscillatory motion in which the restoring force is linearly proportional to displacement from equilibrium |
| **Amplitude ($A$)** | The greatest distance the oscillator travels from its equilibrium position during one cycle |
| **Period ($T$)** | The elapsed time required for the system to complete exactly one full oscillation |
| **Frequency ($f$)** | The count of complete oscillation cycles that occur within one second |
| **Angular frequency ($\omega$)** | $2\pi f$; represents how rapidly the phase of the oscillation advances, in radians per second |
| **Equilibrium position** | The location at which all forces on the oscillator cancel, serving as the center of the motion |
| **Restoring force** | A force whose direction always points toward equilibrium and whose magnitude grows in proportion to displacement |
| **Phase ($\phi$)** | A constant offset in the sinusoidal argument that encodes the oscillator's position and velocity at time $t = 0$ |
| **Damping** | The process by which non-conservative forces such as friction or air resistance steadily reduce the amplitude of oscillation over time |
| **Simple pendulum** | A theoretical model consisting of a concentrated point mass suspended by a massless, rigid, inextensible string |

## Common Misconceptions

1. **Amplitude affects the period** -- In ideal SHM, the period of both spring-mass systems and small-angle pendulums is completely independent of how large the oscillations are.
2. **Mass affects pendulum period** -- A pendulum's period is governed by length and $g$ alone; swapping the bob for a heavier one leaves the period unchanged.
3. **Acceleration is zero at maximum displacement** -- The opposite is true. Displacement is largest at the turning points, so the restoring force — and therefore the acceleration — is at its peak there. Velocity, not acceleration, is zero at those instants.
4. **Velocity is zero at equilibrium** -- Also backwards. As the oscillator passes through equilibrium, the restoring force is zero and the object is moving at its highest speed; it is the acceleration, not the velocity, that is zero at that point.
5. **SHM and circular motion are unrelated** -- They are intimately connected: SHM is mathematically equivalent to the projection of uniform circular motion onto any single diameter of the circle.
6. **A heavier mass on a spring oscillates slower** -- This is correct ($T \propto \sqrt{m}$), but the same reasoning does not transfer to pendulums, where mass cancels out of the period formula entirely.
7. **The pendulum period formula is universally valid** -- The formula $T_p = 2\pi\sqrt{L/g}$ relies on the small-angle approximation and loses accuracy for angles roughly above $15°$.
8. **Total energy of a spring system depends on mass** -- The stored energy $E = \frac{1}{2}kA^2$ is set by the spring constant and the amplitude; mass does not appear in this expression.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Period | s (second) | [T] |
| Frequency | Hz (hertz) = s$^{-1}$ | [T]$^{-1}$ |
| Angular frequency | rad/s | [T]$^{-1}$ |
| Amplitude | m (meter) | [L] |
| Spring constant | N/m | [M][T]$^{-2}$ |
| Energy | J (joule) | [M][L]$^2$[T]$^{-2}$ |
