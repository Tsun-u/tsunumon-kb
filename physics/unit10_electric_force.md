# Unit 10: Electric Force, Field, and Potential

> Exam Weight: 15--18% | ~14--21 Class Periods

## Topics

### 10.1 Electric Charge and Electric Force
- Matter possesses two varieties of electric charge, labeled positive and negative
- Elementary charge: $e = 1.6 \times 10^{-19}$ C (magnitude of charge on a proton or electron)
- Proton charge: $+e$; electron charge: $-e$
- Two charges of the same sign push each other apart; charges of opposite sign pull each other together
- Coulomb's law gives the magnitude of the electric force between two point charges:

$$F_E = k \frac{|q_1||q_2|}{r^2}$$

- Coulomb constant: $k = 8.99 \times 10^9 \text{ N·m}^2/\text{C}^2$
- Equivalently, $k = \frac{1}{4\pi\varepsilon_0}$, where $\varepsilon_0 = 8.85 \times 10^{-12} \text{ C}^2/\text{(N·m}^2\text{)}$
- The electrostatic force is a vector directed along the straight line joining the two charges
- Coulomb's law shares the inverse-square distance dependence of Newton's gravitational law, but unlike gravity it can produce either attraction or repulsion depending on the charge signs
- Superposition: the total electric force on any one charge equals the vector sum of all the individual Coulomb forces exerted on it by every other charge

### 10.2 Conservation of Electric Charge and the Process of Charging
- Electric charge is conserved: no process within an isolated system can alter its total electric charge
- Charge is quantized: every detectable amount of charge is an integer multiple of $e$; fractional free charges do not exist
- Conductors: materials in which charge carriers move freely throughout the bulk (metals, ionic solutions)
- Insulators: materials in which electrons are tightly bound and resist moving (rubber, glass, plastic)
- Charging by friction: when two different materials are rubbed together, electrons transfer from one surface to the other, leaving both objects charged
- Charging by contact: a charged object physically touches a neutral conductor, sharing some of its charge and leaving both objects with the same sign of charge
- Charging by induction: a nearby charged object pushes mobile charges to one side of a neutral conductor; grounding then removes the repelled charges, leaving the conductor with net charge of the opposite sign
- Grounding: a conducting path to a large charge reservoir (typically Earth) lets excess charge drain away until the object is neutralized
- Polarization: an external electric field temporarily shifts the distribution of charge within a neutral insulator without actually moving charges through it; this induced asymmetry is what draws neutral objects toward a nearby charged one

### 10.3 Electric Fields
- Any charged object modifies the space around it, establishing an electric field $\vec{E}$ that other charges can sense
- Definition of electric field at a point:

$$\vec{E} = \frac{\vec{F}_E}{q_{\text{test}}}$$

- where $q_{\text{test}}$ is a small positive test charge and $\vec{F}_E$ is the force on it
- Electric field due to a point charge:

$$E = k \frac{|q|}{r^2}$$

- The field radiates outward from a positive source charge and converges inward toward a negative one
- Electric field lines:
  - Originate on positive charges, terminate on negative charges
  - Density of field lines indicates field strength
  - Field lines never cross
  - Tangent to a field line at any point gives the direction of $\vec{E}$
- When multiple charges are present, the total electric field at any point is the vector sum of the individual contributions—superposition applies
- Uniform electric field between parallel plates:

$$E = \frac{V}{d}$$

- where $V$ is the potential difference and $d$ is the plate separation
- Inside a conductor that has reached electrostatic equilibrium, the net electric field is zero—any nonzero field would drive charge motion until it vanished
- Any surplus charge on a conductor collects on its outer surface, not in its interior

### 10.4 Electric Potential Energy
- Electric potential energy of a system of two point charges:

$$U_E = k \frac{q_1 q_2}{r}$$

- The signed product $q_1 q_2$ automatically captures the physics: $U_E > 0$ when both charges share the same sign (energy stored in repulsion), and $U_E < 0$ when they are opposite in sign (energy released in attraction)
- The zero reference is set at infinite separation: $U_E \to 0$ as $r \to \infty$
- Work done by the electric force:

$$W_E = -\Delta U_E = -(U_f - U_i)$$

