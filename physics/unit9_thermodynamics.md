# Unit 9: Thermodynamics

> Exam Weight: 15--18% | ~10--16 Class Periods

## Topics

### 9.1 Kinetic Theory of Temperature and Pressure
- Kinetic molecular theory pictures a gas as an enormous collection of particles zipping around in continuous, random motion
- Ideal gas assumptions:
  - Gas consists of a large number of identical particles (atoms or molecules)
  - Particles are point-like (volume of particles is negligible compared to container volume)
  - Particles undergo perfectly elastic collisions with each other and container walls
  - No intermolecular forces except during collisions
  - Motion is random; all directions are equally probable
- Temperature tracks the average translational kinetic energy carried by individual gas molecules:

$$K_{\text{avg}} = \frac{3}{2} k_B T$$

- $k_B = 1.38 \times 10^{-23} \text{ J/K}$ is the Boltzmann constant
- Gas pressure originates from the cumulative momentum delivered by countless molecular impacts on the container walls
- Pressure scales with both the number of molecules per unit volume and the average kinetic energy each carries
- Root-mean-square (rms) speed of gas molecules:

$$v_{\text{rms}} = \sqrt{\frac{3 k_B T}{m}}$$

- where $m$ is the mass of a single molecule
- At a fixed temperature, molecules with smaller mass achieve higher $v_{\text{rms}}$
- All kinetic theory and gas law formulas require temperature in kelvin

### 9.2 The Ideal Gas Law
- The ideal gas law ties together the four macroscopic quantities that describe a gas sample:

$$PV = nRT$$

- where $n$ is the number of moles and $R = 8.314 \text{ J/(mol·K)}$ is the universal gas constant
- Equivalent form using number of molecules $N$:

$$PV = N k_B T$$

- where $N = nN_A$ and $N_A = 6.022 \times 10^{23} \text{ mol}^{-1}$ is Avogadro's number
- Relationship: $R = N_A k_B$
- Special processes for a fixed amount of ideal gas:
  - **Isothermal** (constant $T$): $PV = \text{const}$, so $P_1 V_1 = P_2 V_2$
  - **Isobaric** (constant $P$): $\frac{V}{T} = \text{const}$, so $\frac{V_1}{T_1} = \frac{V_2}{T_2}$
  - **Isovolumetric / Isochoric** (constant $V$): $\frac{P}{T} = \text{const}$, so $\frac{P_1}{T_1} = \frac{P_2}{T_2}$
- The ideal gas model is most reliable at high temperatures and low pressures, where molecule-to-molecule attractions and finite molecular volumes become negligible

### 9.3 Thermal Energy Transfer and Equilibrium
- Three distinct pathways through which thermal energy moves from one place to another:
  - **Conduction**: energy passes via molecule-to-molecule contact without bulk material movement; active in solids, liquids, and gases
  - **Convection**: energy is carried bodily by moving portions of a fluid (either driven by density differences or forced by external means); occurs in liquids and gases
  - **Radiation**: energy propagates as electromagnetic waves and needs no material medium, traveling even through a vacuum
- **Zeroth law of thermodynamics**: if system A is in thermal equilibrium with system C, and system B is also in thermal equilibrium with system C, then A and B are in thermal equilibrium with each other
- When two objects in thermal contact ultimately reach the same temperature, no further net heat exchange occurs—they have reached thermal equilibrium
- Absent external intervention, heat always moves spontaneously from the higher-temperature body toward the lower-temperature one
- Internal energy ($U$): the total kinetic and potential energy of all molecules in a system
- For a monatomic ideal gas: $U = \frac{3}{2} n R T = \frac{3}{2} N k_B T$
- Because ideal gas molecules have no potential energy between them, $U$ responds only to temperature changes—not to how $P$ and $V$ are individually arranged

### 9.4 The First Law of Thermodynamics
- The first law expresses energy conservation for any thermodynamic system:

$$\Delta U = Q - W$$

