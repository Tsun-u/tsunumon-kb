# Topic 1: Number and Algebra

> SL: 19 hours | HL: 39 hours

## SL Content

### 1.1 Sequences and Series
- **Arithmetic sequences**: consecutive terms differ by a fixed amount called the common difference $d$; the $n$-th term is $u_n = u_1 + (n-1)d$
- **Arithmetic series**: the total when you add up $n$ terms: $S_n = \frac{n}{2}(2u_1 + (n-1)d) = \frac{n}{2}(u_1 + u_n)$
- **Geometric sequences**: each term is obtained by multiplying the previous one by a constant ratio $r$; the $n$-th term is $u_n = u_1 \cdot r^{n-1}$
- **Geometric series**: sum of $n$ terms: $S_n = \frac{u_1(r^n - 1)}{r - 1} = \frac{u_1(1 - r^n)}{1 - r}$
- **Infinite geometric series** (convergent when $|r| < 1$): as more and more terms are added, the total approaches $S_\infty = \frac{u_1}{1 - r}$
- Sigma notation provides a compact way to write sums: $\sum_{r=1}^{n} u_r$

### 1.2 Exponents and Logarithms
- Laws of exponents: $a^m \cdot a^n = a^{m+n}$, $(a^m)^n = a^{mn}$, $a^{-n} = \frac{1}{a^n}$, $a^{1/n} = \sqrt[n]{a}$
- **Logarithms** answer "what power gives this result?": $\log_a b = c \iff a^c = b$
- Laws of logarithms let you expand or combine log expressions:
  - $\log(xy) = \log x + \log y$
  - $\log(x/y) = \log x - \log y$
  - $\log(x^n) = n\log x$
  - Change of base: $\log_a b = \frac{\log_c b}{\log_c a}$
- Natural logarithm uses base $e$: $\ln x = \log_e x$
- Exponential equations can be solved by applying a logarithm to both sides

### 1.3 Binomial Theorem
- $(a + b)^n = \sum_{r=0}^{n} \binom{n}{r} a^{n-r} b^r$
- Binomial coefficient counts the number of ways to choose $r$ items from $n$: $\binom{n}{r} = \frac{n!}{r!(n-r)!}$
- Pascal's triangle gives a visual method to read off binomial coefficients row by row
- Any specific term in the expansion can be identified by its position using the general term formula

## HL Extension

### 1.4 Proof by Induction
- A four-step logical framework: establish the base case, assume the statement holds for $n = k$, prove it must then hold for $n = k+1$, and write a formal conclusion
- Applicable beyond sum formulas: divisibility results, inequalities, and statements about matrix powers are all fair game

### 1.5 Complex Numbers
- Imaginary unit: $i = \sqrt{-1}$, $i^2 = -1$
- Complex number in Cartesian form: $z = a + bi$, with real part $a$ and imaginary part $b$
- **Polar/modulus-argument form** expresses $z$ in terms of its distance from the origin and angle: $z = r(\cos\theta + i\sin\theta) = re^{i\theta}$
  - Modulus (distance from origin): $|z| = r = \sqrt{a^2 + b^2}$
  - Argument (angle from positive real axis): $\arg(z) = \theta = \arctan(b/a)$
- Arithmetic operations work component-wise; the conjugate flips the imaginary sign: $\bar{z} = a - bi$
- **De Moivre's theorem** makes repeated multiplication elegant: $(r e^{i\theta})^n = r^n e^{in\theta}$
- Roots of polynomials with real coefficients come in conjugate pairs; $n$-th roots of unity are equally spaced around the unit circle
- Complex conjugate root theorem: if $z$ is a root of a real polynomial, so is $\bar{z}$

### 1.6 Counting Principles and Proof
- Permutations count ordered arrangements: $P(n,r) = \frac{n!}{(n-r)!}$
- Combinations count unordered selections: $C(n,r) = \binom{n}{r}$
- Proof by contradiction assumes the negation is true and derives an impossibility
- Proof by counterexample disproves a general claim by exhibiting a single case where it fails

## Key Equations

| Equation | Description |
|----------|-------------|
| $u_n = u_1 + (n-1)d$ | Arithmetic sequence |
| $u_n = u_1 r^{n-1}$ | Geometric sequence |
| $S_\infty = u_1/(1-r)$ | Infinite geometric series ($\|r\| < 1$) |
| $z = re^{i\theta}$ | Complex number (polar/Euler form, HL) |
| $(re^{i\theta})^n = r^n e^{in\theta}$ | De Moivre's theorem (HL) |

## Common Misconceptions

1. **"An infinite series always diverges"** -- A geometric series with $|r| < 1$ actually converges to a well-defined finite value; the terms shrink fast enough that their total is bounded.
2. **"$\log(a + b) = \log a + \log b$"** -- This is a common mix-up; the product law says $\log(ab) = \log a + \log b$, not addition inside the argument.
3. **"$i$ is not a real number, so it doesn't really count"** -- Complex numbers are indispensable in electrical engineering, signal processing, quantum mechanics, and whenever a polynomial needs all its roots accounted for.
4. **"Proof by induction only works for sum formulas"** -- The technique is far more general; it applies to divisibility statements, inequalities, and properties of matrix powers, among other things.

## Comparison with AP Mathematics

- Sequences, series, and logarithm rules overlap broadly with AP Pre-Calculus content, so students switching between the two curricula will find much that is familiar
- IB HL goes further with complex numbers than AP Pre-Calculus does, adding De Moivre's theorem, roots of unity, and connections to polynomial theory
- Mathematical proof by induction plays a central role in IB HL but does not appear as a required topic in AP Calculus
- AP Calculus BC treats series convergence in greater detail, including the ratio test and Taylor/Maclaurin expansions with error analysis
