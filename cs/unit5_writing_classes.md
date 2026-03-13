# Unit 5: Writing Classes

**Exam Weight:** 5-7.5% | **Suggested Time:** ~12-14 class periods
**2025-26 Revision:** Now Unit 3 "Class Creation" (10-18% of exam)

## Topics

### Topic 5.1: Anatomy of a Class
- **Learning Objective (MOD-2.A):** Designate access and visibility constraints to classes, data, constructors, and methods
- **Essential Knowledge:**
  - A class contains instance variables, constructors, and methods
  - `public` - accessible from anywhere
  - `private` - accessible only within the class
  - Instance variables should be `private` (encapsulation)
  - Methods and constructors are typically `public`
  - Data encapsulation: hiding implementation details

### Topic 5.2: Constructors
- **Learning Objective (MOD-2.B):** Define instance variables for the attributes to be initialized through constructors
- **Essential Knowledge:**
  - Constructors have the same name as the class
  - No return type (not even `void`)
  - Used to initialize instance variables
  - Default no-argument constructor is provided only if NO constructor is written
  - A class can have multiple overloaded constructors
  - Constructor parameters often have the same names as instance variables (use `this.`)

### Topic 5.3: Documentation with Comments
- **Learning Objective (MOD-2.C):** Describe the functionality and use of program code through comments
- **Essential Knowledge:**
  - Single-line comments: `//`
  - Multi-line comments: `/* ... */`
  - Javadoc comments: `/** ... */`
  - Preconditions: what must be true before a method is called
  - Postconditions: what is true after a method executes
  - Comments explain WHY, not WHAT (code should be self-documenting)

### Topic 5.4: Accessor Methods
- **Learning Objective (VAR-2.F):** Define behaviors of an object through non-void methods without parameters
- **Essential Knowledge:**
  - Accessor methods (getters) return the value of an instance variable
  - Naming convention: `getVariableName()`
  - Return type matches the instance variable type
  - `toString()` is a special accessor that returns a String representation
  - `toString()` is automatically called in print statements and concatenation

### Topic 5.5: Mutator Methods
- **Learning Objective (VAR-2.G):** Define behaviors of an object through void methods with parameters
- **Essential Knowledge:**
  - Mutator methods (setters) change the value of an instance variable
  - Naming convention: `setVariableName(Type value)`
  - Typically `void` return type
  - Can include validation logic

### Topic 5.6: Writing Methods
- **Learning Objective (MOD-2.D):** Define behaviors of an object through non-void methods with or without parameters
- **Essential Knowledge:**
  - Method signature: access modifier, return type, name, parameters
  - `return` statement exits the method and provides the return value
  - Method decomposition: breaking complex tasks into smaller methods
  - A method can call other methods in the same class

### Topic 5.7: Static Variables and Methods
- **Learning Objective (VAR-2.H):** Define behaviors of a class through static methods
- **Essential Knowledge:**
  - `static` belongs to the class, not to individual objects
  - Static methods can be called without creating an object: `ClassName.method()`
  - Static methods cannot access instance variables or call instance methods directly
  - Static variables are shared across all instances of a class
  - `main` method is static

### Topic 5.8: Scope and Access
- **Learning Objective (VAR-2.I):** Identify the scope of a variable
- **Essential Knowledge:**
  - Instance variables: accessible throughout the class
  - Local variables: accessible only within the method/block where declared
  - Parameters: accessible only within the method
  - If a local variable has the same name as an instance variable, the local variable takes precedence (shadowing)
  - Use `this.variableName` to access the instance variable when shadowed

### Topic 5.9: this Keyword
- **Learning Objective (VAR-2.J):** Represent the connection between an object and its class using `this`
- **Essential Knowledge:**
  - `this` refers to the current object
  - `this.variable` accesses instance variable when shadowed by parameter
  - `this(args)` calls another constructor in the same class (constructor chaining)

### Topic 5.10: Ethical and Social Implications of Computing Systems
- **Learning Objective (IOC-1.A):** Explain the ethical and social implications of computing systems
- **Essential Knowledge:**
  - System reliability and security considerations
  - Privacy concerns with data collection
  - Intellectual property and software licensing
  - Beneficial and harmful effects of computing

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Encapsulation | Bundling data with methods that operate on it; hiding internal details |
| Access modifier | Keywords controlling visibility (`public`, `private`) |
| Instance variable | A variable declared in a class but outside methods |
| Local variable | A variable declared inside a method |
| Constructor | Initializes a new object's state |
| Accessor (getter) | Returns the value of a private instance variable |
| Mutator (setter) | Changes the value of a private instance variable |
| Static | Belongs to the class rather than instances |
| Scope | The region of code where a variable is accessible |
| `this` keyword | Reference to the current object |
| Precondition | What must be true before a method is called |
| Postcondition | What is true after a method completes |

## Common Misconceptions

1. **Default constructor always exists** - Java provides a default no-arg constructor ONLY if you write NO constructors at all. Once you write any constructor, the default disappears.
2. **`void` on constructors** - Constructors do NOT have a return type. Adding `void` makes it a regular method, not a constructor.
3. **Static methods accessing instance variables** - Static methods CANNOT access instance variables or call instance methods without an object reference.
4. **`this` in static context** - `this` cannot be used in static methods because there is no "current object."
5. **Forgetting `this.`** - When a parameter shadows an instance variable, `variable = variable` does nothing useful. Use `this.variable = variable`.
6. **Returning from void methods** - Void methods don't return a value, but `return;` (no value) can be used to exit early.
7. **Public instance variables** - While syntactically valid, this violates encapsulation. Always use `private` instance variables with public getters/setters.

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
