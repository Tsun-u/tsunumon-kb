# Unit 10: Recursion

**Exam Weight (pre-2025):** 5-7.5% | **Suggested Time:** ~5-7 class periods
**2025-26 Revision:** REMOVED from required content. Recursion is no longer tested on the AP exam starting 2025-26. This file documents the original framework for reference.

## Topics

### Topic 10.1: Recursion

This section covers how to determine the result of a recursive method call.

- Recursion: a method calls itself as part of its own definition
- Every recursive method needs a **base case** — the condition that stops the recursion
- Every recursive method needs a **recursive case** — the part that moves the problem toward the base case
- Without a base case, or if the recursive case never converges, a `StackOverflowError` occurs
- Each recursive call creates a new stack frame with its own local variables
- Recursion is well-suited for problems with self-similar subproblems

### Topic 10.2: Recursive Searching and Sorting

This section covers how to apply recursive searching and sorting algorithms.

- **Binary search (recursive version):** repeatedly cuts a sorted array in half
- Binary search requires the array to already be sorted
- Binary search runs in O(log n) time — much faster than linear search for large arrays
- **Merge sort (recursive version):** splits the array in half, sorts each half, then merges them
- Merge sort runs in O(n log n) time — faster than selection sort or insertion sort
- The exam requires tracing the execution of recursive algorithms
- The exam requires understanding the efficiency differences between algorithms

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Recursion | A technique where a method solves a problem by calling itself |
| Base case | The condition that causes the recursion to stop |
| Recursive case | The part that calls the method again with a smaller subproblem |
| Call stack | The stack of method calls that are waiting to complete |
| Stack frame | The memory allocated for each method call to store its local variables |
| StackOverflowError | The error produced when recursive calls go too deep (no base case or no convergence) |
| Binary search | A search on a sorted array that uses divide-and-conquer |
| Merge sort | A sorting algorithm that uses divide-and-conquer |
| Divide and conquer | A strategy that breaks a problem into smaller subproblems and solves each independently |

## Common Misconceptions

1. **Forgetting the base case** — Without a base case, the recursion never stops, eventually producing a `StackOverflowError`.
2. **The recursive case does not approach the base case** — Each recursive call must reduce the problem size so it moves closer to the base case.
3. **Recursion is always better than iteration** — It is not. Recursion uses more memory (call stack growth) and can be slower. Some problems are naturally recursive; others are better solved with loops.
4. **Binary search works on unsorted arrays** — It does not. The array must be sorted for binary search to produce correct results.
5. **Tracing recursion is too difficult** — Many people lose track of which call level is active. Drawing a call stack diagram helps clarify the execution.
6. **Return values in recursion** — Each recursive call has its own return value. The final result depends on how all those values are combined as the calls unwind.
7. **Modifying parameters vs. returning values** — Recursive methods typically work by passing a modified argument and returning an accumulated result.

## Code Patterns and Examples

### Basic Recursion: Factorial
```java
// n! = n * (n-1) * (n-2) * ... * 1
// Base case: 0! = 1
public static int factorial(int n) {
    if (n == 0) {              // base case
        return 1;
    }
    return n * factorial(n - 1); // recursive case
}

// Trace: factorial(4)
// factorial(4) = 4 * factorial(3)
//              = 4 * 3 * factorial(2)
//              = 4 * 3 * 2 * factorial(1)
//              = 4 * 3 * 2 * 1 * factorial(0)
//              = 4 * 3 * 2 * 1 * 1
//              = 24
```

### Fibonacci (Classic but Inefficient)
```java
public static int fibonacci(int n) {
    if (n <= 1) {          // base cases
        return n;
    }
    return fibonacci(n - 1) + fibonacci(n - 2);  // two recursive calls
}
// fibonacci(5) = 5
// Note: This is O(2^n) - very inefficient! Many repeated calculations.
```

### Power
```java
public static double power(double base, int exp) {
    if (exp == 0) {
        return 1.0;
    }
    return base * power(base, exp - 1);
}
// power(2, 5) = 2 * 2 * 2 * 2 * 2 * 1 = 32.0
```

### String Recursion
```java
// Reverse a String
public static String reverse(String str) {
    if (str.length() <= 1) {
        return str;
    }
    return reverse(str.substring(1)) + str.substring(0, 1);
}
// reverse("hello")
// = reverse("ello") + "h"
// = reverse("llo") + "e" + "h"
// = reverse("lo") + "l" + "e" + "h"
// = reverse("o") + "l" + "l" + "e" + "h"
// = "o" + "l" + "l" + "e" + "h"
// = "olleh"

// Count occurrences of a character
public static int countChar(String str, String ch) {
    if (str.length() == 0) {
        return 0;
    }
    int count = str.substring(0, 1).equals(ch) ? 1 : 0;
    return count + countChar(str.substring(1), ch);
}
```

### Binary Search (Recursive)
```java
public static int binarySearch(int[] arr, int target, int low, int high) {
    if (low > high) {
        return -1;  // base case: not found
    }

    int mid = (low + high) / 2;

    if (arr[mid] == target) {
        return mid;              // base case: found
    } else if (arr[mid] < target) {
        return binarySearch(arr, target, mid + 1, high);  // search right half
    } else {
        return binarySearch(arr, target, low, mid - 1);   // search left half
    }
}

// Usage:
int[] sorted = {2, 5, 8, 12, 16, 23, 38, 56, 72, 91};
int index = binarySearch(sorted, 23, 0, sorted.length - 1);
// index = 5

// Trace: binarySearch(sorted, 23, 0, 9)
// mid = 4, arr[4] = 16 < 23 → search right
// binarySearch(sorted, 23, 5, 9)
// mid = 7, arr[7] = 56 > 23 → search left
// binarySearch(sorted, 23, 5, 6)
// mid = 5, arr[5] = 23 == 23 → return 5
```

### Merge Sort (Conceptual)
```java
public static void mergeSort(int[] arr, int left, int right) {
    if (left < right) {
        int mid = (left + right) / 2;
        mergeSort(arr, left, mid);       // sort left half
        mergeSort(arr, mid + 1, right);  // sort right half
        merge(arr, left, mid, right);    // merge sorted halves
    }
}

// merge() combines two sorted halves into one sorted portion
// Students should understand the concept, not necessarily write merge()
```

### Recursion vs. Iteration Comparison
```java
// Sum of 1 to n - Recursive
public static int sumRecursive(int n) {
    if (n == 0) return 0;
    return n + sumRecursive(n - 1);
}

// Sum of 1 to n - Iterative
public static int sumIterative(int n) {
    int sum = 0;
    for (int i = 1; i <= n; i++) {
        sum += i;
    }
    return sum;
}

// Both produce the same result
// Iterative is more memory-efficient (no call stack buildup)
// Recursive is sometimes more elegant and readable
```

### Algorithm Efficiency Comparison

| Algorithm | Time Complexity | Notes |
|-----------|----------------|-------|
| Linear search | O(n) | Works on unsorted data |
| Binary search | O(log n) | Requires sorted data |
| Selection sort | O(n^2) | Simple but slow |
| Insertion sort | O(n^2) | Good for nearly sorted data |
| Merge sort | O(n log n) | Fast, uses extra memory |
