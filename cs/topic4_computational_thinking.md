# Topic 4: Computational Thinking, Problem-Solving and Programming

> SL + HL | Core Topic (largest topic)

## Key Concepts

### 4.1 General Principles of Computational Thinking

- **Abstraction**: focusing on essential features, hiding unnecessary detail
- **Decomposition**: breaking a complex problem into smaller, manageable parts
- **Pattern recognition**: identifying similarities or trends in data/problems
- **Algorithmic thinking**: developing step-by-step solutions

### 4.2 Algorithm Design

#### Pseudocode and Flowcharts
- IB pseudocode conventions for algorithm expression
- Flowchart symbols: process, decision, input/output, start/end, flow lines
- Trace tables for algorithm tracing

#### Standard Algorithms
- **Linear search**: check each element sequentially; O(n)
- **Binary search**: divide sorted array in half repeatedly; O(log n)
- **Bubble sort**: repeatedly swap adjacent elements; O(n²)
- **Selection sort**: find minimum, swap to front; O(n²)
- **Insertion sort**: insert each element into correct position; O(n²)

#### Algorithm Efficiency
- **Big-O notation** (informal understanding):
  - O(1): constant time
  - O(log n): logarithmic
  - O(n): linear
  - O(n²): quadratic
  - O(2ⁿ): exponential

### 4.3 Programming Fundamentals

#### Variables and Data Types
- Integer, real/float, string, Boolean, char
- Variable declaration, assignment, scope
- Constants

#### Control Structures
- **Sequence**: instructions executed in order
- **Selection**: if-else, switch/case
- **Iteration**: for loops, while loops, do-while loops
- Nested control structures

#### Arrays and Collections
- **Arrays**: fixed-size, ordered collections of same data type
- One-dimensional and two-dimensional arrays
- Array operations: traversal, search, insert, delete
- **Collections**: dynamic-size (lists, ArrayLists)

#### Strings
- String operations: concatenation, length, substring, comparison
- Character-level access and manipulation

### 4.4 Object-Oriented Programming (OOP)

- **Classes and objects**: class as blueprint, object as instance
- **Encapsulation**: bundling data and methods; access modifiers (public, private)
- **Inheritance**: subclass extends superclass; code reuse
- **Polymorphism**: same method name, different behavior in different classes
- **Constructors**: special methods to initialize objects
- Methods: instance methods, static methods, accessor/mutator (getter/setter)
- **UML class diagrams**: representing class structure and relationships

### 4.5 Advanced Programming

#### Sub-programs
- Functions and procedures (methods)
- Parameters: passing by value vs. passing by reference
- Return values
- **Recursion**: function calls itself; requires base case and recursive case
  - Examples: factorial, Fibonacci, binary search

#### File Handling
- Reading from and writing to text files
- Sequential file access
- File operations: open, read, write, close

#### Error Handling
- Types of errors: syntax, runtime, logic
- **Exception handling**: try-catch blocks
- Debugging strategies: trace tables, breakpoints, print statements

## Key Terminology

| Term | Definition |
|------|-----------|
| **Abstraction** | Simplifying complex systems by focusing on essential features |
| **Algorithm** | Step-by-step procedure for solving a problem |
| **Big-O notation** | Describes the upper bound of an algorithm's time complexity |
| **Encapsulation** | Bundling data and methods together; hiding internal state |
| **Inheritance** | Mechanism where a class derives properties and methods from a parent class |
| **Polymorphism** | Ability of different classes to respond to the same method call differently |
| **Recursion** | Technique where a function calls itself to solve a problem |
| **UML** | Unified Modeling Language; standardized diagrams for software design |

## Common Misconceptions

1. **"An algorithm must be written in a programming language"** -- Algorithms can be expressed in pseudocode, flowcharts, or natural language.
2. **"Recursion is always better than iteration"** -- Recursion can be elegant but uses more memory (call stack) and can be slower.
3. **"OOP is the only programming paradigm"** -- Procedural, functional, and other paradigms exist and are useful in different contexts.
4. **"A faster algorithm is always better"** -- Algorithm choice depends on data size, readability, memory constraints, and implementation complexity.
5. **"Binary search works on any array"** -- Binary search requires a sorted array.

## Comparison with AP CS

- AP CS A covers OOP in Java with similar depth (classes, inheritance, polymorphism)
- AP CS A does not cover recursion as deeply as IB (but does include it)
- IB CS uses pseudocode extensively; AP CS A uses Java exclusively
- AP CS Principles covers computational thinking concepts similarly to IB
- IB CS includes file handling and error handling explicitly; AP CS A focuses less on these
