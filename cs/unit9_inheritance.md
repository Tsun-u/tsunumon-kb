# Unit 9: Inheritance

**Exam Weight (pre-2025):** 5-10% | **Suggested Time:** ~10-12 class periods
**2025-26 Revision:** REMOVED from required content. Inheritance and polymorphism are no longer tested on the AP exam starting 2025-26. This file documents the original framework for reference.

## Topics

### Topic 9.1: Creating Superclasses and Subclasses
- **Learning Objective (MOD-3.A):** Create an inheritance relationship from a subclass to a superclass
- **Essential Knowledge:**
  - `extends` keyword creates an inheritance relationship
  - Subclass inherits all public methods and variables from superclass
  - Subclass does NOT inherit constructors
  - Subclass does NOT have direct access to `private` members of superclass
  - Java supports single inheritance only (one superclass)
  - "is-a" relationship: a subclass IS-A type of superclass

### Topic 9.2: Writing Constructors for Subclasses
- **Learning Objective (MOD-3.B):** Create an inheritance relationship by writing a constructor
- **Essential Knowledge:**
  - `super(args)` calls the superclass constructor
  - `super()` must be the FIRST statement in the subclass constructor
  - If `super()` is not explicitly called, Java inserts `super()` (no-arg) automatically
  - If superclass has no no-arg constructor, subclass MUST explicitly call `super(args)`

### Topic 9.3: Overriding Methods
- **Learning Objective (MOD-3.C):** Define overriding methods in a subclass
- **Essential Knowledge:**
  - Overriding: subclass provides its own version of an inherited method
  - Method signature must be identical (name, parameters, return type)
  - `@Override` annotation is recommended (catches errors)
  - Overriding vs. overloading: overriding replaces; overloading adds new version with different parameters
  - `super.method()` calls the superclass version of an overridden method

### Topic 9.4: super Keyword
- **Learning Objective (MOD-3.D):** Call methods in a superclass from a subclass
- **Essential Knowledge:**
  - `super.method()` calls the superclass version of a method
  - `super(args)` calls the superclass constructor
  - Cannot chain super: `super.super.method()` is NOT allowed

### Topic 9.5: Creating References Using Inheritance Hierarchies
- **Learning Objective (MOD-3.E):** Define reference variables of a superclass type
- **Essential Knowledge:**
  - A superclass reference can hold a subclass object: `Animal a = new Dog();`
  - The reference type determines which methods can be CALLED
  - The object type determines which version of the method RUNS (polymorphism)
  - Cannot call subclass-only methods through a superclass reference (without casting)

### Topic 9.6: Polymorphism
- **Learning Objective (MOD-3.F):** Call methods in an inheritance hierarchy using polymorphism
- **Essential Knowledge:**
  - Polymorphism: same method call produces different behavior depending on object type
  - Determined at RUNTIME (dynamic dispatch), not compile time
  - Enables writing general code that works with any subclass
  - Method calls are resolved based on the ACTUAL object type, not the reference type

### Topic 9.7: Object Superclass
- **Learning Objective (MOD-3.G):** Explain the effect of methods defined in `Object`
- **Essential Knowledge:**
  - All classes implicitly extend `Object`
  - Key `Object` methods: `toString()`, `equals(Object obj)`
  - Default `toString()` returns class name + hash code (not useful)
  - Default `equals()` uses `==` (reference comparison)
  - Classes should override `toString()` and `equals()` for meaningful behavior

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Inheritance | A class deriving attributes and behaviors from another class |
| Superclass (parent) | The class being inherited from |
| Subclass (child) | The class that inherits |
| `extends` | Keyword to create inheritance relationship |
| `super` | Reference to the superclass |
| Overriding | Replacing an inherited method with a new implementation |
| Overloading | Same method name, different parameters (not inheritance-specific) |
| Polymorphism | Same method call, different behavior based on object type |
| Dynamic dispatch | Runtime determination of which method to execute |
| "is-a" relationship | Subclass is a specialized type of superclass |
| `Object` class | The root of all class hierarchies in Java |

## Common Misconceptions

1. **Subclasses inherit constructors** - No! Constructors are NOT inherited. Subclasses must define their own and call `super()`.
2. **`super()` can be called anywhere** - No! `super()` must be the FIRST statement in a constructor.
3. **Overriding = Overloading** - Overriding replaces a method (same signature). Overloading creates a new method (different parameters).
4. **Private members are inherited** - Private members exist in the subclass object but cannot be accessed directly. Use public getters/setters.
5. **Polymorphism is compile-time** - The method version that runs is determined at RUNTIME based on the actual object type.
6. **Superclass reference can call subclass methods** - Only methods defined in the superclass (or overridden) can be called through a superclass reference.
7. **Multiple inheritance** - Java does NOT support extending multiple classes. A class can only extend ONE superclass.

## Code Patterns and Examples

### Basic Inheritance
```java
// Superclass
public class Animal {
    private String name;

    public Animal(String name) {
        this.name = name;
    }

    public String getName() {
        return name;
    }

    public String speak() {
        return "...";
    }

    public String toString() {
        return name + " says " + speak();
    }
}

// Subclass
public class Dog extends Animal {
    private String breed;

    public Dog(String name, String breed) {
        super(name);          // MUST be first statement
        this.breed = breed;
    }

    @Override
    public String speak() {
        return "Woof!";
    }

    public String getBreed() {
        return breed;
    }
}

// Another subclass
public class Cat extends Animal {
    public Cat(String name) {
        super(name);
    }

    @Override
    public String speak() {
        return "Meow!";
    }
}
```

### Polymorphism
```java
// Superclass reference, subclass object
Animal a1 = new Dog("Rex", "Labrador");
Animal a2 = new Cat("Whiskers");
Animal a3 = new Animal("Generic");

System.out.println(a1.speak());  // "Woof!" (Dog's version)
System.out.println(a2.speak());  // "Meow!" (Cat's version)
System.out.println(a3.speak());  // "..." (Animal's version)

// Polymorphism with arrays
Animal[] animals = {a1, a2, a3};
for (Animal a : animals) {
    System.out.println(a.toString());  // each calls its own speak()
}
// Output:
// Rex says Woof!
// Whiskers says Meow!
// Generic says ...

// Cannot call subclass-specific methods through superclass reference:
// a1.getBreed();  // COMPILE ERROR! Animal has no getBreed()
// Must cast: ((Dog) a1).getBreed();  // "Labrador"
```

### Constructor Chaining
```java
public class Vehicle {
    private int year;
    private String make;

    public Vehicle(int year, String make) {
        this.year = year;
        this.make = make;
    }
}

public class Car extends Vehicle {
    private int numDoors;

    public Car(int year, String make, int numDoors) {
        super(year, make);     // calls Vehicle constructor
        this.numDoors = numDoors;
    }

    public Car(int year, String make) {
        this(year, make, 4);   // calls Car's 3-arg constructor
    }
}
```

### Overriding equals() and toString()
```java
public class Point {
    private int x, y;

    public Point(int x, int y) {
        this.x = x;
        this.y = y;
    }

    @Override
    public boolean equals(Object obj) {
        if (obj instanceof Point) {
            Point other = (Point) obj;
            return this.x == other.x && this.y == other.y;
        }
        return false;
    }

    @Override
    public String toString() {
        return "(" + x + ", " + y + ")";
    }
}
```
