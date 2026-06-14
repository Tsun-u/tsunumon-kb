# Unit 3: Boolean Expressions and if Statements

**Exam Weight:** 15-17.5% | **Suggested Time:** ~11-13 class periods
**2025-26 Revision:** Merged into new Unit 2 "Selection and Iteration"

## Topics

### Topic 3.1: Boolean Expressions

This section covers how to evaluate boolean expressions that use relational operators.

- Relational operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
- These operators compare two values and produce `true` or `false`
- For primitive types, `==` compares the values themselves
- For objects, `==` compares references (memory addresses), not content
- To compare the content of objects, use `.equals()` (especially for strings)

### Topic 3.2: if Statements and Control Flow

This section covers how to trace the execution flow of if statements.

- `if (condition)` executes the block only when the condition is `true`
- Curly braces `{}` define the controlled block; without them, only the immediately following statement is controlled by the if
- The condition is evaluated at runtime

### Topic 3.3: if-else Statements

This section covers how to trace the execution flow of if-else statements.

- `if-else` provides exactly two paths: one for when the condition is `true`, one for `false`
- Exactly one of the two branches will execute
- The else block has no condition of its own

### Topic 3.4: else if Statements

This section covers how to trace the execution flow of else if chains.

- An `else if` chain tests multiple conditions in sequence
- Conditions are evaluated top to bottom; the first one that is `true` runs its block
- Only one block in the entire if-else if-else chain executes
- The order in which conditions are written matters when they overlap

### Topic 3.5: Compound Boolean Expressions

This section covers how to evaluate compound boolean expressions.

- Logical operators: `&&` (AND), `||` (OR), `!` (NOT)
- `&&` returns `true` only when both operands are `true`
- `||` returns `true` when at least one operand is `true`
- `!` inverts a boolean value
- Precedence order: `!` > `&&` > `||`
- Short-circuit evaluation: `&&` skips the right side when the left is `false`; `||` skips the right side when the left is `true`

### Topic 3.6: Equivalent Boolean Expressions

This section covers how to determine whether two boolean expressions are equivalent.

- De Morgan's Laws:
  - `!(a && b)` is equivalent to `!a || !b`
  - `!(a || b)` is equivalent to `!a && !b`
- These rules can simplify complex conditions
- Truth tables can be used to verify that two expressions are equivalent

### Topic 3.7: Comparing Objects

This section covers how to compare objects using `==` and `.equals()`.

- `==` checks whether two references point to the same object
- `.equals()` checks whether two objects have the same content
- Checking for null: use `obj == null` or `obj != null`
- Calling `.equals()` on a `null` reference throws `NullPointerException`

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Boolean expression | An expression that evaluates to either `true` or `false` |
| Relational operator | An operator that compares two values (`==`, `!=`, `<`, `>`, `<=`, `>=`) |
| Logical operator | An operator that combines boolean values (`&&`, `\|\|`, `!`) |
| Control flow | The order in which statements are executed in a program |
| Selection | Choosing which block of code to run based on a condition |
| Short-circuit evaluation | Stopping evaluation of the right operand when the result is already determined |
| De Morgan's Laws | Rules that describe how to distribute `!` across `&&` and `\|\|` |
| Nested if | An if statement placed inside another if statement |
| Dangling else | An ambiguous situation where an else could match more than one if |

## Common Misconceptions

1. **Using `=` instead of `==`** — `=` is the assignment operator; `==` is the comparison operator. `if (x = 5)` causes a compile error for integers in Java (unlike C/C++).
2. **Comparing strings with `==`** — `"hello" == "hello"` may work by coincidence due to string pooling, but `new String("hello") == new String("hello")` is `false`. Always use `.equals()`.
3. **Placing a semicolon after the if condition** — `if (x > 0);` ends the if statement at the semicolon, so the indented line that follows always executes. This is a silent bug that is easy to miss.
4. **Confusing De Morgan's Laws** — Many people forget that the operator also flips: `!(a && b)` becomes `!a || !b` (AND becomes OR, and vice versa).
5. **Short-circuit order surprises** — In `if (obj != null && obj.getValue() > 0)`, if `obj` is null the second condition is safely skipped. Reversing the order would cause a crash.
6. **Omitting curly braces** — Without `{}`, only the first statement after the `if` is conditionally controlled, which is a common source of bugs.
7. **Overlapping else-if conditions** — When conditions overlap, only the first matching branch runs. For example, `grade >= 90` must appear before `grade >= 80`.

## Code Patterns and Examples

### Basic if-else-if
```java
int score = 85;
String grade;

if (score >= 90) {
    grade = "A";
} else if (score >= 80) {
    grade = "B";
} else if (score >= 70) {
    grade = "C";
} else if (score >= 60) {
    grade = "D";
} else {
    grade = "F";
}
```

### Compound Boolean Expressions
```java
// Range check: is x between 1 and 100 (inclusive)?
if (x >= 1 && x <= 100) {
    System.out.println("In range");
}

// Either condition
if (day.equals("Saturday") || day.equals("Sunday")) {
    System.out.println("Weekend!");
}

// Negation
if (!(x > 0)) {
    System.out.println("Non-positive");
}
// Equivalent to:
if (x <= 0) {
    System.out.println("Non-positive");
}
```

### De Morgan's Laws
```java
// These pairs are equivalent:
!(a && b)    ==    !a || !b
!(a || b)    ==    !a && !b

// Example:
// "NOT (sunny AND warm)" == "NOT sunny OR NOT warm"
if (!(isSunny && isWarm)) { ... }
if (!isSunny || !isWarm) { ... }  // equivalent
```

### Comparing Objects
```java
String s1 = "hello";
String s2 = new String("hello");
String s3 = s1;

s1 == s2;       // false (different objects)
s1 == s3;       // true (same reference)
s1.equals(s2);  // true (same content)

// Safe null check pattern
if (str != null && str.length() > 0) {
    // str is non-null and non-empty
}
```

### Short-Circuit Evaluation
```java
// Safe: short-circuit prevents NullPointerException
if (list != null && list.size() > 0) {
    // process list
}

// Dangerous: would crash if list is null
if (list.size() > 0 && list != null) {
    // NullPointerException if list is null!
}
```

### Nested if Statements
```java
if (age >= 16) {
    if (hasLicense) {
        System.out.println("Can drive");
    } else {
        System.out.println("Need a license");
    }
} else {
    System.out.println("Too young to drive");
}
```
