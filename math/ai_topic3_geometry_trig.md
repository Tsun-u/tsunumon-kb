# IB Math AI — Topic 3: Geometry and Trigonometry

> SL: 18 hours | HL: 46 hours

## SL Content

### SL 3.1 3D Geometry
- Distance and midpoint between two points in three-dimensional space
- Volume and surface area of 3D solids: cuboid, prism, cylinder, pyramid, cone, sphere, hemisphere, and composite shapes
- Angle between a line and a plane; angle between two intersecting lines

### SL 3.2 Triangle Trigonometry
- Sine, cosine, and tangent ratios in right-angled triangles
- **Sine rule**: $\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C}$
- **Cosine rule**: $c^2 = a^2 + b^2 - 2ab\cos C$
- Triangle area: $\frac{1}{2}ab\sin C$

### SL 3.3 Applied Trigonometry
- Angles of elevation and depression in practical settings
- **Bearings**: three-digit values measured clockwise from north
- Drawing and labelling diagrams from verbal descriptions

### SL 3.4 Arcs and Sectors
- Arc length and sector area using degree measure (at SL)

### SL 3.5 Perpendicular Bisectors
- Finding equations of perpendicular bisectors given two points or a line segment

### SL 3.6 Voronoi Diagrams
- Key terminology: sites, vertices, edges, cells
- Adding a new site to an existing Voronoi diagram (incremental method)
- **Nearest neighbour interpolation** using Voronoi regions
- Applications: the largest empty circle problem (toxic waste dump context)

## HL Extension

### AHL 3.7 Radian Measure
- Definition of a radian; converting between degrees and radians
- Arc length and sector area using radian measure

### AHL 3.8 Unit Circle Trigonometry
- Defining $\cos\theta$, $\sin\theta$, $\tan\theta = \frac{\sin\theta}{\cos\theta}$ from the unit circle
- Exact values at $0, \frac{\pi}{6}, \frac{\pi}{4}, \frac{\pi}{3}, \frac{\pi}{2}$ and their multiples
- Pythagorean identity: $\cos^2\theta + \sin^2\theta = 1$
- The ambiguous case in the sine rule

### AHL 3.9 Matrix Transformations
- Encoding geometric transformations (reflections, stretches, enlargements, translations, rotations) as $2 \times 2$ matrices
- Composing transformations; the determinant as an area scale factor
- Application to fractal geometry

### AHL 3.10 Vectors: Concepts
- Distinguishing vectors from scalars; representations using column vectors and $\mathbf{i}, \mathbf{j}, \mathbf{k}$ notation
- Magnitude, unit vectors, position vectors; addition and scalar multiplication

### AHL 3.11 Vector Equation of a Line
- $\mathbf{r} = \mathbf{a} + \lambda\mathbf{b}$ in two and three dimensions

### AHL 3.12 Vector Kinematics
- Modelling linear motion at constant velocity: $\mathbf{r} = \mathbf{r_0} + t\mathbf{v}$
- Speed as the magnitude of the velocity vector: $|\mathbf{v}|$

### AHL 3.13 Scalar and Vector Products
- **Dot product**: $\mathbf{a} \cdot \mathbf{b} = |\mathbf{a}||\mathbf{b}|\cos\theta$; finding the angle between two vectors
- **Cross product magnitude**: $|\mathbf{a} \times \mathbf{b}| = |\mathbf{a}||\mathbf{b}|\sin\theta$; geometric interpretation as area

### AHL 3.14 Graph Theory: Foundations
- Basic vocabulary: vertices, edges, degree; adjacent vertices and edges
- Graph types: simple, complete, connected, directed, weighted; subgraphs, trees

### AHL 3.15 Adjacency Matrices
- Representing graphs as adjacency matrices
- Counting walks of length $k$ between vertices using the matrix power $A^k$
- Weighted adjacency tables

### AHL 3.16 Graph Algorithms
- Distinctions among walks, trails, paths, circuits, and cycles
- **Eulerian trails and circuits**; **Hamiltonian paths and cycles**
- **Minimum spanning tree**: Kruskal's algorithm and Prim's algorithm
- **Chinese postman problem** (route inspection)
- **Travelling salesman problem**: nearest neighbour heuristic (upper bound), deleted vertex algorithm (lower bound)

## Key Equations

| Equation | Description |
|----------|-------------|
| $\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C}$ | Sine rule |
| $c^2 = a^2 + b^2 - 2ab\cos C$ | Cosine rule |
| $\text{Area} = \frac{1}{2}ab\sin C$ | Triangle area |
| $\mathbf{r} = \mathbf{a} + \lambda\mathbf{b}$ | Vector line equation (HL) |
| $\mathbf{a}\cdot\mathbf{b} = \|\mathbf{a}\|\|\mathbf{b}\|\cos\theta$ | Dot product (HL) |

## Common Misconceptions

1. **Bearing direction** — Bearings are measured clockwise from due north and written as three digits.
2. **Cosine rule scope** — It works for any triangle, not only right triangles; setting $C = 90°$ reduces it to the Pythagorean theorem.
3. **Eulerian circuits** — A connected graph has an Eulerian circuit only when every vertex has even degree.
4. **Nearest neighbour and the TSP** — The nearest neighbour heuristic gives an upper bound on the optimal route, not the guaranteed shortest path.
5. **Voronoi edges** — Edges are perpendicular bisectors between pairs of sites, not segments connecting sites directly.

## Comparison with Other Courses

- Voronoi diagrams and graph theory are exclusive to AI — they appear in neither AA, AP Calculus, nor AP Statistics
- Vectors are covered in both AI HL and AA HL; AA HL extends to intersections of lines and planes, while AI HL applies vectors primarily to kinematics
- AP Calculus BC handles vector-valued functions through calculus (derivatives and integrals), which AI does not cover
