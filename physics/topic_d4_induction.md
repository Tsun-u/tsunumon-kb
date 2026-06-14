# D.4: Induction

> Theme D: Fields | HL only

## Key Concepts

### Magnetic Flux
- **Magnetic flux** ($\Phi$): $\Phi = BA\cos\theta$
  - $B$: magnetic field strength (T)
  - $A$: area (m²)
  - $\theta$: angle between $B$ and the normal to the surface
- SI unit: weber (Wb) = T·m²
- Flux linkage for $N$ turns: $N\Phi$

### Faraday's Law of Induction
- The EMF induced in a coil is proportional to how rapidly the magnetic flux linkage changes over time:
- $\varepsilon = -N\frac{\Delta\Phi}{\Delta t}$
- The negative sign encodes the directionality of the induced EMF, consistent with Lenz's law

### Lenz's Law
- Whenever flux through a circuit changes, the resulting induced current creates its own magnetic field that acts to resist that change
- This behaviour follows directly from the principle that energy cannot be created from nothing — the opposing force ensures work must be supplied
- Practical illustrations: a falling magnet decelerating as it enters a coil, braking forces on conducting discs moving through fields, and eddy-current damping in metal structures

### Applications of Electromagnetic Induction
- **AC generators**: rotating coil in magnetic field
  - $\varepsilon = NBA\omega\sin(\omega t)$ (sinusoidal EMF)
  - Peak EMF: $\varepsilon_0 = NBA\omega$
- **Transformers**: couple two circuits magnetically so that a time-varying flux in the primary coil drives an EMF in the secondary
  - $\frac{V_s}{V_p} = \frac{N_s}{N_p}$ (ideal transformer)
  - $V_p I_p = V_s I_s$ (power conservation in ideal transformer)
  - Step-up: $N_s > N_p$; step-down: $N_s < N_p$
  - Applications: power transmission (high voltage reduces losses)

### Alternating Current (AC)
- Both voltage and current vary sinusoidally with time: $V = V_0\sin(\omega t)$, $I = I_0\sin(\omega t)$
- **RMS values** represent the equivalent steady-state (DC) magnitudes for power purposes: $V_{rms} = \frac{V_0}{\sqrt{2}}$, $I_{rms} = \frac{I_0}{\sqrt{2}}$
- The mean power delivered to a resistive load equals the product of the RMS quantities: $P_{avg} = I_{rms}V_{rms} = \frac{1}{2}I_0 V_0$

## Key Equations

| Equation | Description |
|----------|-------------|
| $\Phi = BA\cos\theta$ | Magnetic flux |
| $\varepsilon = -N\Delta\Phi/\Delta t$ | Faraday's law |
| $V_s/V_p = N_s/N_p$ | Transformer equation |
| $\varepsilon_0 = NBA\omega$ | Peak EMF of generator |
| $V_{rms} = V_0/\sqrt{2}$ | RMS voltage |
| $P_{avg} = I_{rms}V_{rms}$ | Average AC power |

## Common Misconceptions

1. **"A stationary magnet near a coil induces current"** -- Induction requires flux to be changing. A magnet held still maintains a constant flux through the coil, so Faraday's law gives zero induced EMF.
2. **"Transformers work with DC"** -- A transformer's secondary coil responds only to a changing flux in the core. A steady DC current through the primary produces no flux variation and therefore no output voltage (beyond a brief startup transient).
3. **"Lenz's law violates conservation of energy"** -- Lenz's law is actually a direct expression of energy conservation. The opposing force the induced current exerts means an external agent must do work to maintain the changing flux, preventing free energy generation.
4. **"RMS voltage is the average voltage"** -- For a symmetric sinusoidal wave the true time-average is zero, since positive and negative half-cycles cancel. The RMS value instead gives the equivalent DC voltage that would deliver identical power to a resistive load.

## Comparison with AP Physics

- AP Physics C (E&M) covers Faraday's law and Lenz's law with calculus
- AP Physics 1 and 2 do not cover electromagnetic induction
- IB HL covers induction with algebra-based treatment; similar conceptual depth to AP C
