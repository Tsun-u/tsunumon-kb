# Unit 8: Fluids

> Exam Weight: 10--15% | ~12--17 Class Periods
>
> **Added to the AP Physics 1 course in the 2024-25 curriculum update.**

## Topics

### 8.1 Internal Structure and Density
- Fluids are materials — both liquids and gases — that cannot sustain a shear stress and therefore deform continuously to fill whatever container holds them
- An ideal fluid is treated as perfectly incompressible and free of viscosity (internal frictional resistance)
- Density: $\rho = \frac{m}{V}$ (mass per unit volume)
- Specific gravity: ratio of a substance's density to the density of water ($\rho_{water} = 1000 \text{ kg/m}^3$)
- Whether an object floats or sinks is decided by how its density compares to the surrounding fluid:
  - Object floats if $\rho_{object} < \rho_{fluid}$
  - Object sinks if $\rho_{object} > \rho_{fluid}$
  - Object is neutrally buoyant if $\rho_{object} = \rho_{fluid}$

### 8.2 Pressure
- Pressure: $P = \frac{F}{A}$ (force per unit area; scalar)
- SI unit: pascal (Pa) = N/m$^2$
- Pressure at depth in a fluid (gauge pressure): $P_{gauge} = \rho g h$
- Absolute pressure at depth: $P = P_0 + \rho g h$
  - $P_0$ = pressure at the surface (e.g., atmospheric pressure $\approx 1.013 \times 10^5$ Pa)
- Pascal's principle: any additional pressure introduced at one point in a sealed, static fluid propagates without loss to every other point in that fluid
  - Hydraulic systems: $\frac{F_1}{A_1} = \frac{F_2}{A_2}$
- At any fixed depth inside a static fluid, the pressure is the same in every direction

### 8.3 Fluids and Newton's Laws (Buoyancy)
- Buoyant force: a net upward push that a surrounding fluid exerts on any object immersed within it
- This upward net force arises because fluid pressure is higher at the bottom of the object than at the top, creating an unbalanced pressure force
- **Archimedes' principle**: $F_b = \rho_{fluid} V_{displaced} g$
  - The buoyant force is numerically equal to the gravitational weight of the fluid that the object has pushed aside
- For a floating object: $F_b = mg$ (buoyant force equals weight)
  - Fraction submerged: $\frac{V_{submerged}}{V_{total}} = \frac{\rho_{object}}{\rho_{fluid}}$
- For a fully submerged object: the scale reading (apparent weight) is reduced to $mg - F_b$

### 8.4 Fluid Flow and Continuity
- Steady (laminar) flow: the velocity of the fluid at every fixed location in space does not change as time passes
- Streamlines trace the trajectories of individual fluid particles; in steady flow, two streamlines can never intersect
- **Equation of continuity** (conservation of mass for incompressible fluid):
$$A_1 v_1 = A_2 v_2$$
  - Where $A$ is cross-sectional area and $v$ is fluid speed
  - Because the same volume must pass every cross-section each second, the fluid accelerates wherever the pipe becomes narrower
- Volumetric flow rate: $Q = Av$ (constant throughout a pipe)

### 8.5 Bernoulli's Equation
- **Bernoulli's equation** (conservation of energy for ideal fluid flow):
$$P_1 + \frac{1}{2}\rho v_1^2 + \rho g y_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g y_2$$
- Each term captures a different form of energy stored per unit volume of fluid:
  - $P$: the work-per-volume that pressure forces do on the fluid element
  - $\frac{1}{2}\rho v^2$: kinetic energy per unit volume
  - $\rho g y$: gravitational potential energy per unit volume
- Regions of higher flow speed correspond to regions of lower pressure, and vice versa
- Special cases:
  - Static fluid ($v = 0$): reduces to $P = P_0 + \rho g h$
  - Horizontal flow ($y_1 = y_2$): $P_1 + \frac{1}{2}\rho v_1^2 = P_2 + \frac{1}{2}\rho v_2^2$
  - Torricelli's theorem (tank draining): $v = \sqrt{2gh}$

## Skills to Master

- Use density to predict and quantitatively evaluate whether an object will float, sink, or remain neutrally buoyant
- Compute fluid pressure as a function of depth and distinguish between gauge and absolute pressure
- Leverage Pascal's principle to solve problems involving hydraulic force amplification
- Use Archimedes' principle to find the buoyant force on objects fully or partially submerged in a fluid
- Determine flotation conditions by comparing object and fluid densities and reasoning about displaced volume
- Solve fluid-flow problems using the continuity equation to relate speed and cross-sectional area at different pipe locations
- Employ Bernoulli's equation to connect pressure, speed, and height at two points along a streamline
- Reason qualitatively and quantitatively about the inverse relationship between flow speed and pressure in an ideal fluid

