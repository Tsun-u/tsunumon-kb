# Unit 7: ArrayList

**Exam Weight:** 2.5-7.5% | **Suggested Time:** ~8-10 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 7.1: Introduction to ArrayList

This section covers how to use ArrayList objects to represent a collection of related object references.

- `ArrayList` is a resizable array — elements can be added or removed after creation
- Must be imported before use: `import java.util.ArrayList;`
- Can only store object references, not primitive types directly
- Uses generic syntax: `ArrayList<Type>`
- Write `ArrayList<Integer>` not `ArrayList<int>` (wrapper classes required)
- The initial size (number of elements) is 0; capacity adjusts automatically

### Topic 7.2: ArrayList Methods

This section covers how to call ArrayList methods.

- `int size()` — returns the current number of elements
- `boolean add(E obj)` — appends an element to the end, returns `true`
- `void add(int index, E obj)` — inserts an element at the given index, shifting later elements right
- `E get(int index)` — returns the element at the given index
- `E set(int index, E obj)` — replaces the element at the given index, returns the old element
- `E remove(int index)` — removes and returns the element at the given index, shifting later elements left
- An invalid index throws `IndexOutOfBoundsException`
- Valid indices run from 0 to `size() - 1`

### Topic 7.3: Traversing ArrayLists

This section covers how to traverse all elements in an ArrayList.

- Standard for loop: `for (int i = 0; i < list.size(); i++)`
- Enhanced for loop: `for (Type item : list)`
- Use `list.size()` rather than `list.length`
- When removing elements during traversal, iterate backward or adjust the index after removal
- Adding or removing elements inside an enhanced for loop throws `ConcurrentModificationException`

### Topic 7.4: Developing Algorithms Using ArrayLists

This section covers how to develop algorithms that use ArrayLists.

- The same standard algorithms as arrays (min, max, sum, search) apply
- Inserting while maintaining sorted order
- Removing duplicate elements
- Modifying the list during traversal (requires care)
- ArrayLists can grow and shrink, enabling algorithms that fixed-size arrays cannot easily support

### Topic 7.5: Searching

This section covers how to apply a sequential (linear) search algorithm.

- Linear search checks each element in order
- Works on both arrays and ArrayLists
- Returns the index when found, or -1 when not found
- Time complexity is O(n) (informal understanding)

### Topic 7.6: Sorting

This section covers how to apply selection sort and insertion sort algorithms.

- **Selection sort:** Find the smallest value in the unsorted portion, swap it to the front, repeat for the remainder
- **Insertion sort:** Take the next element and insert it into its correct position in the already-sorted portion
- Both have O(n^2) worst-case performance
- The exam requires tracing sort steps, not writing sort code from scratch

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| ArrayList | A dynamically resizable ordered collection of object references |
| Generics | Type parameters specified with angle brackets, e.g., `<String>` |
| Wrapper class | The object version of a primitive type (`Integer`, `Double`, `Boolean`) |
| Autoboxing | Automatic conversion of a primitive to its corresponding wrapper object |
| Unboxing | Automatic conversion of a wrapper object back to a primitive |
| Linear search | A search that checks each element one by one |
| Selection sort | A sort that repeatedly finds the minimum and moves it to its correct position |
| Insertion sort | A sort that builds a sorted portion by inserting each element into the right place |
| Size | The current number of elements in an ArrayList |

## Common Misconceptions

1. **`ArrayList<int>`** — This is invalid. Wrapper classes must be used: `ArrayList<Integer>`. Primitive types cannot serve as type parameters.
2. **`list.length`** — ArrayLists use `list.size()` (with parentheses). The `length` field (no parentheses) belongs to arrays.
3. **Removing elements during forward traversal** — This causes elements to be skipped. After removing the element at index `i`, the next element shifts to index `i`, but `i` increments, bypassing it. Traverse backward or decrement `i` after removal.
4. **Modifying an ArrayList inside an enhanced for loop** — Adding or removing elements throws `ConcurrentModificationException`.
5. **ArrayLists store primitives** — They store wrapper objects. Autoboxing and unboxing make this largely transparent, but be aware that `null` values can appear.
6. **Confusing `add(index, obj)` and `set(index, obj)`** — `add` inserts (shifts following elements right); `set` replaces (the position stays the same).
7. **Ambiguity of `remove()` with Integer** — `list.remove(3)` removes the element at index 3. To remove the Integer object whose value is 3, use `list.remove(Integer.valueOf(3))`.

