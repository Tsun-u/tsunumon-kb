# Unit 14: Waves, Sound, and Physical Optics

> Exam Weight: 12--15% | ~14--23 Class Periods

## Topics

### 14.1 Properties of Wave Pulses and Waves
- A wave is a traveling disturbance that carries energy from one place to another while the medium's particles stay put, oscillating around their resting positions
- **Transverse waves**: each particle moves at right angles to the wave's travel direction (e.g., vibrating strings, electromagnetic radiation)
- **Longitudinal waves**: each particle moves back and forth along the same line as the wave travels (e.g., sound, a compressed spring)
- **Mechanical waves** need a physical medium to propagate (sound, ocean waves); **electromagnetic waves** travel through vacuum and require no medium (light, radio)
- Amplitude ($A$): how far a particle strays from equilibrium at its greatest displacement
- Wavelength ($\lambda$): the spatial period of the wave — the distance from one point to the next identical point one cycle ahead (e.g., crest to crest)
- Frequency ($f$): the number of full oscillation cycles completed each second
- Period ($T$): the duration of one complete cycle; $T = \frac{1}{f}$
- The universal wave equation relates speed, frequency, and wavelength:

$$v = f \lambda$$

### 14.2 Periodic Waves
- A continuously repeating (sinusoidal) wave is described mathematically by:

$$y(x, t) = A \sin(kx - \omega t)$$

- Wave number: $k = \frac{2\pi}{\lambda}$ quantifies how rapidly the wave oscillates in space (rad/m)
- Angular frequency: $\omega = 2\pi f = \frac{2\pi}{T}$ quantifies how rapidly it oscillates in time (rad/s)
- Wave speed can be expressed compactly as $v = \frac{\omega}{k}$
- The speed at which a transverse wave travels along a taut string is set by the string's tension $F_T$ and its linear mass density $\mu$ (mass per unit length):

$$v = \sqrt{\frac{F_T}{\mu}}$$

- Greater tension accelerates the wave; greater linear density slows it down
- A wave's speed through a given medium is fixed by that medium's characteristics, not by the source that creates the wave

### 14.3 Boundary Behavior of Waves and Polarization
- A pulse hitting a **fixed (rigid) boundary** bounces back flipped — the reflected pulse is inverted relative to the incident pulse (180° phase change)
- A pulse hitting a **free (open) boundary** bounces back in the same orientation — the reflected pulse is upright (no phase change)
- When a wave reaches an interface between two different media, part of it transmits into the second medium and part reflects back
- Transitioning from a less dense to a more dense medium: the reflected portion is inverted
- Transitioning from a more dense to a less dense medium: the reflected portion is upright
- **Polarization** is a feature of transverse waves only; because longitudinal wave oscillations run parallel to propagation, they cannot be polarized
- An unpolarized transverse wave contains vibrations in every orientation perpendicular to the direction of travel
- A polarizing filter selects and transmits only the oscillation component aligned with its transmission axis, blocking the rest
- **Malus's law**: when already-polarized light of intensity $I_0$ encounters a polarizer whose axis is tilted by angle $\theta$ from the light's polarization direction:

$$I = I_0 \cos^2\theta$$

- Completely unpolarized light loses exactly half its intensity when it passes through an ideal polarizer: $I = \frac{1}{2} I_0$

### 14.4 Electromagnetic Waves
- An electromagnetic wave is a coupled pair of oscillating electric ($\vec{E}$) and magnetic ($\vec{B}$) fields; the two fields are mutually perpendicular and both are perpendicular to the wave's direction of travel
- In vacuum, all electromagnetic waves share the same speed:

$$c = 3.00 \times 10^8 \text{ m/s}$$

