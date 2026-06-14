# Unit 9: Inheritance

**Exam Weight (pre-2025):** 5-10% | **Suggested Time:** ~10-12 class periods
**2025-26 Revision:** REMOVED from required content. Inheritance and polymorphism are no longer tested on the AP exam starting 2025-26. This file documents the original framework for reference.

## Topics

### Topic 9.1: Creating Superclasses and Subclasses

This section covers how to establish an inheritance relationship from a subclass to a superclass.

- The `extends` keyword creates an inheritance relationship
- A subclass inherits all public methods and variables from the superclass
- Subclasses do not inherit constructors
- A subclass cannot directly access `private` members of the superclass
- Java supports only single inheritance (a class can extend at most one other class)
- "is-a" relationship: a subclass is a specialized version of the superclass

### Topic 9.2: Writing Constructors for Subclasses

This section covers how to establish an inheritance relationship through constructor design.

- `super(args)` calls the superclass constructor
- `super()` must be the first statement in a subclass constructor
- If `super()` is not written explicitly, Java inserts a no-argument `super()` automatically
- If the superclass has no no-argument constructor, the subclass must explicitly call `super(args)`

### Topic 9.3: Overriding Methods

This section covers how to define overriding methods in a subclass.

- Overriding: the subclass provides its own version of a method inherited from the superclass
- The method signature must be identical (name, parameters, return type)
- Adding `@Override` is recommended (helps the compiler catch errors)
- Overriding vs. overloading: overriding replaces a method; overloading adds a new version with different parameters
- `super.method()` calls the superclass version of the overridden method

### Topic 9.4: super Keyword

This section covers how to call superclass methods from within a subclass.

- `super.method()` invokes the superclass version of a method
- `super(args)` calls the superclass constructor
- Chaining is not allowed: `super.super.method()` is illegal in Java

### Topic 9.5: Creating References Using Inheritance Hierarchies

This section covers how to declare reference variables of a superclass type.

- A superclass reference can point to a subclass object: `Animal a = new Dog();`
- The reference type determines which methods can be called
- The actual object type determines which version of the method runs (polymorphism)
- Calling subclass-specific methods through a superclass reference requires a cast

### Topic 9.6: Polymorphism

This section covers how to use polymorphism to call methods across an inheritance hierarchy.

- Polymorphism: the same method call produces different behavior depending on the object's actual type
- Determined at runtime (dynamic dispatch), not at compile time
- Allows you to write general code that works with any subclass
- Method calls are resolved based on the actual object type, not the declared reference type

### Topic 9.7: Object Superclass

This section covers the effects of methods defined in the `Object` class.

- Every class implicitly extends `Object`
- Key `Object` methods: `toString()`, `equals(Object obj)`
- The default `toString()` returns the class name plus a hash code (rarely meaningful)
- The default `equals()` uses `==` (compares references)
- Classes should override `toString()` and `equals()` to provide meaningful behavior

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Inheritance | The mechanism by which one class acquires the attributes and behaviors of another |
| Superclass (parent) | The class being inherited from |
| Subclass (child) | The class that performs the inheritance |
| `extends` | The keyword used to create an inheritance relationship |
| `super` | A reference to the superclass |
| Overriding | Replacing an inherited method in a subclass with a new implementation |
| Overloading | Defining multiple methods with the same name but different parameters (not restricted to inheritance) |
| Polymorphism | The same method call producing different behavior depending on the object's type |
| Dynamic dispatch | Deciding at runtime which version of a method to execute |
| "is-a" relationship | A subclass is a specialized kind of the superclass |
| `Object` class | The root of the entire Java class hierarchy |

## Common Misconceptions

1. **Subclasses inherit constructors** — They do not. Constructors are not inherited. A subclass must define its own constructors and call `super()` explicitly.
2. **`super()` can appear anywhere** — It cannot. `super()` must be the first statement in a constructor.
3. **Overriding and overloading are the same** — Overriding replaces a method (same signature); overloading adds a method (different parameters).
4. **Private members are inherited** — Private members exist in subclass objects but cannot be accessed directly. Use public getters and setters provided by the superclass.
5. **Polymorphism is resolved at compile time** — The version of the method that actually runs is determined at runtime based on the object's true type.
6. **A superclass reference can call subclass-specific methods** — Only methods defined (or overridden) in the superclass can be called through a superclass reference.
7. **Java supports multiple inheritance** — It does not. A class can extend only one other class.

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
