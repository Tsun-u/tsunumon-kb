# Big Idea 3: Algorithms and Programming (AAP)
> Exam Weight: 30-35%

Programmers combine algorithms and abstraction to write creative programs or solve real-world problems. Executing multiple instructions in a specified order, making decisions based on conditions, and repeating operations are the three fundamental building blocks of any program.

## Topics

### Variables and Assignment

#### Storing Values with Variables

- A variable is an abstraction inside a program that holds a value in memory; each variable holds exactly one value at a time
- Choosing meaningful variable names improves readability and helps others understand what each value represents
- Some programming languages include a type system that binds variables to specific data types (such as integer, string, or boolean)

#### Assignment and Updating Variables

- An assignment operator lets a program change the value stored in a variable
- A variable always holds the most recently assigned value
- An assignment statement evaluates the expression on the right side of the operator and writes the result into the variable
- Example: `a <- expression` evaluates the right-hand side and stores the result in `a`

---

### Data Abstraction, Sequencing, Selection, Iteration, and Algorithms

#### Describing Algorithms Without Code

- An **algorithm** is a finite set of instructions designed to accomplish a specific task
- Beyond visual and text-based programming languages, algorithms can also be expressed in natural language, flowcharts, or pseudocode
- Algorithms can be designed from scratch or built by combining and adapting existing ones

#### Expressing Step-by-Step Processes with Sequential Code

- **Sequencing** means executing each step in the order the code is written
- Each code statement is a basic unit of execution that expresses one action to be performed

#### Arithmetic Operators

- Arithmetic operators include: addition (+), subtraction (-), multiplication (\*), division (/), and modulo (MOD)
- The standard mathematical order of operations applies in programming languages as well
- MOD returns the remainder of integer division (example: 17 MOD 5 = 2)

#### String Operations

- A string is an ordered sequence of characters
- String operations include: concatenation (joining strings together), extracting a substring, and getting the length of a string

#### Comparing Two Values

- Relational operators include: equal to (=), not equal to (!=), greater than (>), less than (<), greater than or equal to (>=), and less than or equal to (<=)
- A **Boolean** value is either true or false
- The result of a relational operation is always a Boolean value

#### Logical Operations on Boolean Values

- Logical operators: NOT, AND, OR
- NOT reverses a Boolean value
- AND produces true only when both operands are true
- OR produces true when at least one operand is true
- Order of precedence for logical operators: NOT first, then AND, then OR

#### Selection (Conditional Statements)

- **Selection** uses a condition to determine which block of code to execute
- `IF(condition)` executes a block when the condition is true; skips it when false
- `IF(condition) / ELSE` takes one path when the condition is true and another when it is false
- **Nested conditionals**: placing one conditional statement inside another

#### Iteration

- **Iteration** is the repeated portion of an algorithm; it can repeat a fixed number of times or repeat until a condition becomes true
- `REPEAT n TIMES`: executes a block of code exactly n times
- `REPEAT UNTIL(condition)`: keeps repeating until the condition evaluates to true
- Iteration can be used to traverse every element in a data structure like a list
- Combined with selection and sequencing, iteration alone is enough to implement any algorithm

#### Lists

- A list is an ordered collection of elements
- Each element has a unique index within the list
- Indexes are typically positive integers starting at 1 (AP CSP pseudocode convention)
- A string can be thought of as a list of characters

#### Comparing Different Algorithms for the Same Problem

- Most problems can be solved by more than one algorithm
- Algorithms that look similar on the surface may produce different side effects or results
- Different algorithms for the same problem may differ significantly in efficiency

#### The General Capability of Algorithms

- Any algorithm can be written using just three structures: sequencing, selection, and iteration
- Common pre-built algorithms include: computing the sum or average of a list, finding the maximum or minimum value, and searching or sorting a list
- Starting from correct existing algorithms as building blocks makes constructing more complex algorithms much more efficient

#### List Operations

- List operations include: accessing an element by index, modifying an element, inserting an element, appending an element, deleting an element, and getting the length of the list
- **Traversing** a list means accessing each element in sequence
- **Linear search / sequential search**: starts from the beginning and checks each element one by one until the target is found or the list is exhausted

#### Algorithms That Operate on List Elements

- When traversing a list, you can perform various operations on each element
- Common traversal operations: searching, filtering, counting, summing, finding the maximum or minimum
- **Binary search** requires a sorted list and works by comparing the target to the middle element, then cutting the search range in half each time
- For large sorted lists, binary search is far more efficient than linear search

#### Analyzing Algorithms That Combine All Three Structures

- Familiarity with well-known algorithms (search, sort) makes writing more complex algorithms much easier
- Binary search can only run on sorted data
- Binary search begins at the middle of a sorted dataset and eliminates half the remaining data with each iteration — far outpacing linear search on large inputs

---

### Procedures (Functions)

#### Calling a Procedure

- A **procedure** is a named set of program instructions that can have parameters and a return value
- Different languages use different names for procedures: method, function, subroutine
- **Parameters** are the input variables of a procedure; **arguments** are the actual values passed in when calling it
- When a procedure is called, execution pauses, jumps into the procedure, runs it to completion, and then returns
- Using parameters makes procedures more flexible and reusable

#### How Procedural Abstraction Reduces Complexity

- **Procedural abstraction** gives a process a name so callers only need to know *what it does*, not *how it does it*
- Through procedural abstraction, the same procedure can be reused in many different contexts
- Parameters make procedures more general and further increase reusability
- Procedural abstraction improves code readability
- Libraries and APIs make it much easier to build complex programs

#### Writing Procedures to Manage Complexity

- A **software library** contains ready-made procedures available for use when building new programs
- Existing code segments can serve as building blocks for constructing new programs
- An **API (Application Programming Interface)** defines the behavior and usage rules for the procedures in a library
- Before using a library or API, reading its documentation is essential to understand what it can do and how to call it correctly

#### Choosing an Appropriate Library or Existing Code

- Software libraries contain pre-built procedures that simplify program construction
- APIs define how library procedures behave and how to interact with them
- Documentation is indispensable for using any library or API correctly

#### Generating Random Values

- `RANDOM(a, b)` returns a random integer between a and b, inclusive
- Random number generators are useful for simulating real-world random events
- Using a random number generator means the program may produce different output each time it runs

---

### Algorithm Efficiency and Limits

#### Measuring Algorithm Efficiency

- Algorithm efficiency is measured by the number of steps required to complete a task relative to the size of the input
- Efficiency is usually expressed as a function of the input size (n)
- Algorithms with polynomial or lower complexity (constant, linear, quadratic, cubic, etc.) are considered reasonably efficient
- Algorithms with exponential complexity are considered unreasonable — they become practically unsolvable for large inputs
- Some problems cannot be solved in a reasonable amount of time regardless of which algorithm is used

#### Undecidable Problems in Computer Science

- A **decidable problem** is one for which an algorithm exists that gives a correct yes/no answer for every possible input (example: "Is this number even?")
- An **undecidable problem** is one for which no algorithm can guarantee a correct yes/no answer for all possible inputs
- An undecidable problem may have solutions for specific inputs, but no single algorithm handles all cases
- Classic example: **the halting problem** — it is impossible to write an algorithm that can determine, for any arbitrary program, whether that program will eventually stop running

---

## Robot Grid Problems (Exam Format Reference)

AP CSP exams include problems simulating a robot moving on a grid:
- The robot can move forward, turn left, and turn right, and can detect whether the space ahead is open
- Students trace through pseudocode to determine the robot's path or final position
- These problems test understanding of sequencing, selection, and iteration in a visual format
