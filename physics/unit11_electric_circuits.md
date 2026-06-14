# Unit 11: Electric Circuits

> Exam Weight: 15--18% | ~12--20 Class Periods

## Topics

### 11.1 Electric Current
- Electric current measures how rapidly charge moves through a cross-section of a conductor
$$I = \frac{\Delta Q}{\Delta t}$$
- SI unit: ampere (A) = coulomb per second (C/s)
- **Conventional current**: a model convention in which current direction is taken as the way positive charges would travel — from high potential toward low potential
- **Electron flow**: the actual movement of electrons in a metal is toward higher potential, which is the reverse of conventional current direction
- In metallic conductors, the mobile charge carriers are free (conduction) electrons rather than positive ions
- **Drift velocity** ($v_d$): the small net speed at which charge carriers slowly migrate through a conductor when an electric field is applied
$$I = nAv_d |q|$$
  - $n$ = number density of charge carriers (number per unit volume)
  - $A$ = cross-sectional area of the conductor
  - $v_d$ = drift velocity
  - $|q|$ = magnitude of charge per carrier ($e = 1.6 \times 10^{-19}$ C for electrons)
- Although drift speed is very slow (typically $\sim 10^{-4}$ m/s), the electric field that drives the motion propagates through the circuit at nearly the speed of light

### 11.2 Simple Circuits
- A **complete circuit** needs an unbroken conducting loop: current must be able to travel from one terminal of the source, through external elements, and back to the other terminal
- **Electromotive force (emf, $\mathcal{E}$)**: the work done per unit charge by a source (battery, generator) to push charge around the circuit; despite the name, it is an energy-per-charge quantity, not a mechanical force
  - SI unit: volt (V) = joule per coulomb (J/C)
- A real battery has **internal resistance** ($r$), an unavoidable opposition to current inside the source itself that wastes some energy as heat
- **Terminal voltage**: the voltage a voltmeter would measure across the battery's external terminals while current is flowing
$$V_{terminal} = \mathcal{E} - Ir$$
  - $I$ = current drawn from the battery
  - With no load connected ($I = 0$), the terminal voltage equals the emf
- A short circuit occurs when a near-zero resistance path connects the terminals, letting an extremely large current surge through the source and rapidly converting energy in the internal resistance to heat

### 11.3 Resistance, Resistivity, and Ohm's Law
- **Ohm's law**: for many conductors, the voltage applied across them is directly proportional to the current that flows
$$V = IR$$
- **Resistance** ($R$): a quantity that captures how strongly a component opposes current for a given applied voltage
  - SI unit: ohm ($\Omega$) = volt per ampere (V/A)
- **Resistivity** ($\rho$): a material-specific constant that, together with geometry, determines a conductor's resistance
$$R = \frac{\rho L}{A}$$
  - $L$ = length of the conductor
  - $A$ = cross-sectional area of the conductor
  - A longer conductor has more resistance; a wider cross-section gives less resistance
- How resistivity changes with temperature differs by material type:
  - In metals, higher temperature means more lattice vibrations that scatter electrons, raising resistivity
  - In semiconductors, higher temperature frees more charge carriers, reducing resistivity
- **Ohmic** materials: those whose $V$-$I$ graph is a straight line through the origin, indicating constant resistance — typical of metals at stable temperature
- **Non-ohmic** materials: those whose resistance depends on the current or voltage, producing a curved $V$-$I$ graph; diodes and incandescent bulb filaments are common examples

### 11.4 Electric Power
- **Electric power**: how quickly a circuit element converts electrical energy into another form such as heat, light, or mechanical motion
$$P = IV$$
- Substituting Ohm's law yields two additional useful forms:
$$P = I^2 R = \frac{V^2}{R}$$
- Total electrical energy transferred over a time interval:
$$E = Pt$$
- The **kilowatt-hour** (kWh) is a unit of energy (not power):
$$1 \text{ kWh} = 3.6 \times 10^6 \text{ J}$$
- All energy delivered to a pure resistor is converted to thermal energy through Joule heating — none is stored
- Power output of a battery: $P_{emf} = \mathcal{E}I$
- Power lost inside the battery itself: $P_{internal} = I^2 r$

