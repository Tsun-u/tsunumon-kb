# IB Math AI — Topic 1: Number and Algebra

> SL: 16 hours | HL: 29 hours

## SL Content

### SL 1.1 Scientific Notation
- Working with numbers expressed as $a \times 10^k$, where $1 \leq a < 10$ and $k \in \mathbb{Z}$
- Technology outputs values in E notation; converting these back to standard scientific form is an expected skill

### SL 1.2 Arithmetic Sequences and Series
- Common difference $d$; general term $u_n = u_1 + (n-1)d$
- Sum formula: $S_n = \frac{n}{2}(2u_1 + (n-1)d) = \frac{n}{2}(u_1 + u_n)$
- Applied contexts: simple interest, straight-line depreciation, salary structures

### SL 1.3 Geometric Sequences and Series
- Common ratio $r$; general term $u_n = u_1 \cdot r^{n-1}$
- Sum formula: $S_n = \frac{u_1(r^n - 1)}{r - 1}$, $r \neq 1$
- Applied contexts: population growth, repeated percentage change, compound phenomena

### SL 1.4 Financial Applications of Geometric Sequences
- **Compound interest**: $FV = PV\left(1 + \frac{r}{100k}\right)^{kn}$ (compounding $k$ times per year)
- **Annual depreciation** using a reducing balance approach
- Financial calculations are performed with a GDC TVM solver or financial app

### SL 1.5 Exponents and Introduction to Logarithms
- Laws of exponents with integer exponents
- Logarithms base 10 and base $e$: the equivalence $\log_a b = c \iff a^c = b$
- Using logarithms to solve exponential equations, numerically and with technology

### SL 1.6 Approximation and Error
- Rounding to decimal places and significant figures
- Upper and lower bounds arising from rounded measurements
- **Percentage error**: $\varepsilon = \left| \frac{v_A - v_E}{v_E} \right| \times 100\%$ ($v_A$ = approximate, $v_E$ = exact value)
- Estimation as a way to verify the reasonableness of results

### SL 1.7 Amortization and Annuities
- Loan amortization and annuity calculations performed using technology (TVM solver)
- Interpreting repayment schedules: distinguishing interest payments from principal reduction

### SL 1.8 Solving Equations with Technology
- Systems of linear equations in up to 3 variables, solved with technology
- Polynomial equations solved using a GDC

## HL Extension

### AHL 1.9 Laws of Logarithms
- $\log_a(xy) = \log_a x + \log_a y$; $\log_a(x/y) = \log_a x - \log_a y$; $\log_a x^n = n \log_a x$

### AHL 1.10 Rational Exponents
- Simplifying expressions involving rational (fractional) exponents, both numerically and algebraically

### AHL 1.11 Infinite Geometric Series
- Convergent infinite geometric series: $S_\infty = \frac{u_1}{1 - r}$ for $|r| < 1$; connection to limits and fractal geometry

### AHL 1.12 Complex Numbers: Cartesian Form
- $i^2 = -1$; $z = a + bi$; real part, imaginary part, complex conjugate
- Applications in physical contexts (e.g., electrical circuits); solving polynomial equations with technology

### AHL 1.13 Complex Numbers: Polar and Euler Form
- Modulus-argument form: $z = r(\cos\theta + i\sin\theta) = r\,\text{cis}\,\theta$
- Euler/exponential form: $z = re^{i\theta}$
- Converting between forms; products and quotients in polar form
- Applications in sinusoidal modelling and phase analysis

### AHL 1.14 Matrices
- Matrix fundamentals: element, row, column, order
- Operations: addition, scalar multiplication, matrix multiplication
- Determinants and inverses of $2\times2$ matrices by hand; larger matrices with technology
- Using matrices to solve systems of linear equations

### AHL 1.15 Eigenvalues and Eigenvectors
- Characteristic polynomial of a $2\times2$ matrix
- Finding eigenvalues and eigenvectors; diagonalization $M = PDP^{-1}$
- Matrix powers: $M^n = PD^nP^{-1}$
- Applied uses: coupled differential equations, Markov chains, transition matrices

## Key Equations

| Equation | Description |
|----------|-------------|
| $u_n = u_1 + (n-1)d$ | Arithmetic sequence |
| $u_n = u_1 r^{n-1}$ | Geometric sequence |
| $FV = PV(1 + \frac{r}{100k})^{kn}$ | Compound interest |
| $\varepsilon = \|\frac{v_A - v_E}{v_E}\| \times 100\%$ | Percentage error |
| $S_\infty = u_1/(1-r)$ | Infinite geometric series (HL, $\|r\| < 1$) |
| $z = re^{i\theta}$ | Complex number, Euler form (HL) |
| $\det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad - bc$ | $2\times2$ determinant (HL) |

## Common Misconceptions

1. **Percentage error denominator** — The denominator is the exact value $v_E$, not the approximate value.
2. **Compound interest periodicity** — The factor $k$ handles monthly ($k=12$), quarterly ($k=4$), and other compounding frequencies, not just annual.
3. **Matrix multiplication order** — In general $AB \neq BA$; order cannot be reversed freely.
4. **Geometric series convergence** — $S_\infty$ exists only when $|r| < 1$; series with $|r| \geq 1$ diverge.

## Comparison with Other Courses

- Financial mathematics (amortization, annuities, TVM solver) is a defining feature of AI — absent from AA and AP Calculus
- Matrices and eigenvalues (AHL) have no parallel in current AA or AP Calculus syllabi
- Complex numbers appear in both AI HL and AA HL, but AA HL treats them more formally (De Moivre's theorem, roots of unity, proof-based arguments)
