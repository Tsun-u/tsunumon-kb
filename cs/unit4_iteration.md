# Unit 4: Iteration

**Exam Weight:** 17.5-22.5% | **Suggested Time:** ~14-16 class periods
**2025-26 Revision:** Merged into new Unit 2 "Selection and Iteration"

## Topics

### Topic 4.1: while Loops

This section covers how to express repetition using while loops.

- `while (condition)` keeps repeating as long as the condition remains `true`
- The condition is checked before each execution of the loop body (pre-test loop)
- If the condition is `false` from the start, the loop body never runs
- The loop body must eventually make the condition `false`; otherwise an infinite loop results
- The loop body can contain any statements, including other loops

### Topic 4.2: for Loops

This section covers how to determine how many times a for loop body executes.

- `for (init; condition; update)` — the header has three parts
- The initialization runs once before the loop begins
- The condition is checked before each iteration
- The update runs after each iteration
- Any for loop can be rewritten as a while loop, and vice versa
- A loop variable declared in the header is scoped to the loop

### Topic 4.3: Developing Algorithms Using Strings

This section covers how to develop algorithms that process strings.

- Use `substring(i, i+1)` to visit each character in a string one at a time
- Common algorithms: counting characters, finding or replacing, reversing, checking for palindromes
- Valid string indices run from 0 to `length() - 1`
- Off-by-one errors are the most frequent mistake when traversing strings

### Topic 4.4: Nested Iteration

This section covers how to express nested repetition.

- Each time the outer loop iterates, the inner loop completes all of its iterations
- Total executions = outer iterations × inner iterations
- Common uses: two-dimensional patterns, tables, comparing all pairs of elements
- Each loop level should use a distinct loop variable

### Topic 4.5: Informal Code Analysis

This section covers how to count statement executions and informally compare algorithm efficiency.

- Count how many times a statement inside a loop runs
- For nested loops, multiply the iteration counts of each level
- Informally compare algorithms (e.g., linear vs. quadratic growth)

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Iteration | Repeating a block of code multiple times |
| Loop | A control structure that repeats code |
| Loop body | The block of code that gets repeated |
| Loop condition | A boolean expression that controls whether the loop continues |
| Infinite loop | A loop whose condition never becomes `false` |
| Off-by-one error | A bug where the loop runs one too many or one too few times |
| Sentinel value | A special value used to signal the end of input |
| Accumulator | A variable that collects a running result across iterations |
| Counter | A variable that tracks the number of iterations |
| Nested loop | A loop placed inside another loop |
| Trace | Manually stepping through code to track its execution |

## Common Misconceptions

1. **Off-by-one errors** — Whether to use `<` or `<=` matters significantly. `for (int i = 0; i < n; i++)` runs n times; `for (int i = 0; i <= n; i++)` runs n+1 times.
2. **Infinite loops** — Forgetting to update the loop variable, or updating it in the wrong direction, causes the loop to run forever.
3. **Modifying the loop variable inside the loop body** — This leads to unpredictable behavior and should be avoided.
4. **Placing a semicolon after the loop header** — `for (int i = 0; i < 10; i++);` has an empty loop body; the indented code that follows runs only once.
5. **String traversal boundaries** — Using `i <= str.length()` instead of `i < str.length()` causes a `StringIndexOutOfBoundsException`.
6. **Confusing nested loop variables** — In two-dimensional patterns, it is easy to lose track of which variable controls which direction.
7. **Choosing between while and for** — Use `for` when the number of iterations is known in advance; use `while` when the loop should continue based on a condition.

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