### 11.5 Compound Direct Current (DC) Circuits
- **Series connection**: resistors chained one after another so every element carries the same current
  - Current is the same through all elements: $I_{total} = I_1 = I_2 = \cdots$
  - Voltages add: $V_{total} = V_1 + V_2 + \cdots$
  - Equivalent resistance: $R_{eq} = R_1 + R_2 + \cdots$
  - The combined resistance exceeds that of any single element in the chain
- **Parallel connection**: resistors joined between the same pair of nodes, sharing the same voltage across each branch
  - Voltage is the same across all elements: $V_{total} = V_1 = V_2 = \cdots$
  - Currents add: $I_{total} = I_1 + I_2 + \cdots$
  - Equivalent resistance: $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots$
  - The combined resistance is smaller than the smallest individual resistor in the group
  - For two resistors in parallel: $R_{eq} = \frac{R_1 R_2}{R_1 + R_2}$
- **Combination (compound) circuits**: networks that mix series and parallel sections
  - Approach: locate distinct series or parallel sub-groups and reduce them one step at a time until a single equivalent resistance remains, then reverse the process to recover individual currents and voltages

### 11.6 Kirchhoff's Loop Rule
- **Kirchhoff's loop rule** (voltage law, KVL): if you add up every voltage rise and drop encountered on a complete trip around any closed circuit loop, the total is zero
$$\sum_{loop} \Delta V = 0$$
- This follows from energy conservation: a test charge returning to its starting point in a circuit must have the same potential energy it started with
- **Sign conventions** when tracing around a chosen loop direction:
  - Battery: gains $+\mathcal{E}$ when traversed from the $-$ to the $+$ terminal; loses $-\mathcal{E}$ when traversed from $+$ to $-$
  - Resistor: drops $-IR$ when followed in the current direction; gains $+IR$ when followed against the current
- The rule holds for any closed loop drawn on a circuit diagram, even one that contains no actual branch current

### 11.7 Kirchhoff's Junction Rule
- **Kirchhoff's junction rule** (current law, KCL): at any point in a circuit where wires branch, the total current arriving must equal the total current departing
$$\sum I_{in} = \sum I_{out}$$
- This reflects charge conservation: in steady state, no charge piles up or disappears at a node
- Procedure for solving multi-loop circuits:
  1. Label each branch with an assumed current direction (a negative result simply means the actual direction is reversed)
  2. Write junction equations at the independent nodes
  3. Write loop equations for independent closed loops
  4. Solve the system of simultaneous equations for the unknown currents

### 11.8 Resistor-Capacitor (RC) Circuits
- An RC circuit pairs a resistor and a capacitor in series; a switch and battery are included for charging scenarios
- **Charging a capacitor** (switch closed at $t = 0$ with battery $\mathcal{E}$):
$$Q(t) = Q_{max}\left(1 - e^{-t/RC}\right) = C\mathcal{E}\left(1 - e^{-t/RC}\right)$$
$$V_C(t) = \mathcal{E}\left(1 - e^{-t/RC}\right)$$
$$I(t) = \frac{\mathcal{E}}{R} e^{-t/RC}$$
  - The circuit current is largest immediately after the switch closes ($\mathcal{E}/R$) and falls exponentially toward zero as the capacitor charges
  - The capacitor voltage begins at zero and grows exponentially, leveling off at $\mathcal{E}$
- **Discharging a capacitor** (battery removed, initial charge $Q_0$):
$$Q(t) = Q_0 e^{-t/RC}$$
$$V_C(t) = V_0 e^{-t/RC}$$
$$I(t) = -\frac{V_0}{R} e^{-t/RC}$$
  - Stored charge, voltage, and current all decline exponentially toward zero
- **Time constant**: $\tau = RC$
  - At $t = \tau$: a charging capacitor has reached $\approx 63.2\%$ of full charge; a discharging one still holds $\approx 36.8\%$
  - At $t = 5\tau$: the charging or discharging process is essentially complete ($> 99\%$)
  - SI unit of $\tau$: seconds (since $\Omega \cdot \text{F} = \text{s}$)
