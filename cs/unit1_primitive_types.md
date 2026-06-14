# Unit 1: Primitive Types

**Exam Weight:** 2.5-5% | **Suggested Time:** ~8-10 class periods
**2025-26 Revision:** Merged into new Unit 1 "Using Objects and Methods"

## Topics

### Topic 1.1: Why Programming? Why Java?

This section covers how to use `System` class output methods to display text in the console.

- `System.out.print()` outputs text and leaves the cursor on the same line
- `System.out.println()` outputs text and moves to a new line automatically
- String literals must be enclosed in double quotes `""`
- Calling `System.out.println()` with no argument outputs a blank line

### Topic 1.2: Variables and Data Types

This section covers how to create string literals, choose appropriate data types, and declare variables of primitive types.

- The AP exam covers three primitive types: `int`, `double`, and `boolean`
- `int` stores whole numbers (no decimal point)
- `double` stores floating-point numbers (with decimal point)
- `boolean` can only hold `true` or `false`
- `String` is a reference type (not a primitive), covered in more detail in Unit 2
- Variable names are case-sensitive; the convention is camelCase
- Variables must be declared before use
- The `final` keyword declares a constant

### Topic 1.3: Expressions and Assignment Statements

This section covers how to assign initial values to variables and evaluate arithmetic expressions.

- The assignment operator `=` stores a value into a variable
- Arithmetic operators: `+`, `-`, `*`, `/`, `%` (remainder)
- Integer division truncates toward zero: `7 / 2` evaluates to `3`
- The remainder operator `%` returns what is left after division: `7 % 2` evaluates to `1`
- Operator precedence: `*`, `/`, `%` are evaluated before `+` and `-`
- Parentheses override default precedence
- Operators at the same precedence level evaluate left to right

### Topic 1.4: Compound Assignment Operators

This section covers how to evaluate expressions that use compound assignment operators.

- Compound assignment operators: `+=`, `-=`, `*=`, `/=`, `%=`
- Increment: `x++` or `++x` (adds 1 to x)
- Decrement: `x--` or `--x` (subtracts 1 from x)
- `x += 3` is equivalent to `x = x + 3`

### Topic 1.5: Casting and Ranges of Variables

This section covers how to evaluate expressions that involve type casting.

- Casting converts a value between types: `(int)`, `(double)`
- `(int) 3.7` evaluates to `3` (truncated, not rounded)
- `(double) 5` evaluates to `5.0`
- Widening: `int` is automatically promoted to `double` with no explicit cast needed
- Narrowing: converting `double` to `int` requires an explicit cast
- Range of `int`: -2,147,483,648 to 2,147,483,647 (`Integer.MIN_VALUE` to `Integer.MAX_VALUE`)
- Integer overflow: values that exceed the range wrap around silently
- Rounding trick: `(int)(x + 0.5)` rounds a positive double to the nearest integer

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Variable | A named storage location in memory |
| Data type | Determines what kind of data a variable can hold |
| Primitive type | A built-in Java type (`int`, `double`, `boolean`) |
| Literal | A fixed value written directly in the code (e.g., `42`, `3.14`, `true`) |
| Expression | A combination of values, variables, and operators that evaluates to a result |
| Assignment | The act of storing a value into a variable using `=` |
| Casting | Explicitly converting a value from one type to another |
| Truncation | Dropping the decimal portion (not rounding) |
| Overflow | When a value exceeds the range a data type can represent |

## Common Misconceptions

1. **Integer division returns a double** — It does not. `7 / 2` evaluates to `3`. Integer division only occurs when both operands are `int`. If either operand is `double`, the result is `double`.
2. **Casting rounds the value** — It does not. `(int) 3.9` evaluates to `3`, not `4`. Casting to `int` always truncates.
3. **`=` means "equals"** — In Java, `=` is the assignment operator. Use `==` for comparison.
4. **Variables initialize themselves** — Local variables have no default value and must be initialized before use. Instance variables do have defaults (`0`, `0.0`, `false`, `null`).
5. **`%` only works with integers** — Java's `%` also works with `double`, but the AP exam focuses on integer remainders.
6. **`x = x + 1` makes no mathematical sense** — In programming, this means "take the current value of x, add 1, and store the result back into x."

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
