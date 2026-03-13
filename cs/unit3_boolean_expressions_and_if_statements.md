# Unit 3: Boolean Expressions and if Statements

**Exam Weight:** 15-17.5% | **Suggested Time:** ~11-13 class periods
**2025-26 Revision:** Merged into new Unit 2 "Selection and Iteration"

## Topics

### Topic 3.1: Boolean Expressions
- **Learning Objective (CON-1.A):** Evaluate Boolean expressions that use relational operators
- **Essential Knowledge:**
  - Relational operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
  - These operators compare two values and return `true` or `false`
  - For primitives, `==` compares values
  - For objects, `==` compares references (memory addresses), NOT content
  - Use `.equals()` to compare object content (especially Strings)

### Topic 3.2: if Statements and Control Flow
- **Learning Objective (CON-1.B):** Evaluate if statements
- **Essential Knowledge:**
  - `if (condition)` executes the block only when condition is `true`
  - Curly braces `{}` define the block; without them, only the next statement is controlled
  - Conditions are evaluated at runtime

### Topic 3.3: if-else Statements
- **Learning Objective (CON-1.C):** Evaluate if-else statements
- **Essential Knowledge:**
  - `if-else` provides two paths: one for `true`, one for `false`
  - Exactly one branch executes
  - The else block has no condition

### Topic 3.4: else if Statements
- **Learning Objective (CON-1.D):** Evaluate else if statements
- **Essential Knowledge:**
  - `else if` chains test multiple conditions in sequence
  - Conditions are evaluated top to bottom; first `true` condition's block executes
  - Only ONE block executes in an if-else if-else chain
  - Order matters when conditions overlap

### Topic 3.5: Compound Boolean Expressions
- **Learning Objective (CON-1.E):** Evaluate compound Boolean expressions
- **Essential Knowledge:**
  - Logical operators: `&&` (AND), `||` (OR), `!` (NOT)
  - `&&` is `true` only when BOTH operands are `true`
  - `||` is `true` when AT LEAST ONE operand is `true`
  - `!` inverts the Boolean value
  - Precedence: `!` > `&&` > `||`
  - Short-circuit evaluation: `&&` stops if left is `false`; `||` stops if left is `true`

### Topic 3.6: Equivalent Boolean Expressions
- **Learning Objective (CON-1.F):** Evaluate equivalent Boolean expressions
- **Essential Knowledge:**
  - De Morgan's Laws:
    - `!(a && b)` is equivalent to `!a || !b`
    - `!(a || b)` is equivalent to `!a && !b`
  - Useful for simplifying complex conditions
  - Truth tables can verify equivalence

### Topic 3.7: Comparing Objects
- **Learning Objective (CON-1.G):** Compare object references using `==` and `.equals()`
- **Essential Knowledge:**
  - `==` checks if two references point to the SAME object
  - `.equals()` checks if two objects have the SAME content
  - `null` check: use `obj == null` or `obj != null`
  - Calling `.equals()` on `null` throws `NullPointerException`

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Boolean expression | An expression that evaluates to `true` or `false` |
| Relational operator | Compares two values (`==`, `!=`, `<`, `>`, `<=`, `>=`) |
| Logical operator | Combines Boolean values (`&&`, `\|\|`, `!`) |
| Control flow | The order in which statements are executed |
| Selection | Choosing which code to execute based on a condition |
| Short-circuit evaluation | Skipping evaluation of the right operand when the result is already determined |
| De Morgan's Laws | Rules for distributing `!` over `&&` and `\|\|` |
| Nested if | An if statement inside another if statement |
| Dangling else | An else that could be matched to multiple if statements |

## Common Misconceptions

1. **Using `=` instead of `==`** - `=` is assignment, `==` is comparison. `if (x = 5)` is a compilation error for `int` (unlike C/C++).
2. **Comparing Strings with `==`** - `"hello" == "hello"` may work due to String pooling, but `new String("hello") == new String("hello")` is `false`. Always use `.equals()`.
3. **Semicolon after if condition** - `if (x > 0);` terminates the if statement; the next line always executes. This is a common silent bug.
4. **De Morgan's Laws confusion** - Students often forget to flip the operator: `!(a && b)` is `!a || !b` (AND becomes OR, and vice versa).
5. **Short-circuit evaluation surprises** - In `if (obj != null && obj.getValue() > 0)`, the second condition is safely skipped if `obj` is `null`. Reversing the order would crash.
6. **Missing braces** - Without `{}`, only the FIRST statement after `if` is conditional. This is a major source of bugs.
7. **Overlapping conditions in else-if** - If conditions overlap, only the first matching branch runs. E.g., grade >= 90 should come before grade >= 80.

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