- where $\Delta U$ is the change in internal energy, $Q$ is the heat added to the system, and $W$ is the work done by the system
- Sign conventions (physics convention):
  - $Q > 0$: heat flows into the system
  - $Q < 0$: heat flows out of the system
  - $W > 0$: work done by the system (gas expands)
  - $W < 0$: work done on the system (gas compresses)
- Work done by a gas during an isobaric process:

$$W = P \Delta V$$

- On a PV diagram:
  - The area beneath a process curve equals the work performed by the gas
  - A clockwise cycle encloses net positive work output (heat engine operation)
  - A counterclockwise cycle encloses net negative work (refrigerator or heat pump operation)
- How the first law simplifies for each special process:
  - **Isothermal** ($\Delta T = 0$): $\Delta U = 0$, so $Q = W$
  - **Isobaric** ($\Delta P = 0$): $W = P \Delta V$, and $\Delta U = Q - P \Delta V$
  - **Isovolumetric** ($\Delta V = 0$): $W = 0$, so $\Delta U = Q$
  - **Adiabatic** ($Q = 0$): $\Delta U = -W$; compression raises temperature, expansion lowers temperature

### 9.5 Specific Heat and Thermal Conductivity
- Heat required to change the temperature of a substance:

$$Q = mc\Delta T$$

- where $m$ is mass, $c$ is specific heat capacity, and $\Delta T = T_f - T_i$
- Specific heat capacity $c$ captures how thermally stubborn a material is: a large $c$ means a substance needs substantial heat input to warm up even a little
- Water's exceptionally large specific heat ($c_{\text{water}} = 4186 \text{ J/(kg·K)}$) has major consequences for climate and biology
- In a well-insulated (isolated) calorimetry setup: $Q_{\text{lost}} + Q_{\text{gained}} = 0$
- Rate of heat conduction through a material:

$$\frac{Q}{\Delta t} = \frac{kA\Delta T}{L}$$

- where $k$ is thermal conductivity, $A$ is cross-sectional area, $\Delta T$ is temperature difference across the material, and $L$ is thickness
- Metals have high $k$ and conduct heat readily; materials like wood, foam, and air have low $k$ and act as effective insulators

### 9.6 Entropy and the Second Law of Thermodynamics
- **Entropy** ($S$): a thermodynamic state function whose value grows with the number of microscopic arrangements (microstates) that produce the same observable macrostate; commonly linked to the idea of dispersal or spreading of energy
- **Second law of thermodynamics**: in any isolated system, total entropy cannot decrease—it either grows (irreversible process) or remains constant (reversible process)

$$\Delta S_{\text{total}} \geq 0$$

- Every real-world process is irreversible to some degree; the universe's total entropy therefore trends upward without exception
- Heat engines convert thermal energy into mechanical work:
  - Absorb heat $Q_H$ from a hot reservoir at temperature $T_H$
  - Expel waste heat $Q_C$ to a cold reservoir at temperature $T_C$
  - Produce net work $W = Q_H - Q_C$
- Efficiency of a heat engine:

$$e = \frac{W}{Q_H} = 1 - \frac{Q_C}{Q_H}$$

- **Carnot efficiency**: the maximum possible efficiency for a heat engine operating between two temperatures:

$$e_{\text{Carnot}} = 1 - \frac{T_C}{T_H}$$

- where $T_C$ and $T_H$ are in kelvin
- Carnot efficiency is an absolute ceiling dictated by the second law; no engine—however carefully built—can surpass it
- Familiar irreversible processes include free gas expansion, spontaneous heat conduction, frictional dissipation, and mixing of distinct gases
- A local entropy reduction (such as a refrigerator chilling its contents) is always paid for by a larger entropy increase in the surroundings, keeping the universal total on an upward trajectory

## Skills to Master

