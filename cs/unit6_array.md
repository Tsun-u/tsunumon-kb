# Unit 6: Array

**Exam Weight:** 10-15% | **Suggested Time:** ~6-8 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 6.1: Array Creation and Access

This section covers how to use a one-dimensional array to represent a collection of related primitive values or object references.

- Array declaration: `type[] arrayName;`
- Array creation: `arrayName = new type[size];`
- Combined form: `int[] numbers = new int[5];`
- Initializer list: `int[] numbers = {1, 2, 3, 4, 5};`
- Valid indices run from 0 to `length - 1`
- `arrayName.length` returns the number of elements (no parentheses!)
- Accessing an invalid index throws `ArrayIndexOutOfBoundsException`
- Default values: `int` → `0`, `double` → `0.0`, `boolean` → `false`, objects → `null`
- Array size is fixed after creation; it cannot be resized

### Topic 6.2: Traversing Arrays

This section covers how to visit every element in a one-dimensional array.

- Forward traversal: `for (int i = 0; i < arr.length; i++)`
- Backward traversal: `for (int i = arr.length - 1; i >= 0; i--)`
- You can traverse all elements or only a subset
- Off-by-one errors are the most common bug
- When using `<` in the condition, the bound is `.length` (not `.length - 1`)

### Topic 6.3: Enhanced for Loop for Arrays

This section covers how to use the enhanced for loop to traverse a one-dimensional array.

- Syntax: `for (type element : array)`
- Read as "for each element in array"
- Cannot modify array elements through the loop variable
- Cannot access the current index
- Cannot traverse in reverse or skip elements
- Best suited for read-only access to every element

### Topic 6.4: Developing Algorithms Using Arrays

This section covers how to develop algorithms that use one-dimensional arrays.

- Standard algorithms: finding min/max, computing sum/average, counting elements that meet a condition
- Shifting elements, reversing an array
- Linear search for a value
- Checking whether all or some elements satisfy a condition
- Identifying duplicate elements
- Accessing adjacent pairs: `arr[i]` and `arr[i+1]` (loop up to `length - 1`)

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Array | A fixed-size, ordered collection of elements of the same type |
| Element | A single value stored in an array |
| Index | The position of an element in an array (starts at 0) |
| Length | The number of elements in an array (`arr.length`) |
| Traversal | Visiting each element in an array in sequence |
| Enhanced for loop | A simplified loop syntax for iterating over all elements |
| Linear search | A search that checks each element one by one until the target is found |
| Initializer list | A way to create an array with predefined values: `{1, 2, 3}` |

## Common Misconceptions

1. **Writing `arr.length()`** — Arrays use `.length` (a field), not `.length()` (which is a String method). There are no parentheses for array length.
2. **Arrays can be resized** — They cannot. Once created, an array's size is fixed. Use `ArrayList` when dynamic resizing is needed.
3. **The enhanced for loop can modify elements** — Assigning to the loop variable does not change the array. The variable is just a copy of the element.
4. **Off-by-one during traversal** — `for (int i = 0; i <= arr.length; i++)` attempts to access index `arr.length`, which is out of bounds.
5. **Object arrays already contain objects** — They do not. An array of object references is initialized to `null`. Each object must be created and assigned individually.
6. **Arrays are passed by value** — Arrays are objects; what gets passed is a reference. Modifying array elements inside a method is visible outside the method.
7. **Comparing arrays with `==`** — This compares references, not content. To compare the contents of two arrays, you must check each element individually.

## Code Patterns and Examples

### Array Creation
```java
// Declaration and creation
int[] scores = new int[5];        // [0, 0, 0, 0, 0]
double[] prices = new double[3];  // [0.0, 0.0, 0.0]
String[] names = new String[4];   // [null, null, null, null]

// Initializer list
int[] primes = {2, 3, 5, 7, 11};
String[] days = {"Mon", "Tue", "Wed", "Thu", "Fri"};
```

### Array Traversal
```java
int[] arr = {10, 20, 30, 40, 50};

// Standard for loop (full control)
for (int i = 0; i < arr.length; i++) {
    System.out.println("Index " + i + ": " + arr[i]);
}

// Enhanced for loop (read-only)
for (int val : arr) {
    System.out.println(val);
}

// Backward traversal
for (int i = arr.length - 1; i >= 0; i--) {
    System.out.println(arr[i]);
}
```

### Standard Algorithms

```java
int[] arr = {34, 12, 78, 56, 23};

// Find maximum
int max = arr[0];
for (int i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
        max = arr[i];
    }
}
// max = 78

// Find minimum
int min = arr[0];
for (int i = 1; i < arr.length; i++) {
    if (arr[i] < min) {
        min = arr[i];
    }
}
// min = 12

// Sum and average
int sum = 0;
for (int val : arr) {
    sum += val;
}
double average = (double) sum / arr.length;

// Count elements matching a condition
int count = 0;
for (int val : arr) {
    if (val > 30) {
        count++;
    }
}

// Linear search
int target = 56;
int foundIndex = -1;
for (int i = 0; i < arr.length; i++) {
    if (arr[i] == target) {
        foundIndex = i;
        break;
    }
}

// Check if all elements are positive
boolean allPositive = true;
for (int val : arr) {
    if (val <= 0) {
        allPositive = false;
        break;
    }
}

// Check if any element is negative
boolean anyNegative = false;
for (int val : arr) {
    if (val < 0) {
        anyNegative = true;
        break;
    }
}
```

### Shift Elements
```java
// Shift left (remove first element)
for (int i = 0; i < arr.length - 1; i++) {
    arr[i] = arr[i + 1];
}
arr[arr.length - 1] = 0;  // fill last position

// Shift right (remove last element)
for (int i = arr.length - 1; i > 0; i--) {
    arr[i] = arr[i - 1];
}
arr[0] = 0;  // fill first position
```

### Reverse an Array
```java
for (int i = 0; i < arr.length / 2; i++) {
    int temp = arr[i];
    arr[i] = arr[arr.length - 1 - i];
    arr[arr.length - 1 - i] = temp;
}
```

### Enhanced For Loop Limitation
```java
int[] arr = {1, 2, 3, 4, 5};

// This does NOT modify the array!
for (int val : arr) {
    val = val * 2;  // only modifies the local copy
}
// arr is still {1, 2, 3, 4, 5}

// Must use standard for loop to modify:
for (int i = 0; i < arr.length; i++) {
    arr[i] = arr[i] * 2;  // actually modifies the array
}
// arr is now {2, 4, 6, 8, 10}
```
