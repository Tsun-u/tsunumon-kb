# Topic 1: Number and Algebra

> SL: 19 hours | HL: 39 hours

## SL Content

### 1.1 Sequences and Series
- **Arithmetic sequences**: common difference $d$; $u_n = u_1 + (n-1)d$
- **Arithmetic series**: $S_n = \frac{n}{2}(2u_1 + (n-1)d) = \frac{n}{2}(u_1 + u_n)$
- **Geometric sequences**: common ratio $r$; $u_n = u_1 \cdot r^{n-1}$
- **Geometric series**: $S_n = \frac{u_1(r^n - 1)}{r - 1} = \frac{u_1(1 - r^n)}{1 - r}$
- **Infinite geometric series** (convergent when $|r| < 1$): $S_\infty = \frac{u_1}{1 - r}$
- Sigma notation: $\sum_{r=1}^{n} u_r$

### 1.2 Exponents and Logarithms
- Laws of exponents: $a^m \cdot a^n = a^{m+n}$, $(a^m)^n = a^{mn}$, $a^{-n} = \frac{1}{a^n}$, $a^{1/n} = \sqrt[n]{a}$
- **Logarithms**: $\log_a b = c \iff a^c = b$
- Laws of logarithms:
  - $\log(xy) = \log x + \log y$
  - $\log(x/y) = \log x - \log y$
  - $\log(x^n) = n\log x$
  - Change of base: $\log_a b = \frac{\log_c b}{\log_c a}$
- Natural logarithm: $\ln x = \log_e x$
- Solving exponential equations using logarithms

### 1.3 Binomial Theorem
- $(a + b)^n = \sum_{r=0}^{n} \binom{n}{r} a^{n-r} b^r$
- Binomial coefficient: $\binom{n}{r} = \frac{n!}{r!(n-r)!}$
- Pascal's triangle
- Finding specific terms in a binomial expansion

## HL Extension

### 1.4 Proof by Induction
- Steps: base case → inductive hypothesis → inductive step → conclusion
- Applications: sum formulas, divisibility, inequalities, matrix powers

### 1.5 Complex Numbers
- Imaginary unit: $i = \sqrt{-1}$, $i^2 = -1$
- Complex number: $z = a + bi$ (Cartesian form)
- **Polar/modulus-argument form**: $z = r(\cos\theta + i\sin\theta) = re^{i\theta}$
  - Modulus: $|z| = r = \sqrt{a^2 + b^2}$
  - Argument: $\arg(z) = \theta = \arctan(b/a)$
- Operations: addition, multiplication, conjugate ($\bar{z} = a - bi$)
- **De Moivre's theorem**: $(r e^{i\theta})^n = r^n e^{in\theta}$
- Roots of unity and solving polynomial equations with complex roots
- Complex conjugate root theorem: if $z$ is a root of a real polynomial, so is $\bar{z}$

### 1.6 Counting Principles and Proof
- Permutations: $P(n,r) = \frac{n!}{(n-r)!}$
- Combinations: $C(n,r) = \binom{n}{r}$
- Proof by contradiction
- Proof by counterexample

## Key Equations

| Equation | Description |
|----------|-------------|
| $u_n = u_1 + (n-1)d$ | Arithmetic sequence |
| $u_n = u_1 r^{n-1}$ | Geometric sequence |
| $S_\infty = u_1/(1-r)$ | Infinite geometric series ($\|r\| < 1$) |
| $z = re^{i\theta}$ | Complex number (polar/Euler form, HL) |
| $(re^{i\theta})^n = r^n e^{in\theta}$ | De Moivre's theorem (HL) |

## Common Misconceptions

1. **"An infinite series always diverges"** -- Geometric series with $|r| < 1$ converge to a finite sum.
2. **"$\log(a + b) = \log a + \log b$"** -- This is incorrect; $\log(ab) = \log a + \log b$, not $\log(a+b)$.
3. **"$i$ is not a real number, so it doesn't matter"** -- Complex numbers are essential in engineering, physics, and solving polynomial equations.
4. **"Proof by induction only works for sums"** -- Induction can prove divisibility, inequalities, matrix results, and more.

## Comparison with AP Mathematics

- AP Pre-Calculus covers sequences, series, and logarithms similarly
- Complex numbers at IB HL level go beyond AP Pre-Calculus (De Moivre, roots of unity)
- Proof by induction is not required in AP Calculus but is central to IB HL
- AP Calculus BC covers series convergence in more depth (ratio test, Taylor series)
