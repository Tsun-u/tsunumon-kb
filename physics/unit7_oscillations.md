# Unit 7: Oscillations

> Exam Weight: 5--8% | ~8--12 Class Periods

## Topics

### 7.1 Defining Simple Harmonic Motion (SHM)
- Simple harmonic motion: periodic motion where the restoring force is proportional to displacement from equilibrium
- For a spring-mass system: $F = -k\Delta x$ (Hooke's Law as restoring force)
  - Leads to: $a = -\frac{k}{m}\Delta x$
- For a simple pendulum (small angle approximation $\sin\theta \approx \theta$):
  - Restoring force component: $F \approx -mg\theta = -\frac{mg}{L}s$
  - Leads to: $a \approx -\frac{g}{L}s$
- Conditions for SHM: restoring force proportional to displacement, directed toward equilibrium
- SHM produces sinusoidal position, velocity, and acceleration as functions of time

### 7.2 Frequency and Period of SHM
- Period ($T$): time for one complete oscillation
- Frequency ($f$): number of oscillations per unit time; $f = \frac{1}{T}$
- Angular frequency: $\omega = 2\pi f = \frac{2\pi}{T}$
- **Spring-mass system period**:
$$T_s = 2\pi\sqrt{\frac{m}{k}}$$
  - Depends on mass and spring constant
  - Does NOT depend on amplitude or gravity
- **Simple pendulum period** (small angle):
$$T_p = 2\pi\sqrt{\frac{L}{g}}$$
  - Depends on length and gravitational acceleration
  - Does NOT depend on mass or amplitude (for small angles)

### 7.3 Representing and Analyzing SHM
- Position: $x(t) = A\cos(\omega t + \phi)$ or $x(t) = A\sin(\omega t + \phi)$
- Velocity: $v(t) = -A\omega\sin(\omega t + \phi)$; maximum at equilibrium: $v_{max} = A\omega$
- Acceleration: $a(t) = -A\omega^2\cos(\omega t + \phi)$; maximum at extremes: $a_{max} = A\omega^2$
- At equilibrium: $x = 0$, $|v| = v_{max}$, $a = 0$
- At maximum displacement (amplitude): $x = \pm A$, $v = 0$, $|a| = a_{max}$
- Energy in SHM:
  - $E_{total} = \frac{1}{2}kA^2$ (constant, depends on amplitude)
  - At any position: $\frac{1}{2}kA^2 = \frac{1}{2}mv^2 + \frac{1}{2}k(\Delta x)^2$
  - KE and PE oscillate but total energy remains constant
  - KE maximum at equilibrium; PE maximum at extremes

## Learning Objectives

- Identify systems that undergo simple harmonic motion
- Explain the role of the restoring force in producing SHM
- Calculate the period and frequency of spring-mass systems and simple pendulums
- Describe how position, velocity, and acceleration vary during SHM
- Apply energy conservation to SHM systems
- Analyze graphs of position, velocity, and acceleration vs. time for SHM
- Determine the effect of changing mass, spring constant, length, or amplitude on period
- Use energy methods to find maximum speed or maximum displacement

## Essential Knowledge

1. SHM occurs when a restoring force is proportional to and opposite the displacement from equilibrium
2. The period of a spring-mass system depends on mass and spring constant, not amplitude
3. The period of a simple pendulum depends on length and gravitational acceleration, not mass or amplitude (small angle)
4. Position, velocity, and acceleration in SHM are sinusoidal functions of time, each 90 degrees out of phase
5. Total mechanical energy in SHM is constant (for ideal systems) and proportional to amplitude squared
6. Maximum speed occurs at equilibrium; maximum acceleration occurs at maximum displacement
7. SHM is the projection of uniform circular motion onto one axis

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
| **Simple harmonic motion** | Periodic motion with restoring force proportional to displacement |
| **Amplitude ($A$)** | Maximum displacement from equilibrium |
| **Period ($T$)** | Time for one complete oscillation cycle |
| **Frequency ($f$)** | Number of complete oscillations per second |
| **Angular frequency ($\omega$)** | $2\pi f$; rate of change of phase angle |
| **Equilibrium position** | Position where net force is zero; center of oscillation |
| **Restoring force** | Force directed toward equilibrium, proportional to displacement |
| **Phase ($\phi$)** | Initial angle that determines starting position of oscillation |
| **Damping** | Gradual decrease in amplitude due to non-conservative forces (e.g., friction, air resistance) |
| **Simple pendulum** | Idealized pendulum: point mass on a massless, inextensible string |

## Common Misconceptions

1. **Amplitude affects the period** -- For ideal SHM (spring-mass and small-angle pendulum), period is independent of amplitude.
2. **Mass affects pendulum period** -- The period of a simple pendulum does NOT depend on mass. Only length and $g$ matter.
3. **Acceleration is zero at maximum displacement** -- FALSE. Acceleration is MAXIMUM at maximum displacement (where restoring force is maximum). Velocity is zero there.
4. **Velocity is zero at equilibrium** -- FALSE. Velocity is MAXIMUM at equilibrium. Acceleration is zero there.
5. **SHM and circular motion are unrelated** -- SHM is the projection of uniform circular motion onto a diameter.
6. **A heavier mass on a spring oscillates slower** -- True ($T \propto \sqrt{m}$), but students sometimes confuse this with pendulums where mass doesn't matter.
7. **The period formula for a pendulum works for all angles** -- Only valid for small angles (typically $\theta < 15°$).
8. **Total energy depends on mass for a spring** -- Total energy $E = \frac{1}{2}kA^2$ depends on spring constant and amplitude, not directly on mass.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Period | s (second) | [T] |
| Frequency | Hz (hertz) = s$^{-1}$ | [T]$^{-1}$ |
| Angular frequency | rad/s | [T]$^{-1}$ |
| Amplitude | m (meter) | [L] |
| Spring constant | N/m | [M][T]$^{-2}$ |
| Energy | J (joule) | [M][L]$^2$[T]$^{-2}$ |
