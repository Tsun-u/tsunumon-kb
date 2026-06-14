# B.5: Current and Circuits

> Theme B: The Particulate Nature of Matter | SL + HL

## Key Concepts

### Electric Current
- **Current** ($I$): the rate at which charge passes through a cross-section; $I = \frac{\Delta q}{\Delta t}$
- SI unit: ampere (A) = C/s
- Conventional current: defined as the direction a positive charge would travel (opposite to actual electron motion)
- **Charge carriers**: electrons in metallic conductors, ions in electrolytes

### Potential Difference (Voltage)
- **Potential difference** ($V$): the electrical energy delivered per unit charge moved between two points; $V = \frac{W}{q}$
- SI unit: volt (V) = J/C
- **EMF** ($\varepsilon$): the energy supplied per unit charge by a source driving the circuit

### Resistance and Ohm's Law
- **Resistance** ($R$): a component's opposition to the flow of charge; $R = \frac{V}{I}$
- SI unit: ohm ($\Omega$)
- **Ohm's law**: $V = IR$ (applies to ohmic conductors, which show a linear V-I relationship)
- **Resistivity**: $R = \frac{\rho L}{A}$ (depends on material, length, cross-sectional area)
- Non-ohmic devices: filament lamps, diodes, thermistors, LDRs

### Circuit Analysis
- **Series circuits**:
  - Every component carries the same current
  - Voltages add: $V_T = V_1 + V_2 + ...$
  - Resistances add: $R_T = R_1 + R_2 + ...$
- **Parallel circuits**:
  - Each branch sits across the same voltage
  - Currents add: $I_T = I_1 + I_2 + ...$
  - Reciprocal resistances add: $\frac{1}{R_T} = \frac{1}{R_1} + \frac{1}{R_2} + ...$
- **Kirchhoff's laws**:
  - Junction rule: $\sum I_{in} = \sum I_{out}$ (conservation of charge)
  - Loop rule: $\sum V = 0$ around any closed loop (conservation of energy)

### Internal Resistance
- Practical batteries possess an internal resistance ($r$) that limits the terminal voltage under load
- Terminal voltage: $V = \varepsilon - Ir$
- $\varepsilon = I(R + r)$

### Power in Circuits
- $P = IV = I^2R = \frac{V^2}{R}$
- Energy dissipated: $E = Pt = IVt$

### Potential Divider
- Two resistors in series divide the EMF proportionally:
- $V_{out} = \frac{R_2}{R_1 + R_2} \cdot V_{in}$
- Applications: sensors with thermistors or LDRs

## Key Equations

| Equation | Description |
|----------|-------------|
| $I = \frac{\Delta q}{\Delta t}$ | Current |
| $V = IR$ | Ohm's law |
| $R = \frac{\rho L}{A}$ | Resistance from resistivity |
| $P = IV = I^2R = V^2/R$ | Electrical power |
| $\varepsilon = I(R + r)$ | EMF with internal resistance |
| $V_{out} = \frac{R_2}{R_1+R_2}V_{in}$ | Potential divider |

## Common Misconceptions

1. **"Current is used up in a circuit"** -- Current is the same throughout a series circuit; energy is transferred, not current.
2. **"Voltage pushes current"** -- Potential difference drives current; it is the cause, current is the effect.
3. **"Adding resistors always increases total resistance"** -- In parallel, adding resistors decreases total resistance.
4. **"Batteries provide constant current"** -- Batteries provide approximately constant EMF; current depends on the circuit.

## Comparison with AP Physics

- AP Physics 1 does not cover circuits in detail (removed in 2024 update)
- AP Physics 2 covers DC circuits with similar scope
- IB includes circuits as core SL content, covering Kirchhoff's laws, internal resistance, and potential dividers