- Arranged from lowest to highest frequency (equivalently, longest to shortest wavelength), the EM spectrum runs: radio, microwave, infrared, visible light, ultraviolet, X-ray, gamma ray
- The human eye responds to wavelengths from roughly $400 \text{ nm}$ (violet) through $700 \text{ nm}$ (red)
- Accelerating electric charges are the source of all electromagnetic radiation
- EM waves transport both energy and momentum, and propagate through empty space without any medium
- Inside a transparent material with refractive index $n$, light slows to $v = \frac{c}{n}$

### 14.5 The Doppler Effect
- The Doppler effect refers to the shift in detected frequency that occurs whenever a wave source and an observer are moving relative to each other
- For sound, when the source and/or observer move along the line joining them:

$$f_{\text{obs}} = f_{\text{source}} \cdot \frac{v \pm v_{\text{obs}}}{v \mp v_{\text{source}}}$$

- Sign selection rule: choose upper signs when the source and observer close the gap between them; choose lower signs when they move apart
  - Observer moving toward the source: $+v_{\text{obs}}$ in the numerator raises the detected frequency
  - Source moving toward the observer: $-v_{\text{source}}$ in the denominator also raises the detected frequency
- Closing gap between source and observer: the detected frequency is **higher** than the emitted frequency
- Widening gap between source and observer: the detected frequency is **lower** than the emitted frequency
- The Doppler shift is a general wave phenomenon, but the formula above is specific to mechanical waves like sound; light requires a relativistic version

### 14.6 Wave Interference and Standing Waves
- **Principle of superposition**: the displacement at any point where two or more waves coexist equals the algebraic sum of the contributions from each wave individually
- **Constructive interference**: when waves arrive with a path difference of $m\lambda$ (where $m = 0, 1, 2, \ldots$) they are in phase and their amplitudes reinforce each other
- **Destructive interference**: when waves arrive with a path difference of $(m + \tfrac{1}{2})\lambda$ they are out of phase and their amplitudes cancel
- **Standing waves** emerge from the superposition of two waves with the same amplitude and frequency travelling in opposite directions through the same medium
- **Nodes**: specific locations that never move — the two travelling waves cancel there at every instant
- **Antinodes**: locations that swing with the greatest amplitude, halfway between successive nodes
- Consecutive nodes (or consecutive antinodes) are spaced exactly $\frac{\lambda}{2}$ apart
- Resonant harmonics for a string anchored at both ends (length $L$):

$$\lambda_n = \frac{2L}{n}, \quad f_n = n f_1 = \frac{n v}{2L} \quad (n = 1, 2, 3, \ldots)$$

- **Open pipe** (open at both ends) — antinodes form at both ends, giving the same harmonic series as a string:

$$f_n = \frac{n v}{2L} \quad (n = 1, 2, 3, \ldots)$$

- **Closed pipe** (one end sealed, one end open) — a node is required at the closed end and an antinode at the open end; only odd harmonics fit this constraint:

$$f_n = \frac{n v}{4L} \quad (n = 1, 3, 5, \ldots)$$

- Memory aid: a rigid (closed) end forces a displacement node; a free (open) end allows a displacement antinode

### 14.7 Diffraction
- Diffraction is the phenomenon by which waves bend around edges and spread into regions that geometric straight-line propagation would leave in shadow
- The effect is most pronounced when the opening or obstacle has a size comparable to the wave's wavelength; much larger obstacles cast relatively sharp shadows
- **Single-slit diffraction** creates a pattern dominated by a bright central region that is twice the angular width of the secondary maxima on either side
- Dark fringes (minima) in the single-slit pattern for a slit of width $a$ occur where:

$$a \sin\theta = m\lambda \quad (m = \pm 1, \pm 2, \pm 3, \ldots)$$

- Note: $m = 0$ corresponds to the bright central maximum, not a dark fringe
- An inverse relationship holds: shrinking the slit width spreads the pattern, while widening the slit compresses it

### 14.8 Double-Slit Interference and Diffraction Gratings
- **Young's double-slit experiment** provided the first compelling evidence for the wave character of light by generating a clear interference pattern
- When two coherent sources separated by gap $d$ emit waves, the overlapping wavefronts create a pattern of alternating bright and dark bands
- Bright fringes form where waves arrive in phase (constructive interference, maxima):