- In a uniform electric field, the potential energy of a charge $q$ is:

$$U_E = qEd$$

- where $d$ is the displacement in the direction of $\vec{E}$ (measured from a chosen reference)
- A positive charge sitting in a uniform field carries more potential energy when it has been pushed against the field; released from rest, it accelerates along $\vec{E}$ toward lower potential energy

### 10.5 Electric Potential
- Electric potential (voltage) normalizes potential energy by the charge that holds it:

$$V = \frac{U_E}{q}$$

- Electric potential due to a point charge:

$$V = k \frac{q}{r}$$

- Because potential is a scalar, the total potential at any point from several charges is just their arithmetic sum—no vector angles to track
- Potential difference (voltage) between two points:

$$\Delta V = V_B - V_A = -\frac{W_{A \to B}}{q}$$

- where $W_{A \to B}$ is the work done by the electric force moving charge $q$ from $A$ to $B$
- Relationship between electric field and potential:

$$E = -\frac{\Delta V}{\Delta r}$$

- The electric field always aims toward lower potential; steep potential gradients correspond to strong fields
- Equipotential lines (surfaces):
  - Curves (or surfaces in 3D) along which $V$ is everywhere the same
  - Always perpendicular to electric field lines
  - Moving a charge along an equipotential requires zero work by the electric force
  - Tightly bunched equipotentials signal a large field in that region

### 10.6 Capacitors
- A capacitor consists of two conductors separated by a gap; it holds separated charge and, in doing so, stores energy in the electric field between them
- Capacitance quantifies how much charge accumulates per volt of applied potential difference:

$$C = \frac{Q}{V}$$

- Unit: farad (F), where $1 \text{ F} = 1 \text{ C/V}$
- Capacitance of a parallel-plate capacitor:

$$C = \varepsilon_0 \frac{A}{d}$$

- where $A$ is the plate area and $d$ is the plate separation
- Energy stored in a capacitor:

$$U_C = \frac{1}{2}CV^2 = \frac{1}{2}QV = \frac{Q^2}{2C}$$

- Dielectrics: insulating materials inserted between capacitor plates
  - Increase capacitance by a factor $\kappa$ (dielectric constant):

$$C_{\text{dielectric}} = \kappa C_0 = \kappa \varepsilon_0 \frac{A}{d}$$

  - The polarized dielectric partially cancels the internal field, weakening $E$ between the plates
  - When charge is fixed (capacitor disconnected before insertion): adding a dielectric lowers $V$ and thereby reduces stored energy
  - When voltage is fixed (capacitor remains connected to a battery): adding a dielectric draws in more charge, increasing stored energy

### 10.7 Conservation of Electric Energy
- Total mechanical energy is conserved as a charged particle travels through an electric field:

$$K_i + U_{E,i} = K_f + U_{E,f}$$

- Equivalently, using potential difference:

$$\Delta K = q \Delta V \quad \text{(for charge } q \text{ through potential difference } \Delta V\text{)}$$

- The work-energy theorem for a charge in an electric field:

$$W_E = \Delta K = q(V_i - V_f) = -q \Delta V$$

- The electron volt (eV) is a convenient energy unit:

$$1 \text{ eV} = 1.6 \times 10^{-19} \text{ J}$$

- One electron volt is the energy picked up by a single elementary charge crossing a potential difference of exactly 1 V
- A positive charge freed from rest spontaneously speeds up as it moves from high potential toward low potential (losing potential energy, gaining kinetic energy)
- A negative charge freed from rest instead accelerates from low potential toward high potential, since the force on it opposes the field direction

## Skills to Master

- Use Coulomb's law to find the magnitude of the electrostatic force acting between two point charges at a known separation
- Combine individual Coulomb forces by vector superposition to find the net electric force on a charge in a multi-charge arrangement
- Articulate why electric charge is both conserved in isolated systems and quantized in integer multiples of $e$
- Contrast the electrical behavior of conductors and insulators, and trace what happens to charge during friction, contact, and induction charging
- Determine the electric field produced by point charges and connect field values to the force experienced by a test charge placed in that region
- Draw and read electric field line diagrams for simple charge distributions, extracting both direction and relative strength information
- Characterize the uniform electric field established between two parallel charged plates
- Evaluate the electric potential energy stored in a configuration of point charges
- Compute the electric potential at a point due to one or more point charges, and find the potential difference between two locations
- Translate between electric field values and potential gradients, and use equipotential maps to reason about field geometry
- Solve for capacitance, plate charge, and stored energy in parallel-plate capacitor problems
- Predict how inserting a dielectric affects capacitance, potential difference, and energy, distinguishing the isolated-capacitor and battery-connected cases
- Apply energy conservation to track how kinetic energy changes when a charged particle moves through a potential difference

