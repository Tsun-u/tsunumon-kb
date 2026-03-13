# Unit 8: Fluids

> Exam Weight: 10--15% | ~12--17 Class Periods
>
> **New unit added in 2024-25 CED revision.**

## Topics

### 8.1 Internal Structure and Density
- A fluid is any substance that flows and takes the shape of its container (liquids and gases)
- An ideal fluid is incompressible and non-viscous (no internal friction)
- Density: $\rho = \frac{m}{V}$ (mass per unit volume)
- Specific gravity: ratio of a substance's density to the density of water ($\rho_{water} = 1000 \text{ kg/m}^3$)
- Density determines whether objects float or sink:
  - Object floats if $\rho_{object} < \rho_{fluid}$
  - Object sinks if $\rho_{object} > \rho_{fluid}$
  - Object is neutrally buoyant if $\rho_{object} = \rho_{fluid}$

### 8.2 Pressure
- Pressure: $P = \frac{F}{A}$ (force per unit area; scalar)
- SI unit: pascal (Pa) = N/m$^2$
- Pressure at depth in a fluid (gauge pressure): $P_{gauge} = \rho g h$
- Absolute pressure at depth: $P = P_0 + \rho g h$
  - $P_0$ = pressure at the surface (e.g., atmospheric pressure $\approx 1.013 \times 10^5$ Pa)
- Pascal's principle: a change in pressure applied to an enclosed fluid is transmitted equally to every point in the fluid
  - Hydraulic systems: $\frac{F_1}{A_1} = \frac{F_2}{A_2}$
- Pressure acts equally in all directions at a given depth (for a static fluid)

### 8.3 Fluids and Newton's Laws (Buoyancy)
- Buoyant force: net upward force exerted by a fluid on an immersed object
- Caused by the pressure difference between the bottom and top of the object
- **Archimedes' principle**: $F_b = \rho_{fluid} V_{displaced} g$
  - Buoyant force equals the weight of fluid displaced
- For a floating object: $F_b = mg$ (buoyant force equals weight)
  - Fraction submerged: $\frac{V_{submerged}}{V_{total}} = \frac{\rho_{object}}{\rho_{fluid}}$
- For a submerged object: apparent weight = $mg - F_b$

### 8.4 Fluid Flow and Continuity
- Steady (laminar) flow: fluid velocity at each point is constant over time
- Streamlines: paths followed by fluid particles; never cross in steady flow
- **Equation of continuity** (conservation of mass for incompressible fluid):
$$A_1 v_1 = A_2 v_2$$
  - Where $A$ is cross-sectional area and $v$ is fluid speed
  - Fluid speeds up where the pipe narrows
- Volumetric flow rate: $Q = Av$ (constant throughout a pipe)

### 8.5 Bernoulli's Equation
- **Bernoulli's equation** (conservation of energy for ideal fluid flow):
$$P_1 + \frac{1}{2}\rho v_1^2 + \rho g y_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g y_2$$
- Each term represents energy per unit volume:
  - $P$: pressure energy (work done by pressure)
  - $\frac{1}{2}\rho v^2$: kinetic energy per unit volume
  - $\rho g y$: gravitational potential energy per unit volume
- Where fluid speeds up, pressure decreases (and vice versa)
- Special cases:
  - Static fluid ($v = 0$): reduces to $P = P_0 + \rho g h$
  - Horizontal flow ($y_1 = y_2$): $P_1 + \frac{1}{2}\rho v_1^2 = P_2 + \frac{1}{2}\rho v_2^2$
  - Torricelli's theorem (tank draining): $v = \sqrt{2gh}$

## Learning Objectives

- Calculate density and apply it to determine floating/sinking behavior
- Calculate pressure at different depths in a fluid
- Apply Pascal's principle to hydraulic systems
- Calculate buoyant force using Archimedes' principle
- Determine whether an object floats, sinks, or is neutrally buoyant
- Apply the equation of continuity to fluid flow problems
- Apply Bernoulli's equation to analyze fluid flow
- Explain how pressure and velocity are related in flowing fluids

## Essential Knowledge

