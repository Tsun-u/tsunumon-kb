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
- Induced EMF equals the rate of change of magnetic flux linkage:
- $\varepsilon = -N\frac{\Delta\Phi}{\Delta t}$
- The negative sign indicates Lenz's law

### Lenz's Law
- The induced current flows in a direction that opposes the change in flux that caused it
- Consequence of conservation of energy
- Examples: dropping a magnet through a coil, eddy currents, electromagnetic braking

### Applications of Electromagnetic Induction
- **AC generators**: rotating coil in magnetic field
  - $\varepsilon = NBA\omega\sin(\omega t)$ (sinusoidal EMF)
  - Peak EMF: $\varepsilon_0 = NBA\omega$
- **Transformers**: transfer electrical energy between circuits via changing magnetic flux
  - $\frac{V_s}{V_p} = \frac{N_s}{N_p}$ (ideal transformer)
  - $V_p I_p = V_s I_s$ (power conservation in ideal transformer)
  - Step-up: $N_s > N_p$; step-down: $N_s < N_p$
  - Applications: power transmission (high voltage reduces losses)

### Alternating Current (AC)
- Sinusoidal: $V = V_0\sin(\omega t)$, $I = I_0\sin(\omega t)$
- **RMS values**: $V_{rms} = \frac{V_0}{\sqrt{2}}$, $I_{rms} = \frac{I_0}{\sqrt{2}}$
- Average power: $P_{avg} = I_{rms}V_{rms} = \frac{1}{2}I_0 V_0$

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

1. **"A stationary magnet near a coil induces current"** -- There must be a change in flux; a stationary magnet produces constant flux and no induced EMF.
2. **"Transformers work with DC"** -- Transformers require changing flux; DC produces constant flux after initial transient.
3. **"Lenz's law violates conservation of energy"** -- On the contrary, Lenz's law is a consequence of conservation of energy; work must be done against the opposing force.
4. **"RMS voltage is the average voltage"** -- The average of a sinusoidal AC voltage is zero; RMS is the effective value that produces the same heating as DC.

## Comparison with AP Physics

- AP Physics C (E&M) covers Faraday's law and Lenz's law with calculus
- AP Physics 1 and 2 do not cover electromagnetic induction
- IB HL covers induction with algebra-based treatment; similar conceptual depth to AP C