## Code Patterns and Examples

### ArrayList Basics
```java
import java.util.ArrayList;

ArrayList<String> names = new ArrayList<String>();
names.add("Alice");     // ["Alice"]
names.add("Bob");       // ["Alice", "Bob"]
names.add("Charlie");   // ["Alice", "Bob", "Charlie"]

names.add(1, "Diana");  // ["Alice", "Diana", "Bob", "Charlie"]
String removed = names.remove(2);  // removed = "Bob"
                                   // ["Alice", "Diana", "Charlie"]
names.set(0, "Eve");    // ["Eve", "Diana", "Charlie"]
String name = names.get(1);  // "Diana"
int size = names.size(); // 3
```

### ArrayList with Autoboxing
```java
ArrayList<Integer> nums = new ArrayList<Integer>();
nums.add(42);          // autoboxing: int 42 -> Integer.valueOf(42)
int val = nums.get(0); // unboxing: Integer -> int
```

### Traversal
```java
ArrayList<String> list = new ArrayList<String>();
list.add("A"); list.add("B"); list.add("C");

// Standard for loop
for (int i = 0; i < list.size(); i++) {
    System.out.println(list.get(i));
}

// Enhanced for loop
for (String s : list) {
    System.out.println(s);
}
```

### Removing During Traversal (CRITICAL PATTERN)
```java
ArrayList<Integer> nums = new ArrayList<Integer>();
// assume nums = [1, 2, 3, 2, 4, 2]

// WRONG: Forward traversal skips elements after removal
for (int i = 0; i < nums.size(); i++) {
    if (nums.get(i) == 2) {
        nums.remove(i);  // after removing, next element shifts to i
                         // but i increments, skipping it!
    }
}

// CORRECT: Backward traversal
for (int i = nums.size() - 1; i >= 0; i--) {
    if (nums.get(i) == 2) {
        nums.remove(i);
    }
}

// CORRECT: Adjust index after removal
for (int i = 0; i < nums.size(); i++) {
    if (nums.get(i) == 2) {
        nums.remove(i);
        i--;  // counteract the i++ to recheck this index
    }
}
```

### Linear Search
```java
public static int linearSearch(ArrayList<String> list, String target) {
    for (int i = 0; i < list.size(); i++) {
        if (list.get(i).equals(target)) {
            return i;
        }
    }
    return -1;  // not found
}
```

### Selection Sort
```java
public static void selectionSort(ArrayList<Integer> list) {
    for (int i = 0; i < list.size() - 1; i++) {
        int minIndex = i;
        for (int j = i + 1; j < list.size(); j++) {
            if (list.get(j) < list.get(minIndex)) {
                minIndex = j;
            }
        }
        // Swap
        int temp = list.get(i);
        list.set(i, list.get(minIndex));
        list.set(minIndex, temp);
    }
}
```

### Insertion Sort
```java
public static void insertionSort(ArrayList<Integer> list) {
    for (int i = 1; i < list.size(); i++) {
        int key = list.get(i);
        int j = i - 1;
        while (j >= 0 && list.get(j) > key) {
            list.set(j + 1, list.get(j));
            j--;
        }
        list.set(j + 1, key);
    }
}
```

### Array to ArrayList Conversion Pattern
```java
// Array to ArrayList
String[] arr = {"A", "B", "C"};
ArrayList<String> list = new ArrayList<String>();
for (String s : arr) {
    list.add(s);
}

// ArrayList to Array (not on AP exam, but useful)
// String[] arr2 = list.toArray(new String[0]);
```