$$d \sin\theta = m\lambda \quad (m = 0, \pm 1, \pm 2, \ldots)$$

- Dark fringes form where waves arrive half a cycle out of phase (destructive interference, minima):

$$d \sin\theta = \left(m + \frac{1}{2}\right)\lambda \quad (m = 0, \pm 1, \pm 2, \ldots)$$

- When the angles are small, the height on a screen placed a distance $L$ away of the $m$-th bright fringe is approximately:

$$y_m = \frac{m \lambda L}{d}$$

- A **diffraction grating** consists of a large number of equally spaced slits; it obeys the same maximum condition ($d \sin\theta = m\lambda$) as double-slit, but the many contributing slits make the bright fringes extremely sharp and narrow
- Adding more slits concentrates the bright fringes into narrower peaks while darkening the surrounding regions
- The key variable is the path-length difference between waves from neighboring slits; constructive interference requires this difference to be an integer multiple of the wavelength

### 14.9 Thin-Film Interference
- When light strikes a thin transparent film (thickness $t$, refractive index $n$), some reflects from the top surface and some from the bottom; these two reflected beams interfere because they have travelled different distances
- **Phase shift rule**: reflecting off a boundary that leads into a medium with a higher refractive index causes a 180° phase inversion; reflecting off a boundary into a lower-index medium causes no phase shift
- Inside the film, the effective wavelength shortens to $\lambda_n = \frac{\lambda}{n}$, where $\lambda$ is the vacuum wavelength
- The round-trip optical path difference for light traversing the film twice is $2nt$
- **When both surfaces produce the same phase behavior** (both shift or neither shifts), the net phase difference comes from path alone:
  - Constructive: $2nt = m\lambda \quad (m = 1, 2, 3, \ldots)$
  - Destructive: $2nt = \left(m + \frac{1}{2}\right)\lambda$
- **When exactly one surface introduces a phase shift** (the typical situation, e.g., a soap film surrounded by air), the extra half-cycle flips which condition gives which outcome:
  - Constructive: $2nt = \left(m + \frac{1}{2}\right)\lambda \quad (m = 0, 1, 2, \ldots)$
  - Destructive: $2nt = m\lambda \quad (m = 1, 2, 3, \ldots)$
- Practical examples include anti-reflection lens coatings, the swirling colors of soap bubbles and oil slicks, and Newton's rings

## Skills to Master

- Identify whether a wave is transverse or longitudinal and give a physical example of each type
- Connect wave speed, frequency, wavelength, and period through $v = f\lambda$ and $T = 1/f$
- Explain why wave speed is set by medium properties rather than the source
- Interpret and construct the sinusoidal wave function $y = A\sin(kx - \omega t)$, identifying each parameter's physical meaning
- Predict whether a reflected pulse is inverted or upright based on whether the boundary is fixed or free
- Use Malus's law to find the transmitted intensity when polarized light passes through a polarizer at a given angle
- Characterize electromagnetic waves and arrange the major regions of the EM spectrum in order of frequency or wavelength
- Compute the frequency heard by a moving observer or from a moving source using the Doppler formula
- Add wave displacements using the superposition principle to identify regions of constructive and destructive interference
- Calculate the allowed resonant frequencies for standing waves on strings, in open pipes, and in closed pipes
- Locate dark fringes in single-slit diffraction using the minimum condition
- Find bright and dark fringe positions for double-slit setups and diffraction gratings
- Solve thin-film interference problems by tracking both optical path difference and phase shifts at each reflecting surface

## Core Concepts

