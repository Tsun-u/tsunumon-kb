# Unit 2: Using Objects

**Exam Weight:** 5-7.5% | **Suggested Time:** ~13-15 class periods
**2025-26 Revision:** Merged into new Unit 1 "Using Objects and Methods"

## Topics

### Topic 2.1: Objects - Instances of Classes

This section covers the relationship between classes and objects.

- A class is a blueprint or template; an object is a specific instance of that class
- Objects have both attributes (state) and behaviors (methods)
- Multiple objects can be created from the same class
- Each object maintains its own independent state (its own instance variable values)

### Topic 2.2: Creating and Storing Objects (Instantiation)

This section covers how to identify constructors and use them to create objects.

- The `new` keyword is required to create an object
- A constructor initializes the state of a newly created object
- A constructor's name must match the class name exactly
- Constructors have no return type (not even `void`)
- A class can define multiple constructors (method overloading)
- `null` is a special value meaning "no object is referenced"

### Topic 2.3: Calling a Void Method

This section covers how to call non-static void methods that take no parameters.

- A void method performs an action but does not return a value
- Called using dot notation: `object.method()`
- Methods define the behaviors that an object can perform

### Topic 2.4: Calling a Void Method with Parameters

This section covers how to call non-static void methods that accept parameters.

- A parameter is a variable declared in the method definition
- An argument is the actual value passed when the method is called
- The number, order, and type of arguments must match the parameters
- Overloaded methods share the same name but have different parameter lists

### Topic 2.5: Calling a Non-void Method

This section covers how to evaluate expressions that involve non-void method calls.

- A non-void method returns a value to the caller
- The returned value can be stored in a variable or used directly in an expression
- The return type is explicitly declared in the method signature

### Topic 2.6: String Objects: Concatenation, Literals, and More

This section covers how to evaluate expressions involving string concatenation.

- Strings are immutable — once created, their content cannot be changed
- The `+` operator concatenates strings
- When either operand of `+` is a String, the other side is automatically converted to a String
- Concatenation evaluates left to right
- Escape sequences: `\"`, `\\`, `\n`

### Topic 2.7: String Methods

This section covers how to call String methods.

- `int length()` — returns the number of characters in the string
- `String substring(int from, int to)` — returns characters from index `from` up to but not including index `to`
- `String substring(int from)` — returns characters from index `from` to the end
- `int indexOf(String str)` — returns the index of the first occurrence of str, or -1 if not found
- `boolean equals(String other)` — compares string content (case-sensitive)
- `int compareTo(String other)` — compares strings in lexicographic order
- String indices start at 0
- An invalid index throws `StringIndexOutOfBoundsException`

### Topic 2.8: Wrapper Classes: Integer and Double

This section covers how to use wrapper class objects.

- `Integer` wraps `int`; `Double` wraps `double`
- Autoboxing: a primitive is automatically converted to its wrapper object
- Unboxing: a wrapper object is automatically converted back to a primitive
- `Integer.MIN_VALUE` and `Integer.MAX_VALUE` are predefined constants
- Wrapper class objects are immutable

### Topic 2.9: Using the Math Class

This section covers how to call static methods.

- `Math` methods are all static (called on the class, no object needed)
- `int Math.abs(int x)` — absolute value of an integer
- `double Math.abs(double x)` — absolute value of a double
- `double Math.pow(double base, double exp)` — raises base to the power exp
- `double Math.sqrt(double x)` — square root
- `double Math.random()` — returns a random value in the range [0.0, 1.0)
- To generate a random integer in the range [a, b] inclusive: `(int)(Math.random() * (b - a + 1)) + a`

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Object | An instance of a class that has state and behavior |
| Class | A blueprint used to create objects |
| Constructor | A special method that initializes a new object's state when it is created |
| Instantiation | The act of creating a new object using `new` |
| Method | A named block of code that performs a specific task |
| Parameter | A variable declared in a method signature |
| Argument | The actual value passed to a method when it is called |
| Return type | The data type of the value a method sends back to the caller |
| void | Indicates that a method does not return a value |
| static | Belongs to the class itself rather than to any individual object |
| Overloading | Defining multiple methods with the same name but different parameter lists in the same class |
| null | A reference that does not point to any object |
| Immutable | Cannot be changed after it is created |
| Autoboxing | Automatic conversion of a primitive to its corresponding wrapper object |
| Unboxing | Automatic conversion of a wrapper object back to its primitive type |

## Common Misconceptions

1. **Comparing strings with `==`** — This compares references (memory addresses), not content. Use `.equals()` to compare string content.
2. **`substring(a, b)` includes index b** — It does not. The returned substring runs from `a` to `b-1`; index `b` is excluded.
3. **String indices start at 1** — They do not. Like arrays, string indices start at 0.
4. **`Math.random()` can return 1.0** — It cannot. The range is [0.0, 1.0), which includes 0 but excludes 1.
5. **Calling a method on `null`** — This throws a `NullPointerException` at runtime.
6. **Strings can be modified** — They cannot. String methods return new String objects; the original is unchanged.
7. **`new` is optional** — Most objects require `new` to be created. String literals are the notable exception (e.g., `String s = "hello"`).

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
