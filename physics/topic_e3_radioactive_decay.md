# E.3: Radioactive Decay

> Theme E: Nuclear and Quantum Physics | SL + HL

## Key Concepts

### Types of Radioactive Decay
- **Alpha decay** ($\alpha$): an unstable nucleus ejects a helium-4 nucleus ($^4_2He$), reducing both mass number and atomic number
  - $^A_Z X \rightarrow ^{A-4}_{Z-2}Y + ^4_2He$
  - Strongly ionizing due to large charge and mass; travels only a short distance before being absorbed (paper or skin suffices)
- **Beta-minus decay** ($\beta^-$): a neutron within the nucleus converts to a proton, emitting an electron and an electron antineutrino
  - $^A_Z X \rightarrow ^A_{Z+1}Y + ^0_{-1}e + \bar{\nu}_e$
  - Intermediate in both ionizing ability and range; a few millimetres of aluminium will block these particles
- **Beta-plus decay** ($\beta^+$): a proton converts to a neutron, emitting a positron and an electron neutrino
  - $^A_Z X \rightarrow ^A_{Z-1}Y + ^0_{+1}e + \nu_e$
- **Gamma decay** ($\gamma$): an excited nucleus drops to a lower energy state by emitting a high-energy photon
  - Mass number $A$ and atomic number $Z$ remain unchanged
  - Weakly ionizing but highly penetrating; significant thicknesses of dense material such as lead or concrete are required for adequate shielding

### Properties of Radiation

| Property | Alpha ($\alpha$) | Beta ($\beta$) | Gamma ($\gamma$) |
|----------|---------|---------|----------|
| Particle | $^4_2He$ | $^0_{-1}e$ (or $^0_{+1}e$) | photon |
| Charge | +2 | -1 (or +1) | 0 |
| Mass | 4 u | ~0 | 0 |
| Ionizing power | High | Medium | Low |
| Penetrating power | Low | Medium | High |
| Stopped by | A sheet of paper or dead skin cells | A few mm of aluminium | Many cm of dense lead or concrete |

### Half-Life
- **Half-life** ($t_{1/2}$): the time interval after which exactly half of the radioactive nuclei present in any given sample will have undergone decay
- Individual decay events occur at unpredictable moments — the process is inherently random and cannot be triggered or prevented by external conditions
- $N = N_0 \left(\frac{1}{2}\right)^{t/t_{1/2}}$
- $N = N_0 e^{-\lambda t}$ where $\lambda$ = decay constant
- $\lambda = \frac{\ln 2}{t_{1/2}}$
- **Activity** ($A$): the rate at which decay events occur in a sample; $A = \lambda N$; SI unit: becquerel (Bq)

### Nuclear Stability
- A nucleus is stable when the strong nuclear force adequately balances electromagnetic repulsion between protons, which depends critically on the proton-to-neutron ratio
- For lighter elements the ratio $N/Z \approx 1$ is typical of stable nuclides; heavier elements require progressively more neutrons than protons ($N/Z > 1$) to maintain stability
- Nuclides lying above the band of stability carry an excess of neutrons and tend to shed them via $\beta^-$ decay
- Nuclides lying below the band of stability carry an excess of protons and reduce proton count through $\beta^+$ decay or by capturing an orbital electron
- For elements with $Z > 82$, the nucleus is so large that even a high $N/Z$ ratio cannot sustain stability; $\alpha$ decay is the predominant mode of adjustment

### Background Radiation
- Natural contributions arrive continuously from cosmic ray showers, radioactive minerals in the ground (particularly radon gas seeping from rock), and isotopes incorporated into food and living tissue (K-40, C-14)
- Human activity introduces additional sources including diagnostic and therapeutic medical procedures, residue from atmospheric weapons tests, and emissions from nuclear power facilities
- Any experimental count rate must be corrected by subtracting a separately measured background count to obtain the true activity of the sample under investigation

## Key Equations

| Equation | Description |
|----------|-------------|
| $N = N_0(1/2)^{t/t_{1/2}}$ | Exponential decay (half-life form) |
| $N = N_0 e^{-\lambda t}$ | Exponential decay (decay constant form) |
| $\lambda = \ln 2 / t_{1/2}$ | Decay constant and half-life relation |
| $A = \lambda N$ | Activity |

## Common Misconceptions

1. **"Radioactive decay can be sped up or slowed down"** — The timing of nuclear decay is governed solely by the nucleus itself. Changing temperature, applying pressure, or placing the material in a different chemical compound has no measurable effect on the decay rate.
2. **"After two half-lives, all nuclei have decayed"** — Each half-life reduces the remaining quantity by half, so after two half-lives 25% of the original nuclei still persist; after three, 12.5% remain. The curve approaches zero asymptotically and never reaches it.
3. **"Radiation always means nuclear radiation"** — The word "radiation" covers the entire electromagnetic spectrum as well as particle emissions. Nuclear radiation — alpha, beta, and gamma — is only one category within this broader meaning.
4. **"All radiation is dangerous"** — Hazard is determined by the type of radiation, its energy, the duration of exposure, and how close the source is. Alpha particles, for example, are blocked by skin and pose negligible external risk, but become hazardous when a source is inhaled or ingested.

## Comparison with AP Physics

- AP Physics 1 does not cover nuclear physics
- AP Physics 2 covers radioactive decay with similar scope
- IB includes radioactive decay as core SL content, integrated with nuclear stability