1. A wave carries energy from one location to another — through a medium in the case of mechanical waves, through space in the case of electromagnetic waves — while the particles of the medium merely oscillate about fixed positions
2. The speed of a mechanical wave is controlled by the medium's physical characteristics (for example, string wave speed depends on tension and linear mass density); electromagnetic waves in vacuum always travel at $c = 3.00 \times 10^8$ m/s
3. Four quantities — amplitude, wave number (or wavelength), angular frequency (or ordinary frequency), and initial phase — completely specify a sinusoidal wave
4. At any boundary, a wave splits into a reflected component and a transmitted component; whether the reflected portion undergoes a phase inversion depends on the mechanical properties of the boundary
5. Only transverse waves can be polarized, because only they have oscillation directions perpendicular to propagation; Malus's law quantifies how much intensity a polarizer passes
6. Relative motion between a wave source and an observer shifts the detected frequency upward when they approach and downward when they separate — this is the Doppler effect
7. When two identical waves travel through each other in opposite directions, their superposition produces a standing wave pattern with permanently stationary nodes and maximum-displacement antinodes
8. Waves spread into the geometric shadow of an aperture or obstacle when its size is comparable to the wavelength; this diffraction effect is most pronounced for single-slit geometry, where the central maximum is especially wide
9. Double-slit and diffraction-grating setups create alternating bright and dark fringes; the angular positions of these fringes are set by the ratio of wavelength to slit spacing
10. A thin film produces interference because light reflecting from the top and bottom surfaces travels different optical path lengths ($2nt$); the fringe pattern also depends on whether either reflection introduces a half-cycle phase shift

## Key Equations

### Universal Wave Equation

$$v = f\lambda = \frac{\lambda}{T}$$

### Sinusoidal Wave

$$y(x, t) = A \sin(kx - \omega t)$$

$$k = \frac{2\pi}{\lambda}, \quad \omega = 2\pi f = \frac{2\pi}{T}, \quad v = \frac{\omega}{k}$$

### Wave Speed on a String

$$v = \sqrt{\frac{F_T}{\mu}}$$

### Malus's Law

$$I = I_0 \cos^2\theta$$

### Doppler Effect (Sound)

$$f_{\text{obs}} = f_{\text{source}} \cdot \frac{v \pm v_{\text{obs}}}{v \mp v_{\text{source}}}$$

### Standing Waves -- String or Open Pipe

$$f_n = \frac{n v}{2L} \quad (n = 1, 2, 3, \ldots)$$

### Standing Waves -- Closed Pipe (one end closed)

$$f_n = \frac{n v}{4L} \quad (n = 1, 3, 5, \ldots)$$

### Single-Slit Diffraction Minima

$$a \sin\theta = m\lambda \quad (m = \pm 1, \pm 2, \pm 3, \ldots)$$

### Double-Slit / Diffraction Grating Maxima

$$d \sin\theta = m\lambda \quad (m = 0, \pm 1, \pm 2, \ldots)$$

### Double-Slit Minima

$$d \sin\theta = \left(m + \frac{1}{2}\right)\lambda \quad (m = 0, \pm 1, \pm 2, \ldots)$$

### Double-Slit Fringe Position (small angle)

$$y_m = \frac{m \lambda L}{d}$$

### Thin-Film Interference (one phase shift)

$$\text{Constructive: } 2nt = \left(m + \frac{1}{2}\right)\lambda \quad (m = 0, 1, 2, \ldots)$$

$$\text{Destructive: } 2nt = m\lambda \quad (m = 1, 2, 3, \ldots)$$

### Speed of Light in a Medium

