# Unit 4: Linear Momentum

> Exam Weight: 10--15% | ~10--15 Class Periods

## Topics

### 4.1 Linear Momentum
- Linear momentum: $\vec{p} = m\vec{v}$
- Momentum is a vector; it points in the same direction as the object's velocity
- Total momentum of a system: $\vec{p}_{sys} = \sum m_i \vec{v}_i$
- A system's total momentum can also be written as the total mass times the velocity of the center of mass: $\vec{p}_{sys} = M\vec{v}_{cm}$

### 4.2 Change in Momentum and Impulse
- Impulse: $\vec{J} = \vec{F}_{avg} \Delta t$
- Impulse-momentum theorem: $\vec{J} = \Delta \vec{p} = \vec{p}_f - \vec{p}_i$
- Newton's second law expressed in terms of momentum: $\vec{F}_{net} = \frac{d\vec{p}}{dt} \approx \frac{\Delta \vec{p}}{\Delta t}$
- The impulse delivered by a varying force equals the area enclosed beneath the force-time graph
- Extending the duration of a collision reduces the peak force involved (e.g., airbags, crumple zones extend impact time)

### 4.3 Conservation of Linear Momentum
- When the net external force on a system is zero, the system's total momentum does not change: $\vec{p}_i = \vec{p}_f$
- This principle holds for all collision and explosion scenarios
- **Elastic collision**: both momentum and kinetic energy remain conserved throughout
- **Inelastic collision**: momentum is conserved, but kinetic energy decreases as some is converted to thermal or deformation energy
- **Perfectly inelastic collision**: the colliding objects merge into one; kinetic energy loss is maximized; $m_1\vec{v}_1 + m_2\vec{v}_2 = (m_1+m_2)\vec{v}_f$
- **Explosion**: a stationary system breaks apart; total momentum remains zero ($\vec{p}_i = 0$, therefore $\vec{p}_f = 0$)
- In two-dimensional situations, momentum conservation is applied separately along each coordinate axis

## Skills to Master

- Compute the momentum of a single object or a collection of objects in a system
- Use the impulse-momentum theorem to find how much an object's momentum changes
- Extract impulse values from force-time graphs by calculating the area under the curve
- Solve collision and explosion problems by applying conservation of linear momentum
- Categorize a collision as elastic, inelastic, or perfectly inelastic based on what quantities are conserved
- Handle two-dimensional collision problems by resolving momentum into perpendicular components
- Connect impulse principles to the design of safety systems (airbags, padding, crumple zones)
- Determine the post-collision velocities of objects given initial conditions and collision type

## Core Concepts

1. Momentum is a vector property of a moving object, calculated by multiplying its mass by its velocity
2. Applying a net force over some time interval delivers an impulse, which is exactly equal to the resulting change in momentum
3. Newton's second law can be reformulated to state that the net force on an object equals the time rate of change of its momentum
4. When no net external force acts on a system, the system's total momentum is conserved — its value before and after any internal event remains the same
5. Momentum conservation governs all types of collisions; kinetic energy conservation is an additional constraint that only some collisions satisfy
6. An elastic collision is one in which both total momentum and total kinetic energy are the same before and after the event
7. In a perfectly inelastic collision the objects lock together, and this configuration produces the greatest possible reduction in kinetic energy (though KE is zero only if the combined system is also at rest)
8. Forces between objects within a system are internal forces; they redistribute momentum among members but leave the system's total momentum unaffected

## Key Equations

### Momentum

$$\vec{p} = m\vec{v}$$

$$\vec{p}_{sys} = \sum m_i \vec{v}_i = M\vec{v}_{cm}$$

### Impulse-Momentum Theorem

$$\vec{J} = \vec{F}_{avg} \Delta t = \Delta \vec{p}$$

### Conservation of Momentum

$$\vec{p}_i = \vec{p}_f \quad \text{(when } \sum \vec{F}_{ext} = 0\text{)}$$