- Connect kinetic molecular theory to macroscopic gas properties by tracing how particle-level behavior gives rise to measurable temperature and pressure
- Compute average translational kinetic energy and root-mean-square speed for gas molecules at a specified temperature
- Use the ideal gas law to find an unknown state variable when the others are known, before and after a thermodynamic change
- Classify and analyze gas processes—isothermal, isobaric, isovolumetric, and adiabatic—using both algebraic and graphical approaches
- Distinguish among conduction, convection, and radiation as pathways for thermal energy transfer
- Use the zeroth law to establish whether two objects are in thermal equilibrium via a common thermal reference
- Employ the first law of thermodynamics to connect changes in internal energy, heat exchanged, and work performed
- Extract work values from PV diagrams by interpreting areas under process curves and enclosed cycle areas
- Determine heat transferred during temperature changes using specific heat capacity
- Evaluate the steady-state rate of heat conduction through a solid layer given its geometry and conductivity
- Articulate the meaning of entropy and the direction imposed on natural processes by the second law
- Compute heat engine efficiency and recognize the Carnot result as an absolute upper bound

## Core Concepts

1. Temperature quantifies how much average translational kinetic energy each gas molecule carries; this relationship is captured by $K_{\text{avg}} = \frac{3}{2} k_B T$
2. The ideal gas law ($PV = nRT$) links all four state variables of a gas sample and becomes accurate when molecule volumes and mutual attractions are both negligible
3. Heat is energy crossing a system boundary because of a temperature difference; it always moves spontaneously from the hotter region to the cooler one, stopping when both reach the same temperature
4. The first law ($\Delta U = Q - W$) extends energy conservation to thermal systems: whatever energy enters as heat, minus whatever leaves as work done by the gas, accumulates as a change in internal energy
5. On a PV diagram, the area beneath a process path equals the work performed by the gas; for a closed cycle, the net work equals the area enclosed by the loop
6. For an ideal gas, internal energy is determined entirely by temperature—pressure and volume separately have no effect once $T$ is fixed
7. Specific heat capacity is a material property expressing how many joules of heat are required to raise one kilogram of a substance by one kelvin
8. Conductive heat flow through a slab increases with higher thermal conductivity, larger cross-sectional area, and greater temperature difference, and decreases with greater thickness
9. The second law of thermodynamics forbids any isolated system from experiencing a net decrease in entropy; every naturally occurring process produces entropy, so the universe's entropy grows continuously
10. The Carnot efficiency sets an absolute ceiling on heat engine performance; no engine—real or theoretical—can surpass it when operating between the same two temperature reservoirs

## Key Equations

### Kinetic Theory

$$K_{\text{avg}} = \frac{3}{2} k_B T$$

$$v_{\text{rms}} = \sqrt{\frac{3 k_B T}{m}}$$

### Ideal Gas Law

$$PV = nRT$$

$$PV = N k_B T$$

### Internal Energy (Monatomic Ideal Gas)

$$U = \frac{3}{2} n R T$$

### First Law of Thermodynamics

$$\Delta U = Q - W$$

### Work Done by Gas (Isobaric Process)

$$W = P \Delta V$$

### Heat Transfer

$$Q = mc\Delta T$$

### Rate of Heat Conduction

$$\frac{Q}{\Delta t} = \frac{kA\Delta T}{L}$$

### Heat Engine Efficiency

$$e = \frac{W}{Q_H} = 1 - \frac{Q_C}{Q_H}$$

### Carnot Efficiency