$$v = \frac{c}{n}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Transverse wave** | A wave whose particles displace at right angles to the direction the wave travels (e.g., waves on a rope) |
| **Longitudinal wave** | A wave whose particles displace along the same direction the wave travels, creating compressions and rarefactions (e.g., sound) |
| **Amplitude** | The greatest displacement a particle reaches from its rest position; determines the energy carried by the wave |
| **Wavelength ($\lambda$)** | The distance over which the wave pattern repeats — equivalently, the gap between any two adjacent points that are in phase |
| **Frequency ($f$)** | How many complete cycles pass a fixed point every second; the SI unit is the hertz (Hz) |
| **Node** | A fixed location on a standing wave where the displacement is always zero because the interfering waves cancel completely |
| **Antinode** | A location on a standing wave that swings back and forth with the largest possible amplitude |
| **Superposition** | The rule that the total wave displacement at any point and time equals the sum of the individual wave displacements there |
| **Polarization** | A property describing which direction a transverse wave oscillates; an unpolarized wave oscillates with equal probability in every transverse direction |
| **Diffraction** | The tendency of waves to curve around edges and spread into the shadow region beyond an aperture or obstacle |
| **Interference** | The pattern of amplitude enhancement (constructive) or reduction (destructive) that results when two or more waves coexist in the same region |
| **Coherent sources** | Sources that emit waves with a fixed, stable phase relationship — a prerequisite for observing a steady interference pattern |
| **Index of refraction ($n$)** | A dimensionless ratio $n = c/v$ showing how much slower light travels in a medium compared with vacuum |
| **Optical path length** | The product of a ray's geometric path length and the refractive index of the medium it traverses ($n \cdot d$); relevant to thin-film calculations |
| **Harmonic** | One of the allowed resonant frequencies of a system; the $n$-th harmonic has frequency $f_n = n f_1$, where $f_1$ is the fundamental |

## Common Misconceptions

1. **Waves carry material along with them as they travel** -- Incorrect. Waves move energy from place to place, but each particle of the medium simply oscillates around a fixed equilibrium point and does not travel with the disturbance.
2. **A louder sound has a higher pitch** -- Incorrect. These are entirely separate attributes. Volume (loudness) reflects wave amplitude and intensity, while pitch reflects frequency. A very loud sound can have a low pitch, and a soft sound can have a high pitch.
3. **The Doppler effect means the source is emitting at a different frequency** -- Incorrect. The source continues to vibrate at exactly the same rate as before. What changes is the frequency that reaches the observer's ears or detector, due to the relative motion compressing or stretching the wave pattern in space.
4. **Diffraction is unique to light** -- Incorrect. All wave types — sound, water ripples, seismic waves, and light — diffract whenever they encounter an opening or object whose size is in the same range as the wavelength.
5. **Making a slit wider will spread the diffraction pattern wider** -- Incorrect. The relationship is inverted: a narrower slit diffracts more strongly and produces a broader central maximum. A wider slit produces a sharper, narrower pattern.
6. **Reflection from any surface always shifts the phase by 180°** -- Incorrect. A half-cycle phase shift occurs only when the reflected ray encounters a medium with a higher refractive index on the other side of the boundary. Reflecting off a medium with a lower index produces no phase shift at all.
7. **Standing waves are a completely different phenomenon from ordinary waves** -- Incorrect. A standing wave is simply what you get when two traveling waves of equal amplitude and frequency move through the same medium in opposite directions and their superposition is taken. Standing waves store energy in place rather than carrying it along.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Wavelength ($\lambda$) | m (meter) | [L] |
| Frequency ($f$) | Hz (hertz) = s$^{-1}$ | [T]$^{-1}$ |
| Period ($T$) | s (second) | [T] |
| Wave speed ($v$) | m/s | [L][T]$^{-1}$ |
| Amplitude ($A$) | m (meter) | [L] |
| Wave number ($k$) | rad/m | [L]$^{-1}$ |
| Angular frequency ($\omega$) | rad/s | [T]$^{-1}$ |
| Intensity ($I$) | W/m$^2$ | [M][T]$^{-3}$ |
| Linear mass density ($\mu$) | kg/m | [M][L]$^{-1}$ |
| Tension ($F_T$) | N (newton) = kg·m/s$^2$ | [M][L][T]$^{-2}$ |
| Index of refraction ($n$) | dimensionless | dimensionless |
| Slit width / separation ($a$, $d$) | m (meter) | [L] |
| Film thickness ($t$) | m (meter) | [L] |
