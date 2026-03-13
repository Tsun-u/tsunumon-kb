# Unit 4: Iteration

**Exam Weight:** 17.5-22.5% | **Suggested Time:** ~14-16 class periods
**2025-26 Revision:** Merged into new Unit 2 "Selection and Iteration"

## Topics

### Topic 4.1: while Loops
- **Learning Objective (CON-2.A):** Represent iterative processes using a while loop
- **Essential Knowledge:**
  - `while (condition)` repeats as long as condition is `true`
  - Condition is checked BEFORE each iteration (pre-test loop)
  - If condition is initially `false`, the body never executes
  - Loop must eventually make the condition `false` (or infinite loop)
  - Loop body can contain any statements, including other loops

### Topic 4.2: for Loops
- **Learning Objective (CON-2.B):** Determine the number of times a for loop body executes
- **Essential Knowledge:**
  - `for (init; condition; update)` - three parts in the header
  - Initialization runs once before the loop starts
  - Condition is checked before each iteration
  - Update runs after each iteration
  - A `for` loop can always be rewritten as a `while` loop and vice versa
  - Loop variable scope: only accessible inside the loop (when declared in header)

### Topic 4.3: Developing Algorithms Using Strings
- **Learning Objective (CON-2.C):** Develop algorithms using Strings
- **Essential Knowledge:**
  - Traverse a String character by character using `substring(i, i+1)`
  - Standard algorithms: count characters, find/replace, reverse, check palindrome
  - String index range: 0 to `length() - 1`
  - Off-by-one errors are common with String traversal

### Topic 4.4: Nested Iteration
- **Learning Objective (CON-2.D):** Represent nested iterative processes
- **Essential Knowledge:**
  - Inner loop completes ALL iterations for EACH iteration of the outer loop
  - Total iterations = outer iterations x inner iterations
  - Common for 2D patterns, grids, and comparing all pairs
  - Each loop should use a different loop variable

### Topic 4.5: Informal Code Analysis
- **Learning Objective (CON-2.E):** Compute statement execution counts and informal run-time comparison
- **Essential Knowledge:**
  - Count how many times a statement executes in a loop
  - Nested loops: multiply the counts
  - Informal comparison of algorithms (e.g., linear vs. quadratic)

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Iteration | Repeating a block of code |
| Loop | A control structure that repeats code |
| Loop body | The block of code that is repeated |
| Loop condition | The Boolean expression that controls repetition |
| Infinite loop | A loop whose condition never becomes `false` |
| Off-by-one error | Iterating one too many or too few times |
| Sentinel value | A special value that signals the end of input |
| Accumulator | A variable that accumulates a result across iterations |
| Counter | A variable that tracks the number of iterations |
| Nested loop | A loop inside another loop |
| Trace | Following code execution step by step |

## Common Misconceptions

1. **Off-by-one errors** - Using `<` vs. `<=` in loop conditions. `for (int i = 0; i < n; i++)` runs n times; `for (int i = 0; i <= n; i++)` runs n+1 times.
2. **Infinite loops** - Forgetting to update the loop variable, or updating it in the wrong direction.
3. **Modifying loop variable inside for loop** - Leads to confusing behavior. Avoid changing the loop variable inside the body.
4. **Semicolon after loop header** - `for (int i = 0; i < 10; i++);` has an empty body. The indented code after it runs once.
5. **String traversal bounds** - Using `i <= str.length()` instead of `i < str.length()` causes `StringIndexOutOfBoundsException`.
6. **Nested loop confusion** - Students often confuse which loop variable controls what, especially in 2D patterns.
7. **while vs. for confusion** - Use `for` when the number of iterations is known; use `while` when it depends on a condition.

## Code Patterns and Examples

### while Loop
```java
// Count-controlled
int count = 0;
while (count < 5) {
    System.out.println(count);
    count++;
}
// Output: 0, 1, 2, 3, 4

// Sentinel-controlled
int sum = 0;
int input = scanner.nextInt();
while (input != -1) {
    sum += input;
    input = scanner.nextInt();
}
```

### for Loop
```java
// Standard counting loop
for (int i = 0; i < 10; i++) {
    System.out.print(i + " ");
}
// Output: 0 1 2 3 4 5 6 7 8 9

// Counting backwards
for (int i = 10; i >= 1; i--) {
    System.out.print(i + " ");
}
// Output: 10 9 8 7 6 5 4 3 2 1

// Step by 2
for (int i = 0; i < 20; i += 2) {
    System.out.print(i + " ");
}
// Output: 0 2 4 6 8 10 12 14 16 18
```

### String Traversal
```java
String word = "Hello";

// Print each character
for (int i = 0; i < word.length(); i++) {
    String ch = word.substring(i, i + 1);
    System.out.println(ch);
}

// Count vowels
int vowelCount = 0;
for (int i = 0; i < word.length(); i++) {
    String ch = word.substring(i, i + 1);
    if ("AEIOUaeiou".indexOf(ch) >= 0) {
        vowelCount++;
    }
}

// Reverse a String
String reversed = "";
for (int i = word.length() - 1; i >= 0; i--) {
    reversed += word.substring(i, i + 1);
}
// reversed = "olleH"
```

### Nested Loops
```java
// Multiplication table
for (int row = 1; row <= 5; row++) {
    for (int col = 1; col <= 5; col++) {
        System.out.printf("%4d", row * col);
    }
    System.out.println();
}

// Triangle pattern
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        System.out.print("*");
    }
    System.out.println();
}
// Output:
// *
// **
// ***
// ****
// *****
```

### Standard Algorithms

```java
// Find maximum in a sequence
int max = Integer.MIN_VALUE;
for (int i = 0; i < n; i++) {
    int value = scanner.nextInt();
    if (value > max) {
        max = value;
    }
}

// Compute average
int sum = 0;
int count = 0;
for (int i = 0; i < n; i++) {
    sum += values[i];
    count++;
}
double average = (double) sum / count;

// Digits of a number
int num = 12345;
while (num > 0) {
    int digit = num % 10;
    System.out.println(digit);
    num /= 10;
}
// Output: 5, 4, 3, 2, 1
```

### Equivalent Loop Forms
```java
// These are equivalent:
// for loop version
for (int i = 0; i < 10; i++) {
    System.out.println(i);
}

// while loop version
int i = 0;
while (i < 10) {
    System.out.println(i);
    i++;
}
```