$$e_{\text{Carnot}} = 1 - \frac{T_C}{T_H}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Temperature** | A scalar property proportional to the average translational kinetic energy of a substance's molecules; converted to kelvin by $T(\text{K}) = T(°\text{C}) + 273.15$ |
| **Pressure** | The perpendicular force exerted per unit area on a surface by gas molecules striking it; $P = F/A$ |
| **Ideal gas** | A model gas in which molecules occupy no volume and interact with one another only through perfectly elastic collisions |
| **Internal energy ($U$)** | The sum of all microscopic kinetic and potential energies within a system; for an ideal gas, this quantity tracks temperature alone |
| **Heat ($Q$)** | Thermal energy crossing a system boundary driven by a temperature difference between the system and its surroundings |
| **Work ($W$)** | In thermodynamics, energy exchanged when a gas boundary moves against an external pressure, causing expansion or compression |
| **Isothermal process** | A process carried out while temperature remains fixed ($\Delta T = 0$) |
| **Isobaric process** | A process in which the pressure stays constant throughout ($\Delta P = 0$) |
| **Isovolumetric process** | A process during which the volume does not change ($\Delta V = 0$); also called isochoric |
| **Adiabatic process** | A process with no heat transfer between the system and its environment ($Q = 0$) |
| **Specific heat capacity ($c$)** | The amount of heat energy needed to raise one kilogram of a substance by one kelvin |
| **Thermal conductivity ($k$)** | A material constant indicating how readily thermal energy passes through a given substance |
| **Entropy ($S$)** | A thermodynamic state function counting the number of accessible microscopic arrangements; higher entropy corresponds to greater energy dispersal among microstates |
| **Heat engine** | Any device that extracts useful mechanical work from heat by drawing energy from a hot source and expelling waste heat to a cooler sink |
| **Carnot engine** | An idealized fully reversible engine operating between two fixed-temperature reservoirs; its efficiency is the highest theoretically attainable |

## Common Misconceptions

1. **Heat and temperature are the same thing** -- These are fundamentally different quantities. Temperature reflects how energetically molecules move on average, whereas heat is energy flowing from one object to another because they differ in temperature. A bathtub and a coffee mug can share the same temperature, yet the bathtub holds far more internal energy due to its greater mass.
2. **Cold flows into an object** -- "Cold" is not a physical substance that travels. Only heat moves, and it always travels from the warmer object to the cooler one. Gripping an ice cube withdraws heat from your hand rather than injecting cold into it.
3. **An ideal gas can be cooled to absolute zero** -- Extrapolating $PV = nRT$ to $T = 0$ K predicts an impossible zero volume or pressure. In practice, real gases condense into liquids long before reaching this limit, and the third law of thermodynamics establishes that absolute zero itself is unreachable in any finite process.
4. **Work done by a gas depends only on initial and final states** -- Unlike internal energy, work is path-dependent. An isothermal path and an adiabatic path between identical endpoints yield different amounts of work, as revealed by the different areas they sweep beneath their respective curves on a PV diagram.
5. **A system at thermal equilibrium has no molecular motion** -- Thermal equilibrium means no net energy transfer occurs, not that all motion has ceased. Molecules continue their random thermal motion; the equilibrium condition is simply that every exchange of energy between system and surroundings is balanced by an equal reverse exchange.
6. **Entropy always means disorder** -- "Disorder" is a helpful but imprecise shorthand. Entropy is formally defined by counting the microstates compatible with a given macrostate. A better framing is that entropy measures how broadly energy is dispersed across the available microscopic configurations.
7. **A heat engine can be 100% efficient** -- The second law rules this out. Even a perfect Carnot engine must expel some heat to a cold reservoir; as long as $T_C > 0$ K, the Carnot formula $e = 1 - T_C/T_H$ gives a value strictly less than 1 for any realizable pair of reservoirs.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Temperature | K (kelvin) | [$\Theta$] |
| Pressure | Pa (pascal) = N/m$^2$ = kg/(m·s$^2$) | [M][L]$^{-1}$[T]$^{-2}$ |
| Volume | m$^3$ | [L]$^3$ |
| Internal energy | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Heat | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Work | J (joule) | [M][L]$^2$[T]$^{-2}$ |
| Specific heat capacity | J/(kg·K) | [L]$^2$[T]$^{-2}$[$\Theta$]$^{-1}$ |
| Thermal conductivity | W/(m·K) = kg·m/(s$^3$·K) | [M][L][T]$^{-3}$[$\Theta$]$^{-1}$ |
| Entropy | J/K | [M][L]$^2$[T]$^{-2}$[$\Theta$]$^{-1}$ |
| Boltzmann constant ($k_B$) | J/K | [M][L]$^2$[T]$^{-2}$[$\Theta$]$^{-1}$ |
| Gas constant ($R$) | J/(mol·K) | [M][L]$^2$[T]$^{-2}$[$\Theta$]$^{-1}$[N]$^{-1}$ |
| Efficiency | dimensionless | -- |