1. Pressure in a static fluid increases linearly with depth: $P = P_0 + \rho g h$
2. Pascal's principle: pressure changes are transmitted equally throughout an enclosed fluid
3. The buoyant force on an object equals the weight of fluid displaced (Archimedes' principle)
4. For an incompressible fluid in steady flow, the product of cross-sectional area and speed is constant (continuity)
5. Bernoulli's equation expresses conservation of energy per unit volume for ideal fluid flow
6. Where fluid speed increases, pressure decreases (Bernoulli effect)
7. An ideal fluid is incompressible and has no viscosity

## Key Equations

### Density

$$\rho = \frac{m}{V}$$

### Pressure

$$P = \frac{F}{A}$$

$$P = P_0 + \rho g h \quad \text{(pressure at depth)}$$

### Pascal's Principle (Hydraulics)

$$\frac{F_1}{A_1} = \frac{F_2}{A_2}$$

### Buoyancy (Archimedes' Principle)

$$F_b = \rho_{fluid} V_{displaced} g$$

### Equation of Continuity

$$A_1 v_1 = A_2 v_2$$

### Bernoulli's Equation

$$P_1 + \frac{1}{2}\rho v_1^2 + \rho g y_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g y_2$$

### Torricelli's Theorem

$$v = \sqrt{2gh}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Fluid** | Substance that flows and conforms to the shape of its container (liquid or gas) |
| **Ideal fluid** | Incompressible, non-viscous fluid with no internal friction |
| **Density ($\rho$)** | Mass per unit volume; $\rho = m/V$ |
| **Pressure ($P$)** | Force per unit area; scalar quantity |
| **Gauge pressure** | Pressure relative to atmospheric pressure: $P_{gauge} = P - P_{atm}$ |
| **Absolute pressure** | Total pressure including atmospheric: $P_{abs} = P_{atm} + P_{gauge}$ |
| **Buoyant force** | Net upward force exerted by fluid on an immersed or floating object |
| **Archimedes' principle** | Buoyant force equals weight of displaced fluid |
| **Pascal's principle** | Pressure change in enclosed fluid is transmitted equally throughout |
| **Streamline** | Path traced by a fluid particle in steady flow |
| **Laminar flow** | Smooth, orderly flow with well-defined streamlines |
| **Continuity equation** | $A_1v_1 = A_2v_2$; conservation of mass for incompressible flow |
| **Bernoulli's equation** | Energy conservation per unit volume along a streamline |
| **Viscosity** | Internal friction in a fluid; zero for ideal fluids |

## Common Misconceptions

1. **Pressure has a direction** -- Pressure is a scalar. Force due to pressure has direction (perpendicular to surface), but pressure itself acts equally in all directions at a point.
2. **Buoyant force depends on the depth of the object** -- For a fully submerged object, buoyant force depends only on the volume of the object and the fluid density, NOT the depth.
3. **Heavier objects always sink** -- What matters is density, not weight. A large steel ship floats because its average density (including air inside) is less than water.
4. **Bernoulli's equation means faster flow = lower pressure always** -- Only along a streamline at the same height. If heights differ, gravitational PE must be included.
5. **The continuity equation applies to compressible fluids** -- The form $A_1v_1 = A_2v_2$ is only valid for incompressible fluids.
6. **Water pressure depends on the shape of the container** -- Pressure at a given depth depends only on depth, fluid density, and $g$, regardless of container shape (hydrostatic paradox).
7. **Atmospheric pressure pushes things down** -- Atmospheric pressure acts in all directions. It pushes up, down, and sideways equally.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Density | kg/m$^3$ | [M][L]$^{-3}$ |
| Pressure | Pa (pascal) = N/m$^2$ = kg/(m$\cdot$s$^2$) | [M][L]$^{-1}$[T]$^{-2}$ |
| Volume | m$^3$ | [L]$^3$ |
| Flow rate | m$^3$/s | [L]$^3$[T]$^{-1}$ |
| Force | N | [M][L][T]$^{-2}$ |

### Common Pressure Units
| Unit | Value in Pa |
|------|------------|
| 1 atm | 101,325 Pa |
| 1 bar | 100,000 Pa |
| 1 mmHg (torr) | 133.3 Pa |
| 1 psi | 6,895 Pa |
