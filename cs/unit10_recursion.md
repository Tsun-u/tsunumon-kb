# Unit 10: Recursion

**Exam Weight (pre-2025):** 5-7.5% | **Suggested Time:** ~5-7 class periods
**2025-26 Revision:** REMOVED from required content. Recursion is no longer tested on the AP exam starting 2025-26. This file documents the original framework for reference.

## Topics

### Topic 10.1: Recursion
- **Learning Objective (CON-2.O):** Determine the result of a recursive method call
- **Essential Knowledge:**
  - Recursion: a method that calls itself
  - Every recursive method needs a **base case** (stopping condition)
  - Every recursive method needs a **recursive case** that moves toward the base case
  - Without a base case or progress toward it: `StackOverflowError`
  - Each recursive call creates a new stack frame with its own local variables
  - Recursion can solve problems that have self-similar subproblems

### Topic 10.2: Recursive Searching and Sorting
- **Learning Objective (CON-2.P):** Apply recursive search and sort algorithms
- **Essential Knowledge:**
  - **Binary search** (recursive): divides sorted array in half each step
  - Binary search requires a SORTED array
  - Binary search is O(log n) - much faster than linear search for large arrays
  - **Merge sort** (recursive): divide array in half, sort each half, merge
  - Merge sort is O(n log n) - faster than selection/insertion sort
  - Students should trace through recursive algorithms
  - Students should understand the efficiency comparison

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Recursion | A method calling itself to solve a problem |
| Base case | The condition that stops recursion |
| Recursive case | The part that calls the method again with a smaller problem |
| Call stack | The stack of method calls waiting to complete |
| Stack frame | Memory allocated for each method call's local variables |
| StackOverflowError | Error from too many recursive calls (no base case or no progress) |
| Binary search | Divide-and-conquer search on a sorted array |
| Merge sort | Divide-and-conquer sorting algorithm |
| Divide and conquer | Breaking a problem into smaller subproblems |

## Common Misconceptions

1. **Forgetting the base case** - Without a base case, recursion never stops, causing `StackOverflowError`.
2. **Not making progress toward base case** - Each recursive call must bring the problem closer to the base case.
3. **Recursion is always better than iteration** - Not necessarily. Recursion uses more memory (call stack) and can be slower. Some problems are naturally recursive; others are better iterative.
4. **Binary search works on unsorted arrays** - No! The array MUST be sorted for binary search to work correctly.
5. **Tracing recursion** - Students often struggle to track which call is executing. Draw the call stack!
6. **Return values in recursion** - Each recursive call returns its own value. The final result depends on how return values are combined.
7. **Modifying parameters vs. return values** - Recursive methods typically work by passing modified parameters and returning accumulated results.

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
