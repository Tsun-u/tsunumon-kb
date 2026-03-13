# Unit 7: ArrayList

**Exam Weight:** 2.5-7.5% | **Suggested Time:** ~8-10 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 7.1: Introduction to ArrayList
- **Learning Objective (VAR-2.L):** Represent collections of related object reference data using ArrayList objects
- **Essential Knowledge:**
  - `ArrayList` is a resizable array (grows and shrinks dynamically)
  - Must import: `import java.util.ArrayList;`
  - Stores object references only (not primitives directly)
  - Uses generics: `ArrayList<Type>`
  - `ArrayList<Integer>` not `ArrayList<int>` (wrapper classes required)
  - Default initial capacity, but size starts at 0

### Topic 7.2: ArrayList Methods
- **Learning Objective (VAR-2.M):** Call ArrayList methods
- **Essential Knowledge:**
  - `int size()` - returns number of elements
  - `boolean add(E obj)` - appends to end, returns `true`
  - `void add(int index, E obj)` - inserts at index, shifts elements right
  - `E get(int index)` - returns element at index
  - `E set(int index, E obj)` - replaces element, returns old element
  - `E remove(int index)` - removes and returns element, shifts elements left
  - `IndexOutOfBoundsException` for invalid indices
  - Indices range from 0 to `size() - 1`

### Topic 7.3: Traversing ArrayLists
- **Learning Objective (CON-2.I):** Traverse elements in an ArrayList
- **Essential Knowledge:**
  - Standard for loop: `for (int i = 0; i < list.size(); i++)`
  - Enhanced for loop: `for (Type item : list)`
  - Use `list.size()` not `list.length`
  - When removing during traversal, traverse backwards or adjust index
  - `ConcurrentModificationException` if modifying during enhanced for loop

### Topic 7.4: Developing Algorithms Using ArrayLists
- **Learning Objective (CON-2.J):** Develop algorithms using ArrayLists
- **Essential Knowledge:**
  - Same standard algorithms as arrays (min, max, sum, search)
  - Insert while maintaining order
  - Remove duplicates
  - Simultaneously traverse and modify (with care)
  - ArrayList can grow/shrink, enabling algorithms not possible with arrays

### Topic 7.5: Searching
- **Learning Objective (CON-2.K):** Apply sequential/linear search algorithms
- **Essential Knowledge:**
  - Linear search: check each element sequentially
  - Can search arrays or ArrayLists
  - Returns index if found, -1 if not found
  - O(n) time complexity (informal understanding)

### Topic 7.6: Sorting
- **Learning Objective (CON-2.L):** Apply selection sort and insertion sort algorithms
- **Essential Knowledge:**
  - **Selection sort:** Find the minimum, swap to front, repeat for remaining
  - **Insertion sort:** Take next element, insert into correct position in sorted portion
  - Both are O(n^2) in worst case
  - Students should trace through sorting algorithms
  - Students are NOT required to write sorting code from scratch on the exam, but must understand and trace them

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| ArrayList | A resizable ordered collection of object references |
| Generics | Type parameter in angle brackets, e.g., `<String>` |
| Wrapper class | Object version of a primitive (`Integer`, `Double`, `Boolean`) |
| Autoboxing | Automatic primitive-to-wrapper conversion |
| Unboxing | Automatic wrapper-to-primitive conversion |
| Linear search | Sequentially checking each element |
| Selection sort | Repeatedly finding the minimum and placing it in order |
| Insertion sort | Building a sorted portion by inserting elements one at a time |
| Size | Current number of elements in an ArrayList |

## Common Misconceptions

1. **`ArrayList<int>`** - WRONG! Must use wrapper class: `ArrayList<Integer>`. Primitives cannot be used as type parameters.
2. **`list.length`** - WRONG! ArrayLists use `list.size()` (with parentheses). Arrays use `.length` (no parentheses).
3. **Removing during forward traversal** - Skips elements! When you remove index `i`, the next element shifts to index `i`. Either traverse backwards or decrement `i` after removal.
4. **Modifying during enhanced for loop** - Adding or removing elements during an enhanced for loop causes `ConcurrentModificationException`.
5. **ArrayList stores primitives** - It stores wrapper objects. Autoboxing/unboxing makes it seem transparent, but be aware of `null` values.
6. **Confusing `add(index, obj)` with `set(index, obj)`** - `add` inserts (shifts elements); `set` replaces (no shifting).
7. **`remove()` with Integer** - `list.remove(3)` removes at INDEX 3. To remove the Integer VALUE 3, use `list.remove(Integer.valueOf(3))`.

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
