# Topic 4: Computational Thinking, Problem-Solving and Programming

> SL + HL | Core Topic (largest topic)

## Key Concepts

### 4.1 General Principles of Computational Thinking

- **Abstraction**: stripping away irrelevant detail so you can focus on what actually matters for the problem
- **Decomposition**: splitting a large problem into smaller, more tractable sub-problems
- **Pattern recognition**: noticing shared structures or recurring trends across problems or datasets
- **Algorithmic thinking**: constructing a precise, ordered set of steps that leads to a solution

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
| **Abstraction** | Hiding unnecessary complexity so that thinking can stay at the right level |
| **Algorithm** | A finite, unambiguous sequence of steps that solves a problem |
| **Big-O notation** | A notation for expressing how an algorithm's time (or space) requirement grows relative to input size |
| **Encapsulation** | Packaging an object's data together with the methods that act on it, and restricting direct access from outside |
| **Inheritance** | A relationship where one class acquires the attributes and methods of a parent class |
| **Polymorphism** | The ability for different classes to provide their own implementations of the same method name |
| **Recursion** | An approach where a function solves a problem by calling itself on a smaller version of that problem |
| **UML** | Unified Modeling Language; a standardized notation for visualizing software structure and behavior |

## Common Misconceptions

1. **"An algorithm must be written in a programming language"** — Algorithms can be expressed in pseudocode, flowcharts, or plain natural language; code is just one form.
2. **"Recursion is always better than iteration"** — Recursion can be cleaner to read, but it consumes call-stack memory and can be slower than an equivalent loop.
3. **"OOP is the only programming paradigm"** — Procedural, functional, and declarative paradigms each have contexts where they work better.
4. **"A faster algorithm is always better"** — The right choice depends on data size, available memory, readability requirements, and how complex the implementation is.
5. **"Binary search works on any array"** — Binary search only works correctly on a sorted array.

## Comparison with AP CS

- AP CS A covers OOP in Java with similar depth (classes, inheritance, polymorphism)
- AP CS A does not cover recursion as deeply as IB (but does include it)
- IB CS uses pseudocode extensively; AP CS A uses Java exclusively
- AP CS Principles covers computational thinking concepts similarly to IB
- IB CS includes file handling and error handling explicitly; AP CS A focuses less on these