$$m_1 \vec{v}_{1i} + m_2 \vec{v}_{2i} = m_1 \vec{v}_{1f} + m_2 \vec{v}_{2f}$$

### Perfectly Inelastic Collision

$$m_1 \vec{v}_{1i} + m_2 \vec{v}_{2i} = (m_1 + m_2)\vec{v}_f$$

### Elastic Collision (1D, two objects)

$$v_{1f} = \frac{m_1 - m_2}{m_1 + m_2}v_{1i} + \frac{2m_2}{m_1 + m_2}v_{2i}$$

$$v_{2f} = \frac{2m_1}{m_1 + m_2}v_{1i} + \frac{m_2 - m_1}{m_1 + m_2}v_{2i}$$

### Kinetic Energy in Collisions

$$K = \frac{1}{2}mv^2 = \frac{p^2}{2m}$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Linear momentum ($\vec{p}$)** | A vector quantity equal to an object's mass multiplied by its velocity |
| **Impulse ($\vec{J}$)** | The product of average force and elapsed time; numerically equal to the change in momentum |
| **Elastic collision** | An interaction where total kinetic energy is preserved alongside total momentum |
| **Inelastic collision** | An interaction where momentum is preserved but some kinetic energy converts to other forms |
| **Perfectly inelastic** | A special inelastic case where the objects combine into one body, yielding the largest possible KE loss |
| **Explosion** | A process where a single body or system breaks into separate pieces; the time-reverse of a perfectly inelastic collision |
| **Closed/isolated system** | A system experiencing no net external force, so its total momentum cannot change |
| **Center of mass** | The single location where a system's entire mass can be treated as concentrated for momentum calculations |
| **Internal forces** | Interactions occurring between objects that belong to the same system; they exchange momentum within the system without altering the total |
| **External forces** | Forces originating from agents outside the system boundary; these are the only forces capable of changing the system's total momentum |

## Common Misconceptions

1. **Momentum and kinetic energy are interchangeable concepts** -- They are distinct. Momentum ($\vec{p} = m\vec{v}$) is a vector; kinetic energy ($K = \frac{1}{2}mv^2$) is a scalar. Both are simultaneously conserved only in elastic collisions; in other collisions only momentum is guaranteed to be conserved.
2. **Momentum is always conserved in any situation** -- Momentum is conserved only when the net external force on the system is zero. For a brief collision, external forces like ground friction often act for so short a time that their impulse is negligible, making conservation approximately valid — but it is not universally guaranteed.
3. **A perfectly inelastic collision destroys all kinetic energy** -- This is incorrect in general. The maximum amount of KE that can be lost is lost, but the combined object usually continues moving and retains kinetic energy. Only if the initial total momentum is zero will the final KE also be zero.
4. **A lighter object always rebounds when hit by a heavier one** -- Rebound depends on the mass ratio and the type of collision. A light object bounces back only when striking a significantly more massive object that remains essentially stationary.
5. **Force and impulse mean the same thing** -- Impulse is force multiplied by time, so a weak force sustained over a long period can deliver just as much impulse as a strong force acting briefly. They are related but not identical.
6. **In two dimensions, momentum conservation is applied to the total, not each component** -- In fact, conservation must hold independently along each axis. Students frequently treat 2D problems as if momentum in one equation is enough, missing the need to write separate equations for x and y.
7. **A more massive object inevitably carries more momentum** -- Mass is only one factor. A small but fast-moving object ($m$ small, $v$ large) can exceed the momentum of a large but slow-moving object. What matters is the product $mv$, not mass alone.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Momentum | kg$\cdot$m/s = N$\cdot$s | [M][L][T]$^{-1}$ |
| Impulse | N$\cdot$s = kg$\cdot$m/s | [M][L][T]$^{-1}$ |
| Force | N | [M][L][T]$^{-2}$ |
| Time | s | [T] |
| Kinetic energy | J | [M][L]$^2$[T]$^{-2}$ |