## Core Concepts

1. Electric charge is an intrinsic property of certain particles; the total charge of an isolated system never changes, and all observed charges are integer multiples of $e = 1.6 \times 10^{-19}$ C
2. Coulomb's law gives an inverse-square electrostatic force that mirrors Newton's gravitational law in mathematical form, but with the added feature that it can push charges apart as well as pull them together
3. The electric field at any point is defined as the electrostatic force per unit positive charge placed there; fields from individual sources add as vectors following the superposition principle
4. Electric field line diagrams encode both direction (tangent to lines) and relative field strength (spacing between lines); lines leave positive charges and arrive at negative charges
5. Within a conductor at electrostatic equilibrium, the internal electric field is exactly zero; any net charge distributes itself entirely on the outer surface
6. Electric potential is a scalar obtained by dividing potential energy by charge; this makes it additive without vector bookkeeping, so potentials from several sources simply sum numerically
7. The electric field vector always points in the direction of steepest potential decrease; equipotential surfaces, where potential is uniform, cut the field lines at right angles
8. The capacitance of a parallel-plate capacitor is set by its physical geometry—plate area and gap width—as well as the dielectric constant of whatever fills the gap
9. A charged capacitor stores energy within the electric field it maintains; this energy can be written equivalently in terms of $C$, $Q$, or $V$
10. As a charged particle moves through an electric field, total mechanical energy is conserved: any gain in kinetic energy comes at the expense of an equal drop in electric potential energy

## Key Equations

### Coulomb's Law

$$F_E = k \frac{|q_1||q_2|}{r^2}, \quad k = 8.99 \times 10^9 \text{ N·m}^2/\text{C}^2$$

### Electric Field

$$\vec{E} = \frac{\vec{F}_E}{q_{\text{test}}}$$

$$E = k \frac{|q|}{r^2} \quad \text{(point charge)}$$

$$E = \frac{V}{d} \quad \text{(uniform field, parallel plates)}$$

### Electric Potential Energy

$$U_E = k \frac{q_1 q_2}{r} \quad \text{(two point charges)}$$

### Electric Potential

$$V = \frac{U_E}{q}$$

$$V = k \frac{q}{r} \quad \text{(point charge)}$$

$$E = -\frac{\Delta V}{\Delta r}$$

### Capacitance and Stored Energy

$$C = \frac{Q}{V}$$

$$C = \varepsilon_0 \frac{A}{d} \quad \text{(parallel plates)}$$

$$C_{\text{dielectric}} = \kappa \varepsilon_0 \frac{A}{d}$$

$$U_C = \frac{1}{2}CV^2 = \frac{1}{2}QV = \frac{Q^2}{2C}$$

### Energy Conservation

$$K_i + U_{E,i} = K_f + U_{E,f}$$

