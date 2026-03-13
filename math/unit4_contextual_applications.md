# Unit 4: Contextual Applications of Differentiation
> AB Exam Weight: 10–15% | BC Exam Weight: 6–9% | ~10–11 Class Periods

## Big Ideas: CHA, FUN, LIM

---

## Topics

### 4.1 Interpreting the Meaning of the Derivative in Context
- **Learning Objective (CHA-3.A):** Interpret the meaning of a derivative in context.
- **Essential Knowledge:**
  - The derivative $f'(a)$ represents the instantaneous rate of change of $f$ at $x = a$.
  - Units of $f'(x)$: (units of $f$) / (units of $x$).
  - Example: If $C(t)$ is cost in dollars and $t$ is items produced, then $C'(50) = 3.2$ means "when 50 items have been produced, the cost is increasing at a rate of $3.20 per item."
  - Students must include units, direction (increasing/decreasing), and context in interpretations.

### 4.2 Straight-Line Motion: Connecting Position, Velocity, and Acceleration
- **Learning Objective (CHA-3.B):** Calculate rates of change in motion problems.
- **Essential Knowledge:**
  - Position: $s(t)$ or $x(t)$
  - Velocity: $v(t) = s'(t)$ — rate of change of position
  - Acceleration: $a(t) = v'(t) = s''(t)$ — rate of change of velocity
  - Speed: $|v(t)|$ (magnitude of velocity)
  - A particle is:
    - Moving right/up when $v(t) > 0$
    - Moving left/down when $v(t) < 0$
    - At rest when $v(t) = 0$
  - Speeding up when $v(t)$ and $a(t)$ have the same sign.
  - Slowing down when $v(t)$ and $a(t)$ have opposite signs.
  - Common misconception: Negative velocity means slowing down. (Correct: negative velocity means moving in the negative direction.)

### 4.3 Rates of Change in Applied Contexts Other Than Motion
- **Learning Objective (CHA-3.C):** Interpret rates of change in various applied contexts.
- **Essential Knowledge:**
  - The derivative applies to any quantity that changes: population growth, temperature change, volume, cost, etc.
  - Marginal cost: $C'(x)$ approximates the cost of producing one additional unit.
  - Always include units and context when interpreting derivatives.

### 4.4 Introduction to Related Rates
- **Learning Objective (CHA-3.D):** Calculate related rates.
- **Essential Knowledge:**
  - Related rates problems involve two or more quantities that change with respect to time.
  - Strategy:
    1. Identify all variables and given rates.
    2. Write an equation relating the variables.
    3. Differentiate both sides with respect to $t$ (implicit differentiation).
    4. Substitute known values and solve for the unknown rate.
  - Common geometric relationships used:
    - Pythagorean theorem: $a^2 + b^2 = c^2$
    - Area of circle: $A = \pi r^2$
    - Volume of sphere: $V = \frac{4}{3}\pi r^3$
    - Volume of cone: $V = \frac{1}{3}\pi r^2 h$
    - Similar triangles

### 4.5 Solving Related Rates Problems
- **Learning Objective (CHA-3.D):** Solve related rates problems.
- **Essential Knowledge:**
  - After differentiating, substitute values that are true at the specific instant in question.
  - Do NOT substitute specific values before differentiating.
  - Common misconception: Substituting constant values before taking the derivative.
  - Example: A ladder sliding down a wall — if $x^2 + y^2 = L^2$, then $2x\frac{dx}{dt} + 2y\frac{dy}{dt} = 0$.

### 4.6 Approximating Values of a Function Using Local Linearity and Linearization
- **Learning Objective (CHA-3.E):** Approximate function values using linearization.
- **Essential Knowledge:**
  - **Linear approximation (tangent line approximation):**
    $$f(x) \approx f(a) + f'(a)(x - a) \text{ for } x \text{ near } a$$
  - This is the tangent line at $x = a$ used as an approximation.
  - The approximation is better when $x$ is closer to $a$.
  - If $f''(a) > 0$ (concave up), the linear approximation is an underestimate.
  - If $f''(a) < 0$ (concave down), the linear approximation is an overestimate.

### 4.7 Using L'Hopital's Rule for Determining Limits of Indeterminate Forms
- **Learning Objective (LIM-4.A):** Apply L'Hopital's Rule.
- **Essential Knowledge:**
  - **L'Hopital's Rule:** If $\lim_{x \to c} \frac{f(x)}{g(x)}$ yields $\frac{0}{0}$ or $\frac{\pm\infty}{\pm\infty}$, then:
    $$\lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}$$
    provided the latter limit exists (or is $\pm\infty$).
  - Can be applied repeatedly if the result is still indeterminate.
  - Must verify the indeterminate form before applying.
  - Common misconception: Applying L'Hopital's Rule when the form is not indeterminate.
  - Common misconception: Using the quotient rule instead of differentiating numerator and denominator separately.

---

## Key Formulas Summary

| Concept | Formula |
|---------|---------|
| Velocity | $v(t) = s'(t)$ |
| Acceleration | $a(t) = v'(t) = s''(t)$ |
| Speed | $\|v(t)\|$ |
| Linear approximation | $f(x) \approx f(a) + f'(a)(x - a)$ |
| L'Hopital's Rule | $\lim \frac{f(x)}{g(x)} = \lim \frac{f'(x)}{g'(x)}$ (for $\frac{0}{0}$ or $\frac{\infty}{\infty}$) |

## Common Misconceptions
- Confusing velocity and speed (velocity can be negative; speed cannot).
- In related rates, substituting values before differentiating.
- Thinking negative acceleration always means slowing down (depends on sign of velocity).
- Applying L'Hopital's Rule to non-indeterminate forms.
- Forgetting to verify the indeterminate form at each step of repeated L'Hopital application.
- In linearization, not recognizing whether the approximation is an over- or underestimate based on concavity.
