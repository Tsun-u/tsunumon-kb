# Unit 1: Primitive Types

**Exam Weight:** 2.5-5% | **Suggested Time:** ~8-10 class periods
**2025-26 Revision:** Merged into new Unit 1 "Using Objects and Methods"

## Topics

### Topic 1.1: Why Programming? Why Java?
- **Learning Objective (MOD-1.A):** Call `System` class methods to generate output to the console
- **Essential Knowledge:**
  - `System.out.print()` displays output without a newline
  - `System.out.println()` displays output followed by a newline
  - String literals are enclosed in double quotes `""`
  - `System.out.println()` with no arguments outputs a blank line

### Topic 1.2: Variables and Data Types
- **Learning Objective (VAR-1.A):** Create string literals
- **Learning Objective (VAR-1.B):** Identify the most appropriate data type category for a particular specification
- **Learning Objective (VAR-1.C):** Declare variables of the correct types to represent primitive data
- **Essential Knowledge:**
  - Three primitive types on the AP exam: `int`, `double`, `boolean`
  - `int` stores whole numbers (no decimals)
  - `double` stores floating-point numbers (with decimals)
  - `boolean` stores `true` or `false`
  - `String` is a reference type (not primitive), covered more in Unit 2
  - Variable names are case-sensitive and follow camelCase convention
  - Variables must be declared before use
  - `final` keyword declares a constant

### Topic 1.3: Expressions and Assignment Statements
- **Learning Objective (VAR-1.D):** Define variables with appropriate initial values
- **Learning Objective (VAR-1.E):** Evaluate arithmetic expressions in a program
- **Essential Knowledge:**
  - Assignment operator `=` assigns a value to a variable
  - Arithmetic operators: `+`, `-`, `*`, `/`, `%` (modulus)
  - Integer division truncates (rounds toward zero): `7 / 2` evaluates to `3`
  - Modulus `%` returns the remainder: `7 % 2` evaluates to `1`
  - Operator precedence: `*`, `/`, `%` before `+`, `-`
  - Parentheses override precedence
  - Expressions are evaluated left to right for equal precedence

### Topic 1.4: Compound Assignment Operators
- **Learning Objective (VAR-1.F):** Evaluate compound assignment expressions
- **Essential Knowledge:**
  - Compound operators: `+=`, `-=`, `*=`, `/=`, `%=`
  - Increment: `x++` or `++x` (adds 1)
  - Decrement: `x--` or `--x` (subtracts 1)
  - `x += 3` is equivalent to `x = x + 3`

### Topic 1.5: Casting and Ranges of Variables
- **Learning Objective (VAR-1.G):** Evaluate expressions that use casting
- **Essential Knowledge:**
  - Casting converts between types: `(int)`, `(double)`
  - `(int) 3.7` evaluates to `3` (truncation, NOT rounding)
  - `(double) 5` evaluates to `5.0`
  - Implicit widening: `int` to `double` happens automatically
  - Explicit narrowing: `double` to `int` requires cast
  - `int` range: -2,147,483,648 to 2,147,483,647 (Integer.MIN_VALUE to Integer.MAX_VALUE)
  - Integer overflow: exceeding range wraps around silently
  - Rounding trick: `(int)(x + 0.5)` rounds positive doubles to nearest int

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Variable | A named storage location in memory |
| Data type | Defines what kind of data a variable can hold |
| Primitive type | Basic built-in data types (`int`, `double`, `boolean`) |
| Literal | A fixed value written directly in code (e.g., `42`, `3.14`, `true`) |
| Expression | A combination of values, variables, and operators that evaluates to a value |
| Assignment | Storing a value in a variable using `=` |
| Casting | Explicitly converting a value from one type to another |
| Truncation | Removing the decimal portion (not rounding) |
| Overflow | When a value exceeds the range of its data type |

## Common Misconceptions

1. **Integer division returns a double** - No! `7 / 2` is `3`, not `3.5`. Both operands must be `int` for integer division to occur. If either is `double`, the result is `double`.
2. **Casting rounds the value** - No! `(int) 3.9` is `3`, not `4`. Casting to `int` truncates.
3. **`=` means "equals"** - No! `=` is assignment. `==` is comparison.
4. **Variables automatically initialize** - Local variables do NOT have default values; they must be initialized before use. Instance variables do have defaults (`0`, `0.0`, `false`, `null`).
5. **`%` only works on integers** - It works on `double` too in Java, but the AP exam focuses on integer modulus.
6. **`x = x + 1` is mathematically nonsensical** - In programming, it means "take the current value of x, add 1, and store the result back in x."

## Code Patterns and Examples

### Variable Declaration and Initialization
```java
int age = 25;
double gpa = 3.75;
boolean isStudent = true;
String name = "Alice";  // String is a reference type

final double TAX_RATE = 0.08;  // constant
```

### Integer Division vs. Double Division
```java
int a = 7 / 2;           // a = 3 (integer division, truncated)
double b = 7 / 2;        // b = 3.0 (still integer division, then widened)
double c = 7.0 / 2;      // c = 3.5 (double division)
double d = (double) 7 / 2; // d = 3.5 (cast forces double division)
```

### Modulus Operator
```java
int remainder = 17 % 5;   // remainder = 2
boolean isEven = (x % 2 == 0);  // check if x is even
int lastDigit = num % 10;       // extract last digit
```

### Casting
```java
double price = 9.99;
int dollars = (int) price;       // dollars = 9 (truncated)

int total = 7;
int count = 2;
double average = (double) total / count;  // 3.5, not 3.0
```

### Compound Assignment
```java
int score = 100;
score += 10;   // score = 110
score -= 5;    // score = 105
score *= 2;    // score = 210
score /= 3;    // score = 70
score %= 4;    // score = 2
```
