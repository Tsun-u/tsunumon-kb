# Unit 5: Analytical Applications of Differentiation
> AB Exam Weight: 15–18% | BC Exam Weight: 8–11% | ~15–16 Class Periods

## Big Ideas: FUN, LIM

---

## Topics

### 5.1 Using the Mean Value Theorem
- **Learning Objective (FUN-1.B):** Apply the Mean Value Theorem.
- **Essential Knowledge:**
  - **Mean Value Theorem (MVT):** If $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists at least one $c$ in $(a, b)$ such that:
    $$f'(c) = \frac{f(b) - f(a)}{b - a}$$
  - Geometric meaning: There is a point where the tangent line is parallel to the secant line through $(a, f(a))$ and $(b, f(b))$.
  - **Rolle's Theorem** (special case): If $f(a) = f(b)$, then there exists $c$ in $(a, b)$ where $f'(c) = 0$.
  - Both conditions (continuity on closed interval, differentiability on open interval) must be verified.

### 5.2 Extreme Value Theorem, Global Versus Local Extrema, and Critical Points
- **Learning Objective (FUN-1.C):** Determine extreme values using the Extreme Value Theorem.
- **Essential Knowledge:**
  - **Extreme Value Theorem (EVT):** If $f$ is continuous on $[a, b]$, then $f$ attains both a global maximum and a global minimum on $[a, b]$.
  - **Critical point:** $x = c$ is a critical point of $f$ if $f'(c) = 0$ or $f'(c)$ does not exist (and $c$ is in the domain of $f$).
  - Local (relative) extrema can only occur at critical points.
  - Not every critical point is a local extremum.

### 5.3 Determining Intervals on Which a Function Is Increasing or Decreasing
- **Learning Objective (FUN-4.A):** Determine intervals of increase/decrease.
- **Essential Knowledge:**
  - $f$ is increasing on an interval where $f'(x) > 0$.
  - $f$ is decreasing on an interval where $f'(x) < 0$.
  - Find critical points, test sign of $f'$ in each interval.
  - Common misconception: $f'(c) = 0$ means $f$ is neither increasing nor decreasing at $c$. (Correct: $f$ can still be increasing or decreasing at a point where $f' = 0$.)

### 5.4 Using the First Derivative Test to Determine Relative (Local) Extrema
- **Learning Objective (FUN-4.A):** Use the First Derivative Test.
- **Essential Knowledge:**
  - **First Derivative Test:** At a critical point $c$:
    - If $f'$ changes from positive to negative at $c$: local maximum.
    - If $f'$ changes from negative to positive at $c$: local minimum.
    - If $f'$ does not change sign at $c$: no local extremum.

### 5.5 Using the Candidates Test to Determine Absolute (Global) Extrema
- **Learning Objective (FUN-1.C):** Find absolute extrema on a closed interval.
- **Essential Knowledge:**
  - **Candidates Test (Closed Interval Method):**
    1. Find all critical points of $f$ in $(a, b)$.
    2. Evaluate $f$ at each critical point and at the endpoints $a$ and $b$.
    3. The largest value is the absolute maximum; the smallest is the absolute minimum.
  - This method works because of the Extreme Value Theorem.

### 5.6 Determining Concavity of Functions over Their Domains
- **Learning Objective (FUN-4.A):** Determine concavity.
- **Essential Knowledge:**
  - $f$ is concave up on an interval where $f''(x) > 0$ (the graph "holds water").
  - $f$ is concave down on an interval where $f''(x) < 0$ (the graph "spills water").
  - **Inflection point:** A point where concavity changes (and the function is defined).
  - At an inflection point, $f''(x) = 0$ or $f''(x)$ does not exist, AND concavity changes.

### 5.7 Using the Second Derivative Test to Determine Extrema
- **Learning Objective (FUN-4.A):** Use the Second Derivative Test.
- **Essential Knowledge:**
  - **Second Derivative Test:** At a critical point $c$ where $f'(c) = 0$:
    - If $f''(c) > 0$: local minimum (concave up).
    - If $f''(c) < 0$: local maximum (concave down).
    - If $f''(c) = 0$: test is inconclusive; use First Derivative Test.

### 5.8 Sketching Graphs of Functions and Their Derivatives
- **Learning Objective (FUN-4.A):** Sketch and analyze graphs of $f$, $f'$, and $f''$.
- **Essential Knowledge:**
  - Connections between $f$, $f'$, and $f''$:
    - Where $f' > 0$, $f$ is increasing.
    - Where $f' < 0$, $f$ is decreasing.
    - Where $f' = 0$ (and changes sign), $f$ has a local extremum.
    - Where $f'' > 0$, $f$ is concave up ($f'$ is increasing).
    - Where $f'' < 0$, $f$ is concave down ($f'$ is decreasing).
    - Where $f'' = 0$ (and changes sign), $f$ has an inflection point.

### 5.9 Connecting a Function, Its First Derivative, and Its Second Derivative
- **Learning Objective (FUN-4.A):** Connect information from $f$, $f'$, and $f''$.
- **Essential Knowledge:**
  - Given any one of $f$, $f'$, or $f''$ (as a graph, equation, or table), students should be able to determine key features of the others.
  - $x$-intercepts of $f'$ correspond to critical points of $f$.
  - $x$-intercepts of $f''$ are candidates for inflection points of $f$.

### 5.10 Introduction to Optimization Problems
- **Learning Objective (FUN-4.B):** Set up optimization problems.
- **Essential Knowledge:**
  - Optimization involves finding the maximum or minimum value of a function subject to constraints.
  - Strategy:
    1. Identify the quantity to optimize.
    2. Write it as a function of one variable (using the constraint to eliminate variables).
    3. Determine the domain (feasible values).

### 5.11 Solving Optimization Problems
- **Learning Objective (FUN-4.C):** Solve optimization problems.
- **Essential Knowledge:**
  - Find critical points, evaluate at critical points and endpoints (if closed interval).
  - Justify that the answer is indeed a maximum or minimum (using First or Second Derivative Test, or by evaluating at endpoints).
  - Common problem types: maximizing area, minimizing material/cost, maximizing volume.

### 5.12 Exploring Behaviors of Implicit Relations
- **Learning Objective (FUN-4.D):** Analyze implicit relations using derivatives.
- **Essential Knowledge:**
  - Apply first and second derivative analysis to implicitly defined curves.
  - Find tangent lines, determine increasing/decreasing behavior, and find extrema for implicit relations.
  - The second derivative of an implicit relation may require substituting the first derivative expression.

---

## Key Formulas Summary

| Theorem/Concept | Statement |
|----------------|-----------|
| Mean Value Theorem | $f'(c) = \frac{f(b)-f(a)}{b-a}$ for some $c \in (a,b)$ |
| Rolle's Theorem | If $f(a)=f(b)$, then $f'(c)=0$ for some $c \in (a,b)$ |
| Extreme Value Theorem | Continuous $f$ on $[a,b]$ attains max and min |
| First Derivative Test | Sign change of $f'$ determines local extrema |
| Second Derivative Test | $f'(c)=0$ and $f''(c)>0 \Rightarrow$ local min; $f''(c)<0 \Rightarrow$ local max |

## Common Misconceptions
- Confusing local and global extrema.
- Assuming every critical point is an extremum.
- Assuming $f''(c) = 0$ means inflection point (concavity must change).
- Forgetting to check endpoints when finding absolute extrema on a closed interval.
- In optimization, not verifying the domain of the function or that the critical point gives the desired extremum.
- Applying the Mean Value Theorem without verifying continuity and differentiability conditions.