$$1 \text{ eV} = 1.6 \times 10^{-19} \text{ J}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Electric charge** | An intrinsic property of matter that comes in positive and negative varieties and is measured in coulombs (C) |
| **Elementary charge** | The indivisible unit of charge carried by a single proton or electron: $e = 1.6 \times 10^{-19}$ C |
| **Coulomb's law** | The quantitative rule for the force between two point charges: $F = k |q_1| |q_2| / r^2$ |
| **Conductor** | A substance whose charge carriers can shift position freely in response to an electric force |
| **Insulator** | A substance in which charge carriers are tightly bound and cannot move freely |
| **Electric field** | A vector quantity at each point in space equal to the electrostatic force a unit positive charge would experience there: $\vec{E} = \vec{F}/q$ |
| **Field lines** | Directed curves that map the electric field; a tangent at any point gives the field direction, and line density reflects field strength |
| **Electric potential energy** | The configuration-dependent energy held by a system of charges by virtue of their positions relative to one another |
| **Electric potential (voltage)** | The electric potential energy per unit charge at a location: $V = U_E / q$; measured in volts (V) |
| **Potential difference** | The change in electric potential from one point to another: $\Delta V = V_B - V_A$ |
| **Equipotential line** | A curve (or surface in 3D) on which electric potential has the same value everywhere; always perpendicular to $\vec{E}$ |
| **Capacitance** | How much charge a device accumulates per volt of potential difference applied: $C = Q/V$; measured in farads (F) |
| **Dielectric** | An insulating medium inserted between capacitor plates that multiplies capacitance by its dielectric constant $\kappa$ |
| **Electron volt (eV)** | A convenient energy unit equal to the work done accelerating one electron through 1 V: $1 \text{ eV} = 1.6 \times 10^{-19}$ J |
| **Grounding** | Electrically linking an object to a large charge reservoir (typically Earth) so that excess charge can freely drain away |

## Common Misconceptions

1. **Electric field lines are the paths that charges follow** -- Field lines indicate the direction of instantaneous force on a positive test charge, not the trajectory the charge will trace. A charge in motion already carries momentum, so its actual path is shaped by both its initial velocity and the local field direction—typically resulting in a curve rather than a straight field line.
2. **Electric potential and electric field are the same thing** -- These are separate physical quantities. $\vec{E}$ is a vector (units N/C or V/m) describing force per charge at a point, whereas $V$ is a scalar (units J/C or V) describing energy per charge. They are connected through $E = -\Delta V / \Delta r$, but knowing one does not by itself tell you the value of the other.
3. **A point with zero electric field must have zero electric potential** -- Not true. At the midpoint between two identical positive charges, the electric fields from each charge point in opposite directions and cancel ($\vec{E} = 0$), yet the potential contributions from both charges are positive and add together ($V > 0$).
4. **A point with zero electric potential must have zero electric field** -- Not true. At the midpoint between a $+q$ and $-q$ pair of equal magnitude, the potentials cancel ($V = 0$), but the electric fields from both charges point in the same direction and reinforce, giving $\vec{E} \neq 0$.
5. **Electric potential energy belongs to a single charge** -- Potential energy is a property of the interaction between charges, not of any individual charge in isolation. It takes at least two charged objects to define a meaningful electric potential energy; removing one charge makes the concept inapplicable.
6. **A capacitor stores charge; one plate has more charge than the other** -- The two plates always carry equal magnitudes of charge with opposite signs ($+Q$ and $-Q$), so the net stored charge is zero. The $Q$ appearing in $C = Q/V$ denotes the charge magnitude on one plate only, not any net charge on the device.
7. **Inserting a dielectric always increases the energy stored in a capacitor** -- The outcome depends on the electrical boundary condition. With the capacitor isolated (fixed $Q$), a dielectric lowers the voltage across the plates, reducing stored energy. With the capacitor still attached to a battery (fixed $V$), more charge flows in, increasing stored energy. The two scenarios give opposite results.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Electric charge | C (coulomb) | [A][T] |
| Electric force | N (newton) | [M][L][T]$^{-2}$ |
| Electric field | N/C = V/m | [M][L][A]$^{-1}$[T]$^{-3}$ |
| Electric potential (voltage) | V (volt) = J/C | [M][L]$^{2}$[A]$^{-1}$[T]$^{-3}$ |
| Electric potential energy | J (joule) | [M][L]$^{2}$[T]$^{-2}$ |
| Capacitance | F (farad) = C/V | [A]$^{2}$[T]$^{4}$[M]$^{-1}$[L]$^{-2}$ |
| Permittivity ($\varepsilon_0$) | C$^2$/(N·m$^2$) = F/m | [A]$^{2}$[T]$^{4}$[M]$^{-1}$[L]$^{-3}$ |
| Coulomb constant ($k$) | N·m$^2$/C$^2$ | [M][L]$^{3}$[A]$^{-2}$[T]$^{-4}$ |
| Energy (electron volt) | eV ($1.6 \times 10^{-19}$ J) | [M][L]$^{2}$[T]$^{-2}$ |
