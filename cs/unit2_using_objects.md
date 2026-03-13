# Unit 2: Using Objects

**Exam Weight:** 5-7.5% | **Suggested Time:** ~13-15 class periods
**2025-26 Revision:** Merged into new Unit 1 "Using Objects and Methods"

## Topics

### Topic 2.1: Objects - Instances of Classes
- **Learning Objective (MOD-1.B):** Explain the relationship between a class and an object
- **Essential Knowledge:**
  - A class is a blueprint/template; an object is an instance of a class
  - Objects have attributes (state) and behaviors (methods)
  - Multiple objects can be created from the same class
  - Each object has its own state (instance variable values)

### Topic 2.2: Creating and Storing Objects (Instantiation)
- **Learning Objective (MOD-1.C):** Identify a class constructor
- **Learning Objective (MOD-1.D):** Call a class constructor to create an object
- **Essential Knowledge:**
  - Objects are created using the `new` keyword
  - Constructors initialize an object's state
  - Constructor name matches the class name
  - Constructors do NOT have a return type
  - A class can have multiple constructors (overloading)
  - `null` is a special value meaning "no object reference"

### Topic 2.3: Calling a Void Method
- **Learning Objective (VAR-2.A):** Call non-static void methods without parameters
- **Essential Knowledge:**
  - Void methods perform an action but do not return a value
  - Called using dot notation: `object.method()`
  - Methods define the behavior of an object

### Topic 2.4: Calling a Void Method with Parameters
- **Learning Objective (VAR-2.B):** Call non-static void methods with parameters
- **Essential Knowledge:**
  - Parameters are values passed to a method
  - Arguments are the actual values provided when calling
  - Parameters must match in number, order, and compatible types
  - Overloaded methods have the same name but different parameter lists

### Topic 2.5: Calling a Non-void Method
- **Learning Objective (VAR-2.C):** Evaluate expressions that use non-void methods
- **Essential Knowledge:**
  - Non-void methods return a value
  - The return value can be stored in a variable or used in an expression
  - Return type is specified in the method signature

### Topic 2.6: String Objects: Concatenation, Literals, and More
- **Learning Objective (VAR-1.H):** Evaluate expressions involving String concatenation
- **Essential Knowledge:**
  - Strings are immutable (cannot be changed once created)
  - `+` concatenates Strings
  - If either operand of `+` is a String, the other is converted to String
  - Concatenation is evaluated left to right
  - Escape sequences: `\"`, `\\`, `\n`

### Topic 2.7: String Methods
- **Learning Objective (VAR-2.D):** Call String methods
- **Essential Knowledge:**
  - `int length()` - returns number of characters
  - `String substring(int from, int to)` - returns substring from index `from` to `to-1`
  - `String substring(int from)` - returns substring from index to end
  - `int indexOf(String str)` - returns first index of str, or -1 if not found
  - `boolean equals(String other)` - compares content (case-sensitive)
  - `int compareTo(String other)` - lexicographic comparison
  - String indices start at 0
  - `StringIndexOutOfBoundsException` if index is invalid

### Topic 2.8: Wrapper Classes: Integer and Double
- **Learning Objective (VAR-1.I):** Use wrapper class objects
- **Essential Knowledge:**
  - `Integer` wraps `int`; `Double` wraps `double`
  - Autoboxing: automatic conversion from primitive to wrapper
  - Unboxing: automatic conversion from wrapper to primitive
  - `Integer.MIN_VALUE` and `Integer.MAX_VALUE` constants
  - Wrapper objects are immutable

### Topic 2.9: Using the Math Class
- **Learning Objective (VAR-2.E):** Call static methods
- **Essential Knowledge:**
  - `Math` methods are static (called on the class, not an object)
  - `int Math.abs(int x)` - absolute value
  - `double Math.abs(double x)` - absolute value
  - `double Math.pow(double base, double exp)` - power
  - `double Math.sqrt(double x)` - square root
  - `double Math.random()` - returns [0.0, 1.0)
  - Random int in range [a, b]: `(int)(Math.random() * (b - a + 1)) + a`

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Object | An instance of a class with state and behavior |
| Class | A blueprint for creating objects |
| Constructor | A special method that initializes an object |
| Instantiation | Creating a new object using `new` |
| Method | A named block of code that performs a task |
| Parameter | A variable declared in a method signature |
| Argument | An actual value passed to a method |
| Return type | The data type of the value a method returns |
| void | Indicates a method returns nothing |
| static | Belongs to the class, not to individual objects |
| Overloading | Multiple methods with the same name but different parameters |
| null | A reference that points to no object |
| Immutable | Cannot be changed after creation |
| Autoboxing | Automatic primitive-to-wrapper conversion |
| Unboxing | Automatic wrapper-to-primitive conversion |

## Common Misconceptions

1. **Comparing Strings with `==`** - This compares references, not content! Use `.equals()` for content comparison.
2. **`substring(a, b)` includes index `b`** - No! It includes `a` up to but NOT including `b`.
3. **String indices start at 1** - No! They start at 0, like arrays.
4. **`Math.random()` can return 1.0** - No! It returns values in [0.0, 1.0) - inclusive of 0, exclusive of 1.
5. **Calling methods on `null`** - Causes `NullPointerException` at runtime.
6. **Strings are mutable** - No! String methods return NEW strings; the original is unchanged.
7. **`new` is optional** - For most objects, `new` is required. String literals are an exception (e.g., `String s = "hello"`).

## Code Patterns and Examples

### Creating Objects
```java
// Constructor calls
String greeting = new String("Hello");
String greeting2 = "Hello";  // String literal shorthand

// Scanner for input
Scanner input = new Scanner(System.in);
```

### String Methods
```java
String str = "Hello World";
int len = str.length();           // 11
String sub = str.substring(0, 5); // "Hello"
String sub2 = str.substring(6);   // "World"
int idx = str.indexOf("World");   // 6
int idx2 = str.indexOf("xyz");    // -1
boolean eq = str.equals("Hello World");  // true
int cmp = "apple".compareTo("banana");   // negative (a < b)
```

### String Concatenation
```java
String name = "Alice";
int age = 20;
String msg = name + " is " + age;  // "Alice is 20"

// Left-to-right evaluation matters:
System.out.println(1 + 2 + " sum");     // "3 sum"
System.out.println("sum " + 1 + 2);     // "sum 12"
System.out.println("sum " + (1 + 2));   // "sum 3"
```

### Math Class
```java
int absVal = Math.abs(-5);        // 5
double power = Math.pow(2, 10);   // 1024.0
double root = Math.sqrt(144);     // 12.0

// Random integer from 1 to 6 (inclusive)
int die = (int)(Math.random() * 6) + 1;

// Random integer from min to max (inclusive)
int rand = (int)(Math.random() * (max - min + 1)) + min;
```

### Wrapper Classes
```java
Integer intObj = 42;           // autoboxing
int val = intObj;              // unboxing
int maxInt = Integer.MAX_VALUE; // 2147483647
int minInt = Integer.MIN_VALUE; // -2147483648
```
