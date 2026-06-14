# Unit 1: Kinematics

> Exam Weight: 10--15% | ~12--17 Class Periods

## Topics

### 1.1 Scalars and Vectors in One Dimension
- Scalars have magnitude but no direction (examples: distance, speed, mass, time, energy)
- Vectors carry both magnitude and direction (examples: displacement, velocity, acceleration, force)
- A vector is written with an arrow over the symbol: $\vec{v}$
- Graphically, vectors appear as arrows whose length encodes the magnitude

### 1.2 Displacement, Velocity, and Acceleration
- Displacement measures the net change in position: $\Delta x = x - x_0$ (vector quantity)
- Average velocity equals displacement divided by elapsed time: $\bar{v} = \frac{\Delta x}{\Delta t}$ (vector)
- Instantaneous velocity is the value at one particular moment; it equals the slope on a position-time graph
- Average acceleration equals the velocity change divided by elapsed time: $\bar{a} = \frac{\Delta v}{\Delta t}$ (vector)
- Instantaneous acceleration corresponds to the slope at any point on a velocity-time graph

### 1.3 Representing Motion
- On a position-time graph, the slope at any point gives velocity
- A velocity-time graph encodes acceleration as slope and displacement as the area enclosed under the curve
- An acceleration-time graph: the area under the curve equals the change in velocity
- Dot (motion) diagrams show an object's successive positions; dot spacing reflects speed, and arrows convey velocity or acceleration direction

### 1.4 Reference Frames and Relative Motion
- Every measurement of motion is made with respect to a selected reference frame
- Relative velocity between two objects: $\vec{v}_{AC} = \vec{v}_{AB} + \vec{v}_{BC}$
- Observers in different inertial frames may report different velocities for the same object, yet they agree on acceleration

### 1.5 Vectors and Motion in Two Dimensions
- A vector is projected onto coordinate axes: $v_x = v \cos\theta$, $v_y = v \sin\theta$
- The vector's magnitude is recovered via: $v = \sqrt{v_x^2 + v_y^2}$
- The vector's angle with respect to the x-axis: $\theta = \tan^{-1}\left(\frac{v_y}{v_x}\right)$
- In projectile motion the horizontal and vertical motions are fully independent of each other
  - Horizontal: $a_x = 0$, constant velocity
  - Vertical: $a_y = -g$, uniformly accelerated

## Skills to Master

- Express and model motion in one and two dimensions through multiple representations: words, diagrams, graphs, and equations
- Differentiate between scalar and vector quantities by identifying whether direction is involved
- Compute displacement, velocity, and acceleration from provided data sets or graphical information
- Interpret motion graphs to extract kinematic information encoded as slopes and enclosed areas
- Use the kinematic equations to find unknown quantities when acceleration is constant
- Separate two-dimensional motion into independent horizontal and vertical components
- Tackle projectile motion problems by treating each dimension separately
- Convert velocity descriptions between different reference frames using vector addition

## Core Concepts

1. Position, velocity, and acceleration are linked quantities; on a graph, velocity is the slope of the position curve and acceleration is the slope of the velocity curve, while areas under curves give the reverse relationship
2. When an object undergoes constant acceleration, a set of kinematic equations connects position, velocity, acceleration, and elapsed time
3. A projectile released near Earth's surface with no air resistance is subject only to downward gravitational acceleration ($g \approx 9.8 \text{ m/s}^2$); no horizontal acceleration acts on it
4. Solving two-dimensional motion problems becomes tractable by separating the motion into x and y components and treating each independently
5. How motion appears depends on which reference frame the observer occupies; measured velocities differ between frames, but all inertial observers agree on the acceleration of any given object

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
| **Distance** | The total length of the path an object follows; a scalar that is never negative |
| **Displacement** | The straight-line shift from an object's initial to final position; a vector |
| **Speed** | How fast an object moves regardless of direction; the scalar magnitude of velocity |
| **Velocity** | The rate at which position changes with time; a vector quantity |
| **Acceleration** | The rate at which velocity changes with time; a vector quantity |
| **Instantaneous** | The value of a quantity at one precise moment in time (mathematically, the limit as $\Delta t \to 0$) |
| **Average** | A quantity computed over a specified, finite time interval |
| **Projectile** | Any object whose only source of acceleration during flight is gravity (air resistance neglected) |
| **Reference frame** | The coordinate system an observer uses to measure and describe motion |
| **Free fall** | Motion in which gravity provides the sole acceleration; $a = g = 9.8 \text{ m/s}^2$ directed downward |

## Common Misconceptions

1. **Velocity and acceleration must point in the same direction** -- This is incorrect. Velocity and acceleration are independent vectors; a ball thrown upward, for instance, moves upward while gravity accelerates it downward simultaneously.
2. **Zero velocity means zero acceleration** -- This is incorrect. A projectile momentarily has $v_y = 0$ at the peak of its arc, yet gravity still gives it $a_y = -g$ at that very instant.
3. **Heavier objects fall faster** -- This is incorrect when air resistance is absent. Every object near Earth's surface gains speed at the same rate $g$, regardless of mass.
4. **Acceleration means speeding up** -- Not always. When acceleration opposes the direction of motion the object slows down; when it aligns with motion the object speeds up. The sign (or direction) determines the effect.
5. **Projectile motion is not "free fall"** -- Projectile motion is in fact free fall extended into two dimensions. Gravity acts vertically at all times; the horizontal direction simply has no acceleration component.
6. **Distance = magnitude of displacement** -- This equality holds only for straight-line travel in a single direction. Whenever the path bends or reverses, the total distance walked exceeds the straight-line displacement magnitude.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Position / Displacement | m (meter) | [L] |
| Velocity | m/s | [L][T]$^{-1}$ |
| Acceleration | m/s$^2$ | [L][T]$^{-2}$ |
| Time | s (second) | [T] |
| Angle | rad (radian) | dimensionless |
