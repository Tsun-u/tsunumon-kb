# Unit 4: Contextual Applications of Differentiation
> AB Exam Weight: 10–15% | BC Exam Weight: 6–9% | ~10–11 Class Periods

---

## Topics

### 4.1 Interpreting the Meaning of the Derivative in Context
- The derivative $f'(a)$ is the instantaneous rate at which $f$ is changing when the input is $a$.
- Units of $f'(x)$: (units of output) / (units of input) — always state units when interpreting.
- Example: If $C(t)$ is cost in dollars and $t$ is items produced, then $C'(50) = 3.2$ means the cost is rising at \$3.20 per additional item at the moment when 50 items have been made.
- A complete interpretation includes units, the direction of change (increasing or decreasing), and the real-world meaning.

### 4.2 Straight-Line Motion: Connecting Position, Velocity, and Acceleration
- Position: $s(t)$ or $x(t)$ describes where an object is at time $t$
- Velocity: $v(t) = s'(t)$ — how quickly and in which direction the position is changing
- Acceleration: $a(t) = v'(t) = s''(t)$ — how quickly velocity is changing
- Speed: $|v(t)|$ — magnitude of velocity, always non-negative
- A particle moves in the positive direction when $v(t) > 0$, negative direction when $v(t) < 0$, and is momentarily at rest when $v(t) = 0$.
- Speeding up happens when velocity and acceleration share the same sign; slowing down happens when they have opposite signs.

### 4.3 Rates of Change in Applied Contexts Other Than Motion
- The derivative describes the rate of change of any quantity — population, temperature, volume, revenue, and so on.
- Marginal cost $C'(x)$ tells you approximately how much it costs to produce one more unit at output level $x$.
- In every application context, units and real-world meaning must accompany the numerical answer.

### 4.4 Introduction to Related Rates
- Related rates problems involve two or more quantities that all change as time passes, with their rates connected by an underlying relationship.
- General approach:
  1. Name all variables and record any given rates.
  2. Write an equation relating the variables.
  3. Differentiate both sides with respect to $t$ using implicit differentiation.
  4. Plug in the known values at the instant of interest and solve for the unknown rate.
- Useful geometric relationships:
  - Pythagorean theorem: $a^2 + b^2 = c^2$
  - Area of circle: $A = \pi r^2$
  - Volume of sphere: $V = \frac{4}{3}\pi r^3$
  - Volume of cone: $V = \frac{1}{3}\pi r^2 h$
  - Similar triangles

### 4.5 Solving Related Rates Problems
- Only substitute specific numerical values after differentiating — plugging in constants before differentiating turns variables into numbers too early and produces wrong results.
- Example: A ladder sliding down a wall — if $x^2 + y^2 = L^2$, differentiating gives $2x\frac{dx}{dt} + 2y\frac{dy}{dt} = 0$, then substitute the values at the specific moment.

### 4.6 Approximating Values of a Function Using Local Linearity and Linearization
- Near a point $a$ where $f$ is differentiable, the tangent line is a reliable stand-in for the function:
  $$f(x) \approx f(a) + f'(a)(x - a) \text{ for } x \text{ near } a$$
- The closer $x$ is to $a$, the better the approximation.
- The direction of the error depends on concavity:
  - $f''(a) > 0$ (concave up): the tangent line lies below the curve, so linearization underestimates.
  - $f''(a) < 0$ (concave down): the tangent line lies above the curve, so linearization overestimates.

### 4.7 Using L'Hopital's Rule for Determining Limits of Indeterminate Forms
- **L'Hopital's Rule:** When $\lim_{x \to c} \frac{f(x)}{g(x)}$ gives the indeterminate form $\frac{0}{0}$ or $\frac{\pm\infty}{\pm\infty}$:
  $$\lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}$$
  provided this new limit exists (or is $\pm\infty$).
- The rule can be applied more than once if the result is still indeterminate after the first application.
- Always confirm the indeterminate form before applying the rule — it's not valid for determinate forms.
- The numerator and denominator are differentiated separately, not as a quotient via the quotient rule.

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
