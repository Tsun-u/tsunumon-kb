# Unit 5: Writing Classes

**Exam Weight:** 5-7.5% | **Suggested Time:** ~12-14 class periods
**2025-26 Revision:** Now Unit 3 "Class Creation" (10-18% of exam)

## Topics

### Topic 5.1: Anatomy of a Class

This section covers how to set appropriate access permissions and visibility for classes, data, constructors, and methods.

- A class contains instance variables, constructors, and methods
- `public` — accessible from anywhere
- `private` — accessible only within the same class
- Instance variables should be declared `private` (encapsulation principle)
- Methods and constructors are typically declared `public`
- Data encapsulation hides implementation details from the outside

### Topic 5.2: Constructors

This section covers how to declare and initialize instance variables through constructors.

- A constructor's name must exactly match the class name
- Constructors have no return type (not even `void`)
- They are used to initialize instance variables
- Java provides a default no-argument constructor only if no constructors are written at all
- A class can have multiple overloaded constructors
- When a constructor parameter has the same name as an instance variable, use `this.` to distinguish them

### Topic 5.3: Documentation with Comments

This section covers how to use comments to document what code does and how to use it.

- Single-line comments: `//`
- Multi-line comments: `/* ... */`
- Javadoc comments: `/** ... */`
- Precondition: a condition that must be true before a method is called
- Postcondition: a condition guaranteed to be true after a method completes
- Good comments explain "why," not "what" — the code itself should convey what is happening

### Topic 5.4: Accessor Methods

This section covers how to define object behavior using non-void methods that take no parameters.

- An accessor (getter) returns the value of an instance variable
- Naming convention: `getVariableName()`
- The return type matches the type of the instance variable
- `toString()` is a special accessor that returns a string representation of the object
- `toString()` is called automatically in print statements and string concatenation

### Topic 5.5: Mutator Methods

This section covers how to define object behavior using void methods with parameters.

- A mutator (setter) changes the value of an instance variable
- Naming convention: `setVariableName(Type value)`
- Typically has a `void` return type
- Can include validation logic to enforce constraints

### Topic 5.6: Writing Methods

This section covers how to define object behavior using methods with and without parameters that return values.

- A method signature includes: access modifier, return type, method name, parameter list
- The `return` statement ends the method and sends a value back to the caller
- Method decomposition: breaking complex work into smaller helper methods
- A method can call other methods in the same class

### Topic 5.7: Static Variables and Methods

This section covers how to define class-level behavior using static methods.

- `static` means belonging to the class itself, not to any individual object
- Static methods can be called without creating an object: `ClassName.method()`
- Static methods cannot directly access instance variables or call instance methods
- Static variables are shared across all instances of the class
- The `main` method is static

### Topic 5.8: Scope and Access

This section covers how to identify the scope of a variable.

- Instance variables: accessible throughout the entire class
- Local variables: accessible only within the method or block where they are declared
- Parameters: accessible only within their method
- When a local variable has the same name as an instance variable, the local variable shadows the instance variable
- Use `this.variableName` to access the instance variable when shadowing occurs

### Topic 5.9: this Keyword

This section covers how to use `this` to express the connection between an object and its class.

- `this` refers to the current object
- `this.variable` explicitly refers to the instance variable when a parameter shadows it
- `this(args)` calls another constructor in the same class (constructor chaining)

### Topic 5.10: Ethical and Social Implications of Computing Systems

This section covers how to describe the ethical and social effects of computing systems.

- Considerations around system reliability and security
- Privacy concerns raised by data collection
- Intellectual property rights and software licensing
- Both positive and negative effects of computing technology on society

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Encapsulation | Bundling data with the methods that operate on it while hiding internal details from outside code |
| Access modifier | A keyword that controls visibility (`public`, `private`) |
| Instance variable | A variable declared inside a class but outside any method |
| Local variable | A variable declared inside a method |
| Constructor | A method that initializes a new object's state when it is created |
| Accessor (getter) | A method that returns the value of a private instance variable |
| Mutator (setter) | A method that modifies the value of a private instance variable |
| Static | Belongs to the class rather than to any individual instance |
| Scope | The region of a program where a variable can be accessed |
| `this` keyword | A reference to the current object |
| Precondition | A condition that must be true before a method is called |
| Postcondition | A condition guaranteed to hold after a method finishes |

## Common Misconceptions

1. **The default constructor always exists** — Java only provides the default no-argument constructor when you write no constructors at all. Once you define any constructor, the default disappears.
2. **Constructors need `void`** — Constructors have no return type. Adding `void` turns it into a regular method, not a constructor.
3. **Static methods can access instance variables** — Static methods cannot directly access instance variables or call instance methods; they must do so through an object reference.
4. **Using `this` in a static context** — `this` cannot be used inside a static method because there is no "current object."
5. **Forgetting `this.`** — When a parameter and an instance variable share the same name, writing `variable = variable` assigns the parameter back to itself and has no effect. You must write `this.variable = variable`.
6. **void methods cannot use return** — Void methods cannot return a value, but they can use `return;` (with no value) to exit early.
7. **Making instance variables public** — This is syntactically valid but breaks encapsulation. Instance variables should always be `private`, with public getters and setters provided as needed.

## Code Patterns and Examples

### Complete Class Example
```java
public class Student {
    // Instance variables (private for encapsulation)
    private String name;
    private int age;
    private double gpa;
    private static int studentCount = 0;  // shared across all instances

    // Constructor
    public Student(String name, int age, double gpa) {
        this.name = name;
        this.age = age;
        this.gpa = gpa;
        studentCount++;
    }

    // No-arg constructor (overloaded)
    public Student() {
        this("Unknown", 0, 0.0);  // constructor chaining
    }

    // Accessor methods (getters)
    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public double getGpa() {
        return gpa;
    }

    // Mutator methods (setters)
    public void setName(String name) {
        this.name = name;
    }

    public void setGpa(double gpa) {
        if (gpa >= 0.0 && gpa <= 4.0) {  // validation
            this.gpa = gpa;
        }
    }

    // Non-void method
    public boolean isHonorsStudent() {
        return gpa >= 3.5;
    }

    // Static method
    public static int getStudentCount() {
        return studentCount;
    }

    // toString
    public String toString() {
        return name + " (age " + age + ", GPA: " + gpa + ")";
    }
}
```

### Using the Class
```java
Student s1 = new Student("Alice", 17, 3.8);
Student s2 = new Student("Bob", 16, 3.2);

System.out.println(s1.getName());       // "Alice"
System.out.println(s1.isHonorsStudent()); // true
System.out.println(s2.isHonorsStudent()); // false

s2.setGpa(3.6);
System.out.println(s2);  // toString() called automatically
// Output: "Bob (age 16, GPA: 3.6)"

System.out.println(Student.getStudentCount()); // 2 (static method)
```

### Scope Example
```java
public class Example {
    private int value = 10;  // instance variable

    public void method(int value) {   // parameter shadows instance variable
        int result = value * 2;       // uses parameter, not instance variable
        int total = this.value + value; // this.value = 10, value = parameter
        System.out.println(result);
        System.out.println(total);
    }
}
```