## Core Concepts

1. In a fluid at rest, pressure grows in direct proportion to depth below the surface, following $P = P_0 + \rho g h$
2. Pascal's principle states that a pressure increase applied at any point of a confined static fluid shows up with the same magnitude at every other point in that fluid
3. Archimedes' principle: the upward buoyant force acting on an object submerged in a fluid is exactly equal to the weight of the fluid volume that the object has displaced
4. For an incompressible fluid moving in steady flow, the continuity condition requires that the product $Av$ remain the same at every cross-section of a pipe
5. Bernoulli's equation is an expression of mechanical energy conservation per unit volume applied to a parcel of ideal fluid moving along a streamline
6. As an ideal fluid accelerates through a constriction, its pressure drops — a consequence of Bernoulli's equation known as the Bernoulli effect
7. The ideal fluid model assumes the fluid cannot be compressed and flows without any internal frictional (viscous) resistance

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
| **Fluid** | Any material (liquid or gas) that flows freely and assumes the shape of its container because it cannot resist shear stress |
| **Ideal fluid** | A theoretical fluid model that is perfectly incompressible and entirely free of viscous (internal friction) effects |
| **Density ($\rho$)** | The amount of mass packed into each unit of volume; $\rho = m/V$ |
| **Pressure ($P$)** | The perpendicular force exerted per unit area on a surface; a scalar with no directional attribute of its own |
| **Gauge pressure** | The pressure measured above atmospheric baseline: $P_{gauge} = P - P_{atm}$ |
| **Absolute pressure** | The complete pressure including the atmospheric contribution: $P_{abs} = P_{atm} + P_{gauge}$ |
| **Buoyant force** | The net upward force that a fluid exerts on any object partially or wholly submerged within it |
| **Archimedes' principle** | The buoyant force on an object equals the weight of the fluid volume the object displaces |
| **Pascal's principle** | Any pressure change introduced into a confined fluid propagates uniformly to all parts of the fluid |
| **Streamline** | The trajectory followed by a single fluid particle in steady flow; a visual map of flow direction at each point |
| **Laminar flow** | Orderly, layered fluid motion in which adjacent layers slide past each other without mixing |
| **Continuity equation** | $A_1v_1 = A_2v_2$; expresses conservation of mass for incompressible fluid through a variable-area conduit |
| **Bernoulli's equation** | Relates pressure, kinetic energy density, and gravitational potential energy density at two points on the same streamline in ideal flow |
| **Viscosity** | A fluid's internal resistance to flow arising from intermolecular friction; assumed to be zero in the ideal fluid model |

## Common Misconceptions

1. **Pressure has a direction** -- Pressure itself is a scalar quantity with no direction. The contact force that pressure produces on a surface is directed perpendicular to that surface, but the pressure value at any point in the fluid is the same regardless of the orientation you probe it.
2. **Buoyant force depends on the depth of the object** -- Once an object is fully submerged, the buoyant force depends on the object's volume and the fluid's density, not on how deep the object sits. Moving it deeper changes the absolute pressures on top and bottom equally, so the net upward force stays constant.
3. **Heavier objects always sink** -- The deciding factor is density, not total weight. A steel ship can float because its hull encloses a large air volume, making its overall average density lower than that of water.
4. **Faster flow always means lower pressure** -- This is only guaranteed along a single streamline at constant elevation. When comparing points at different heights, the gravitational potential energy term $\rho g y$ must be included, and the outcome depends on how all three terms in Bernoulli's equation balance.
5. **The continuity equation applies to compressible fluids** -- The simple form $A_1v_1 = A_2v_2$ is derived assuming constant density; it breaks down for compressible flows where density varies along the pipe.
6. **Water pressure depends on the container shape** -- In a static fluid, pressure at a fixed depth is determined solely by that depth, the fluid density, and $g$. The shape or width of the container is irrelevant — this is the hydrostatic paradox.
7. **Atmospheric pressure pushes things down** -- Atmospheric pressure is isotropic: it pushes on every exposed surface with equal magnitude regardless of whether that surface faces up, down, or sideways.

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
