# Unit 6: Array

**Exam Weight:** 10-15% | **Suggested Time:** ~6-8 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 6.1: Array Creation and Access
- **Learning Objective (VAR-2.K):** Represent collections of related primitive or object reference data using one-dimensional arrays
- **Essential Knowledge:**
  - Array declaration: `type[] arrayName;`
  - Array creation: `arrayName = new type[size];`
  - Combined: `int[] numbers = new int[5];`
  - Initializer list: `int[] numbers = {1, 2, 3, 4, 5};`
  - Indices range from 0 to `length - 1`
  - `arrayName.length` returns the number of elements (no parentheses!)
  - `ArrayIndexOutOfBoundsException` for invalid indices
  - Default values: `0` for `int`, `0.0` for `double`, `false` for `boolean`, `null` for objects
  - Array size is fixed after creation

### Topic 6.2: Traversing Arrays
- **Learning Objective (CON-2.F):** Traverse elements in a 1D array
- **Essential Knowledge:**
  - Forward traversal: `for (int i = 0; i < arr.length; i++)`
  - Backward traversal: `for (int i = arr.length - 1; i >= 0; i--)`
  - All elements or partial traversal
  - Off-by-one errors are the most common bug
  - Loop bound uses `.length` (not `.length - 1` for standard traversal with `<`)

### Topic 6.3: Enhanced for Loop for Arrays
- **Learning Objective (CON-2.G):** Traverse elements in a 1D array using an enhanced for loop
- **Essential Knowledge:**
  - Syntax: `for (type element : array)`
  - Reads as "for each element in array"
  - Cannot modify array elements through the loop variable
  - Cannot access the index
  - Cannot traverse backwards or skip elements
  - Best for read-only access to all elements

### Topic 6.4: Developing Algorithms Using Arrays
- **Learning Objective (CON-2.H):** Develop algorithms using 1D arrays
- **Essential Knowledge:**
  - Standard algorithms: find min/max, compute sum/average, count matches
  - Shift elements, reverse array
  - Search for a value (linear search)
  - Determine if all/any elements meet a condition
  - Identify duplicates
  - Access consecutive pairs: `arr[i]` and `arr[i+1]` (loop to `length - 1`)

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Array | A fixed-size, ordered collection of elements of the same type |
| Element | A single value stored in an array |
| Index | The position of an element (starting at 0) |
| Length | The number of elements in the array (`arr.length`) |
| Traversal | Visiting each element in the array |
| Enhanced for loop | A simplified loop for iterating through all elements |
| Linear search | Checking each element sequentially to find a target |
| Initializer list | Creating an array with predefined values: `{1, 2, 3}` |

## Common Misconceptions

1. **`arr.length()` with parentheses** - Arrays use `.length` (a field), NOT `.length()` (that's for Strings). No parentheses!
2. **Arrays are resizable** - No! Array size is fixed at creation. Use `ArrayList` for dynamic sizing.
3. **Enhanced for loop can modify elements** - Assigning to the loop variable does NOT change the array. The loop variable is a copy.
4. **Off-by-one in traversal** - `for (int i = 0; i <= arr.length; i++)` accesses index `arr.length` which is OUT OF BOUNDS.
5. **Array of objects contains objects** - No! It contains `null` references by default. Objects must be created and assigned individually.
6. **Arrays are passed by value** - Arrays are objects; the reference is passed. Changes to array elements inside a method ARE visible outside.
7. **Comparing arrays with `==`** - This compares references. To compare contents, loop through and compare element by element.

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
