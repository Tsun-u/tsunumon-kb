# Unit 4: Linear Momentum

> Exam Weight: 10--15% | ~10--15 Class Periods

## Topics

### 4.1 Linear Momentum
- Linear momentum: $\vec{p} = m\vec{v}$
- Momentum is a vector quantity; direction same as velocity
- Momentum of a system: $\vec{p}_{sys} = \sum m_i \vec{v}_i$
- A system's total momentum equals the product of total mass and velocity of center of mass: $\vec{p}_{sys} = M\vec{v}_{cm}$

### 4.2 Change in Momentum and Impulse
- Impulse: $\vec{J} = \vec{F}_{avg} \Delta t$
- Impulse-momentum theorem: $\vec{J} = \Delta \vec{p} = \vec{p}_f - \vec{p}_i$
- Newton's second law in momentum form: $\vec{F}_{net} = \frac{d\vec{p}}{dt} \approx \frac{\Delta \vec{p}}{\Delta t}$
- Impulse equals the area under a force-time graph
- To reduce force during a collision: increase the time of interaction (e.g., airbags, crumple zones)

### 4.3 Conservation of Linear Momentum
- If the net external force on a system is zero, total momentum is conserved: $\vec{p}_i = \vec{p}_f$
- Applies to all types of collisions and explosions
- **Elastic collision**: both momentum and kinetic energy are conserved
- **Inelastic collision**: momentum is conserved, kinetic energy is NOT conserved (some KE converted to thermal/deformation energy)
- **Perfectly inelastic collision**: objects stick together; maximum KE loss; $m_1\vec{v}_1 + m_2\vec{v}_2 = (m_1+m_2)\vec{v}_f$
- **Explosion**: objects initially at rest separate; momentum conserved ($\vec{p}_i = 0$, so $\vec{p}_f = 0$)
- Conservation applies independently in x and y directions for 2D collisions

## Learning Objectives

- Calculate the momentum of an object or system of objects
- Apply the impulse-momentum theorem to determine changes in momentum
- Use force-time graphs to determine impulse
- Apply conservation of linear momentum to collisions and explosions
- Distinguish between elastic, inelastic, and perfectly inelastic collisions
- Analyze 2D collisions using component-wise momentum conservation
- Explain real-world applications of impulse (safety devices)
- Predict the velocity of objects after collisions

## Essential Knowledge

1. Momentum is a vector quantity defined as the product of mass and velocity
2. A net force acting over a time interval produces an impulse that changes an object's momentum
3. Newton's second law can be expressed as the rate of change of momentum
4. In a closed system (no net external force), total momentum is conserved
5. Momentum conservation applies to all collisions regardless of whether kinetic energy is conserved
6. In elastic collisions, both momentum and kinetic energy are conserved
7. In perfectly inelastic collisions, objects stick together and kinetic energy is at a minimum (but not zero unless both initially at rest)
8. The velocity of the center of mass of a system is unchanged by internal forces

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
| **Linear momentum ($\vec{p}$)** | Product of mass and velocity; vector quantity |
| **Impulse ($\vec{J}$)** | Product of average force and time interval; equals change in momentum |
| **Elastic collision** | Collision in which both momentum and kinetic energy are conserved |
| **Inelastic collision** | Collision in which momentum is conserved but kinetic energy is not |
| **Perfectly inelastic** | Collision where objects stick together; maximum KE loss |
| **Explosion** | Event where initially combined objects separate; reverse of perfectly inelastic collision |
| **Closed/isolated system** | System with no net external force (or negligible external forces during collision) |
| **Center of mass** | Point at which the total mass of a system can be considered concentrated |
| **Internal forces** | Forces between objects within the system (do not change total momentum) |
| **External forces** | Forces from outside the system (can change total momentum) |

## Common Misconceptions

1. **Momentum is the same as kinetic energy** -- No. Momentum is $\vec{p} = m\vec{v}$ (vector); KE is $K = \frac{1}{2}mv^2$ (scalar). They are independently conserved only in elastic collisions.
2. **Momentum is always conserved** -- Only when net external force is zero. During a collision, if external forces (like friction with the ground) are negligible during the short collision time, momentum is approximately conserved.
3. **In a perfectly inelastic collision, all KE is lost** -- Not necessarily. Only the maximum possible amount of KE is lost (converted to other forms). KE is zero only if $\vec{p}_i = 0$.
4. **A lighter object always bounces back in a collision** -- Only when it hits a much more massive, essentially stationary object.
5. **Force is the same as impulse** -- Impulse includes time. A small force over a long time can produce the same impulse as a large force over a short time.
6. **Momentum is always conserved in each direction separately** -- Yes, this is correct. But students often forget to apply conservation component-wise in 2D.
7. **Heavier objects always have more momentum** -- Not necessarily. A light fast object can have more momentum than a heavy slow one.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Momentum | kg$\cdot$m/s = N$\cdot$s | [M][L][T]$^{-1}$ |
| Impulse | N$\cdot$s = kg$\cdot$m/s | [M][L][T]$^{-1}$ |
| Force | N | [M][L][T]$^{-2}$ |
| Time | s | [T] |
| Kinetic energy | J | [M][L]$^2$[T]$^{-2}$ |
