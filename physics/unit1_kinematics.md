# Unit 1: Kinematics

> Exam Weight: 10--15% | ~12--17 Class Periods

## Topics

### 1.1 Scalars and Vectors in One Dimension
- Scalars: quantities with magnitude only (distance, speed, mass, time, energy)
- Vectors: quantities with magnitude and direction (displacement, velocity, acceleration, force)
- Vectors notated with arrow above symbol: $\vec{v}$
- Vectors can be visually modeled as arrows; length proportional to magnitude

### 1.2 Displacement, Velocity, and Acceleration
- Displacement: change in position, $\Delta x = x - x_0$ (vector)
- Average velocity: $\bar{v} = \frac{\Delta x}{\Delta t}$ (vector)
- Instantaneous velocity: velocity at a specific instant; slope of position-time graph
- Average acceleration: $\bar{a} = \frac{\Delta v}{\Delta t}$ (vector)
- Instantaneous acceleration: slope of velocity-time graph

### 1.3 Representing Motion
- Position vs. time graphs: slope = velocity
- Velocity vs. time graphs: slope = acceleration, area under curve = displacement
- Acceleration vs. time graphs: area under curve = change in velocity
- Motion diagrams (dot diagrams): spacing indicates speed, arrows indicate velocity/acceleration

### 1.4 Reference Frames and Relative Motion
- All motion is measured relative to a chosen reference frame
- Relative velocity: $\vec{v}_{AC} = \vec{v}_{AB} + \vec{v}_{BC}$
- Different observers may disagree on velocity but agree on acceleration (in inertial frames)

### 1.5 Vectors and Motion in Two Dimensions
- Vector components: $v_x = v \cos\theta$, $v_y = v \sin\theta$
- Vector magnitude: $v = \sqrt{v_x^2 + v_y^2}$
- Vector direction: $\theta = \tan^{-1}\left(\frac{v_y}{v_x}\right)$
- Projectile motion: horizontal and vertical components are independent
  - Horizontal: $a_x = 0$, constant velocity
  - Vertical: $a_y = -g$, uniformly accelerated

## Learning Objectives

- Describe and represent motion in one and two dimensions using words, diagrams, graphs, and equations
- Distinguish between scalar and vector quantities
- Calculate displacement, velocity, and acceleration from given data or graphs
- Analyze motion graphs to extract physical meaning (slopes, areas)
- Apply kinematic equations to solve problems involving constant acceleration
- Decompose two-dimensional motion into independent components
- Solve projectile motion problems
- Transform between reference frames using relative velocity

## Essential Knowledge

1. Motion can be described by position, velocity, and acceleration, which are interrelated through calculus concepts (slopes and areas on graphs)
2. For constant acceleration, kinematic equations relate position, velocity, acceleration, and time
3. In the absence of air resistance, a projectile near Earth's surface experiences only gravitational acceleration ($g \approx 9.8 \text{ m/s}^2$) directed downward
4. Two-dimensional motion can be analyzed by treating horizontal and vertical components independently
5. The description of motion depends on the observer's reference frame; velocity is relative but acceleration is the same in all inertial frames

## Key Equations

### Kinematic Equations (Constant Acceleration)

$$v_x = v_{x0} + a_x t$$

$$x = x_0 + v_{x0} t + \frac{1}{2} a_x t^2$$

$$v_x^2 = v_{x0}^2 + 2 a_x (x - x_0)$$

$$\bar{v}_x = \frac{v_{x0} + v_x}{2} \quad \text{(only for constant acceleration)}$$

### Vector Components

$$v_x = v \cos\theta, \quad v_y = v \sin\theta$$

$$v = \sqrt{v_x^2 + v_y^2}$$

### Projectile Motion (no air resistance)

$$x = x_0 + v_{x0} t \quad (a_x = 0)$$

$$y = y_0 + v_{y0} t - \frac{1}{2} g t^2 \quad (a_y = -g)$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Distance** | Total path length traveled; scalar, always non-negative |
| **Displacement** | Change in position; vector from initial to final position |
| **Speed** | Magnitude of velocity; scalar |
| **Velocity** | Rate of change of position; vector |
| **Acceleration** | Rate of change of velocity; vector |
| **Instantaneous** | Value at a specific instant in time (limit as $\Delta t \to 0$) |
| **Average** | Value over a finite time interval |
| **Projectile** | Object moving under the influence of gravity alone (no air resistance) |
| **Reference frame** | Coordinate system relative to which motion is described |
| **Free fall** | Motion under gravity alone; $a = g = 9.8 \text{ m/s}^2$ downward |

## Common Misconceptions

1. **Velocity and acceleration must point in the same direction** -- False. An object can have velocity in one direction and acceleration in the opposite direction (e.g., a ball thrown upward is still decelerating while moving up).
2. **Zero velocity means zero acceleration** -- False. At the top of a projectile's path, $v_y = 0$ but $a_y = -g$.
3. **Heavier objects fall faster** -- False (in absence of air resistance). All objects have the same gravitational acceleration $g$.
4. **Acceleration means speeding up** -- Not necessarily. Negative acceleration (deceleration) means slowing down in the positive direction, or speeding up in the negative direction.
5. **Projectile motion is not "free fall"** -- Projectile motion IS free fall in two dimensions. The horizontal component simply has zero acceleration.
6. **Distance = magnitude of displacement** -- Only true for straight-line motion in one direction. For any path with direction changes, distance > |displacement|.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Position / Displacement | m (meter) | [L] |
| Velocity | m/s | [L][T]$^{-1}$ |
| Acceleration | m/s$^2$ | [L][T]$^{-2}$ |
| Time | s (second) | [T] |
| Angle | rad (radian) | dimensionless |