- **Steady state**: once $t \gg \tau$, the capacitor voltage matches the source voltage, no current flows in that branch, and the capacitor behaves as an open circuit

## Skills to Master

- Explain what electric current represents and contrast how conventional current and electron flow differ in direction
- Use Ohm's law to find an unknown voltage, current, or resistance given the other two quantities
- Express how a conductor's resistance depends on its material resistivity, its length, and its cross-sectional area
- Compute power dissipated in a circuit element using any applicable form: $P = IV$, $P = I^2R$, or $P = V^2/R$
- Combine resistors in series and parallel to find equivalent resistance for multi-element networks
- Use Kirchhoff's loop and junction rules together to solve for unknown currents and voltages in multi-loop circuits
- Predict how voltage, current, and stored charge evolve over time in RC circuits during both charging and discharging phases
- Evaluate the time constant $\tau = RC$ and use it to find circuit quantities at any given moment
- Contrast emf with terminal voltage and account for the effect of internal resistance on a real battery's output

## Core Concepts

1. Current quantifies how much charge passes through a cross-section per unit time; by convention its direction follows the path a positive charge would take, moving from higher to lower potential
2. For ohmic conductors, voltage and current are proportional ($V = IR$), giving a straight-line graph; the slope is the constant resistance
3. A conductor's resistance is set by three factors: the intrinsic resistivity of the material, how long the conductor is, and the size of its cross-sectional area — as well as temperature
4. Electrical energy delivered to a resistor turns into thermal energy at a rate given by $P = IV = I^2R = V^2/R$
5. Series circuits share a common current while individual voltages add up; parallel circuits share a common voltage while individual currents add up
6. Because energy is conserved, any charge completing a full loop in a circuit must gain exactly as much potential as it loses — the algebraic sum of all voltage changes around a closed loop is zero (Kirchhoff's voltage law)
7. Because charge is conserved, the total current flowing into any node must equal the total current flowing out — there is no accumulation of charge at a junction (Kirchhoff's current law)
8. When a capacitor charges or discharges through a resistor, the charge and voltage follow exponential curves governed by the time constant $\tau = RC$; once fully charged, the capacitor passes no steady-state current and acts as an open circuit

## Key Equations

### Electric Current

$$I = \frac{\Delta Q}{\Delta t}$$

$$I = nAv_d |q|$$

### Terminal Voltage

$$V_{terminal} = \mathcal{E} - Ir$$

### Ohm's Law and Resistance

$$V = IR$$

$$R = \frac{\rho L}{A}$$

### Electric Power

$$P = IV = I^2 R = \frac{V^2}{R}$$

$$E = Pt$$

### Series Resistance

$$R_{eq} = R_1 + R_2 + \cdots + R_n$$

### Parallel Resistance

$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \cdots + \frac{1}{R_n}$$

### Kirchhoff's Rules

$$\sum_{loop} \Delta V = 0 \quad \text{(loop rule)}$$

$$\sum I_{in} = \sum I_{out} \quad \text{(junction rule)}$$

### RC Circuits -- Charging

$$Q(t) = C\mathcal{E}\left(1 - e^{-t/RC}\right)$$

$$I(t) = \frac{\mathcal{E}}{R} e^{-t/RC}$$

### RC Circuits -- Discharging

$$Q(t) = Q_0 e^{-t/RC}$$

$$I(t) = -\frac{Q_0}{RC} e^{-t/RC}$$

### Time Constant

$$\tau = RC$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Electric current ($I$)** | The amount of electric charge passing through a cross-section per unit time; $I = \Delta Q / \Delta t$ |
| **Conventional current** | A model in which current direction is assigned to the path positive charges would follow, moving from high potential to low potential |
| **Drift velocity ($v_d$)** | The slow, net displacement speed of charge carriers in a conductor when an electric field is applied |
| **Electromotive force (emf, $\mathcal{E}$)** | The work done per unit charge by a source (such as a battery) in moving charge through the circuit; unit is volt (V) |
| **Internal resistance ($r$)** | Inherent resistance inside a real battery or generator that causes some energy to be lost internally |
| **Terminal voltage** | The measurable voltage between the external terminals of a source when current is flowing; $V = \mathcal{E} - Ir$ |
| **Resistance ($R$)** | A measure of how strongly a component impedes current; numerically the voltage across it divided by the current through it ($R = V/I$); unit is ohm ($\Omega$) |
| **Resistivity ($\rho$)** | A material-specific constant that scales how much resistance a given geometry of that material will have |
| **Ohmic material** | A material whose voltage-current relationship is linear, meaning its resistance stays constant regardless of applied voltage |
| **Non-ohmic material** | A material whose resistance changes with operating conditions, producing a curved $V$-$I$ characteristic |
| **Kirchhoff's loop rule** | A statement of energy conservation: the signed sum of all potential differences encountered on any closed circuit path equals zero |
| **Kirchhoff's junction rule** | A statement of charge conservation: at any branching point in a circuit, the charge flowing in every second must equal the charge flowing out |
| **Time constant ($\tau$)** | The product $RC$ that sets the timescale for exponential growth or decay of charge and voltage in an RC circuit |
| **Steady state** | The long-time condition in an RC circuit ($t \gg \tau$) where the capacitor is fully charged and no current passes through it |
| **Kilowatt-hour (kWh)** | A practical unit of electrical energy equal to $3.6 \times 10^6$ J; used by utility companies to measure energy consumption |

## Common Misconceptions

1. **Current is "used up" as it passes through resistors** -- This is wrong. The same amount of current exits a resistor as enters it — charge is conserved. What the resistor consumes is electric potential energy (voltage drops), not charge flow.
2. **A battery supplies constant current** -- A battery maintains an approximately constant emf, not constant current. How much current actually flows depends on the total resistance of the external circuit via $I = \mathcal{E} / R_{total}$.
3. **Larger resistance always means less power dissipated** -- This depends on what is held constant. In a series circuit where current is fixed, a larger resistor dissipates more power ($P = I^2R$). In a parallel circuit where voltage is fixed, a larger resistor dissipates less power ($P = V^2/R$). The answer flips depending on circuit configuration.
4. **Adding a resistor in parallel increases total resistance** -- The opposite is true. Each additional parallel path gives current another route to take, so the equivalent resistance always decreases. $R_{eq}$ is always smaller than the smallest individual resistor in the group.
5. **Electrons move at the speed of light through a wire** -- In reality, electrons drift at speeds around $10^{-4}$ m/s. What travels at near light-speed is the electric field disturbance, which simultaneously nudges all the electrons in the wire into motion — that is why lights turn on instantly.
6. **In an RC circuit, the capacitor charges linearly** -- Charging (and discharging) follows an exponential curve, not a straight line. As charge builds on the capacitor, the voltage opposing further charge flow grows, reducing the current and slowing the rate of accumulation.
7. **A fully charged capacitor behaves like a short circuit** -- The two cases are reversed. A fully charged capacitor allows no current to flow and behaves like an open circuit. It is an initially uncharged capacitor that behaves momentarily like a short circuit, allowing maximum current at $t = 0$.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Electric current | A (ampere) = C/s | [I] |
| Charge | C (coulomb) = A$\cdot$s | [I][T] |
| Voltage / emf | V (volt) = J/C = W/A | [M][L]$^2$[T]$^{-3}$[I]$^{-1}$ |
| Resistance | $\Omega$ (ohm) = V/A | [M][L]$^2$[T]$^{-3}$[I]$^{-2}$ |
| Resistivity | $\Omega \cdot$m | [M][L]$^3$[T]$^{-3}$[I]$^{-2}$ |
| Capacitance | F (farad) = C/V | [M]$^{-1}$[L]$^{-2}$[T]$^4$[I]$^2$ |
| Electric power | W (watt) = J/s = V$\cdot$A | [M][L]$^2$[T]$^{-3}$ |
| Energy | J (joule) = W$\cdot$s | [M][L]$^2$[T]$^{-2}$ |
| Energy (practical) | kWh = $3.6 \times 10^6$ J | [M][L]$^2$[T]$^{-2}$ |
| Time constant ($\tau = RC$) | s (second) = $\Omega \cdot$F | [T] |
