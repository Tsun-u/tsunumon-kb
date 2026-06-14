# Unit 5: Analytical Applications of Differentiation
> AB Exam Weight: 15–18% | BC Exam Weight: 8–11% | ~15–16 Class Periods

---

## Topics

### 5.1 Using the Mean Value Theorem
- **Mean Value Theorem (MVT):** If $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then at least one $c$ in $(a, b)$ satisfies:
  $$f'(c) = \frac{f(b) - f(a)}{b - a}$$
- Geometrically, this says there is always a point on the curve where the tangent is parallel to the secant line connecting the two endpoints.
- **Rolle's Theorem** is the special case where $f(a) = f(b)$: at some point in between, the derivative must be zero.
- Both conditions — continuity on the closed interval and differentiability on the open interval — must be confirmed before applying the theorem.

### 5.2 Extreme Value Theorem, Global Versus Local Extrema, and Critical Points
- **Extreme Value Theorem (EVT):** A function that is continuous on a closed interval $[a, b]$ is guaranteed to achieve both a global maximum and a global minimum somewhere on that interval.
- **Critical point:** $x = c$ is a critical point when $f'(c) = 0$ or $f'(c)$ does not exist (with $c$ in the domain of $f$).
- Local extrema can only occur at critical points, but not every critical point is a local extremum.

### 5.3 Determining Intervals on Which a Function Is Increasing or Decreasing
- $f$ is increasing on any interval where $f'(x) > 0$.
- $f$ is decreasing on any interval where $f'(x) < 0$.
- The process: find critical points, then test the sign of $f'$ in each resulting interval.
- A point where $f'(c) = 0$ doesn't automatically mean the function stops increasing or decreasing — the sign of $f'$ on either side is what matters.

### 5.4 Using the First Derivative Test to Determine Relative (Local) Extrema
- **First Derivative Test:** At a critical point $c$, examine how the sign of $f'$ changes:
  - $f'$ changes from positive to negative: local maximum at $c$.
  - $f'$ changes from negative to positive: local minimum at $c$.
  - $f'$ does not change sign: no local extremum at $c$.

### 5.5 Using the Candidates Test to Determine Absolute (Global) Extrema
- **Candidates Test (Closed Interval Method):** To find absolute extrema on $[a, b]$:
  1. Locate all critical points of $f$ inside $(a, b)$.
  2. Evaluate $f$ at each critical point and at both endpoints $a$ and $b$.
  3. The largest output is the absolute maximum; the smallest is the absolute minimum.
- This method works because the Extreme Value Theorem guarantees the extrema are attained somewhere.

### 5.6 Determining Concavity of Functions over Their Domains
- $f$ is concave up on any interval where $f''(x) > 0$ — the graph curves like a bowl holding water.
- $f$ is concave down on any interval where $f''(x) < 0$ — the graph curves like an upside-down bowl.
- **Inflection point:** A point where concavity changes, and the function is defined there.
- At an inflection point, $f''(x) = 0$ or $f''(x)$ is undefined, but a sign change in $f''$ must also occur.

### 5.7 Using the Second Derivative Test to Determine Extrema
- **Second Derivative Test:** When $f'(c) = 0$, check $f''(c)$:
  - $f''(c) > 0$: the graph is concave up at $c$, so $c$ is a local minimum.
  - $f''(c) < 0$: the graph is concave down at $c$, so $c$ is a local maximum.
  - $f''(c) = 0$: the test gives no information; fall back to the First Derivative Test.

### 5.8 Sketching Graphs of Functions and Their Derivatives
- The derivative graph encodes all the key features of the original function:
  - Where $f' > 0$: $f$ is increasing.
  - Where $f' < 0$: $f$ is decreasing.
  - Where $f' = 0$ and changes sign: $f$ has a local extremum.
  - Where $f'' > 0$: $f$ is concave up (equivalently, $f'$ is increasing).
  - Where $f'' < 0$: $f$ is concave down ($f'$ is decreasing).
  - Where $f''$ changes sign: $f$ has an inflection point.

### 5.9 Connecting a Function, Its First Derivative, and Its Second Derivative
- Given $f$, $f'$, or $f''$ in any form — equation, graph, or table — you should be able to read off key features of the others.
- The $x$-intercepts of $f'$ identify critical points of $f$.
- The $x$-intercepts of $f''$ are candidates for inflection points of $f$ (a sign change is still required).

### 5.10 Introduction to Optimization Problems
- Optimization means finding where some quantity reaches its largest or smallest value under given constraints.
- Getting set up correctly is half the work:
  1. Identify clearly which quantity is being optimized.
  2. Express that quantity as a function of a single variable, using the constraint to eliminate extras.
  3. Determine the realistic domain of the function.

### 5.11 Solving Optimization Problems
- Once the objective function is set up, find its critical points and evaluate at critical points and any relevant endpoints.
- Always justify that the answer found is actually the desired maximum or minimum — use the First Derivative Test, Second Derivative Test, or endpoint comparison.
- Typical problems: maximizing enclosed area, minimizing material cost, maximizing container volume.

### 5.12 Exploring Behaviors of Implicit Relations
- First and second derivative analysis extends naturally to curves defined implicitly.
- Finding tangent lines, determining where the curve rises or falls, and locating extrema all follow the same logic as for explicit functions.
- Computing the second derivative implicitly usually requires substituting the expression for $\frac{dy}{dx}$ partway through.

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
