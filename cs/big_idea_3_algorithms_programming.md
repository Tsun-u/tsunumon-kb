# Big Idea 3: Algorithms and Programming (AAP)
> Exam Weight: 30-35%

Programmers integrate algorithms and abstraction to create programs for creative purposes and to solve problems. Using multiple program statements in a specified order, making decisions, and repeating the same process multiple times are the building blocks of programs.

## Topics

### AAP-1: Variables and Assignments

#### AAP-1.A: Represent a value with a variable
- **Essential Knowledge:**
  - A variable is an abstraction inside a program that can hold a value; each variable has associated data storage that represents one value at a time
  - Using meaningful variable names helps with the readability of program code and understanding of what values are represented by the variables
  - Some programming languages provide types to represent data, which are referenced using variables (e.g., integers, strings, Booleans)

#### AAP-1.B: Determine the value of a variable as a result of an assignment
- **Essential Knowledge:**
  - The assignment operator allows a program to change the value represented by a variable
  - The value stored in a variable will be the most recent value assigned
  - An assignment statement sets (or changes) the value stored in the variable to the value on the right side of the assignment operator
  - For example: `a <- expression` evaluates the expression and assigns the result to variable `a`

---

### AAP-2: Data Abstraction, Sequences, Selection, Iteration, and Algorithms

#### AAP-2.A: Express an algorithm that uses sequencing without using a programming language
- **Essential Knowledge:**
  - An algorithm is a finite set of instructions that accomplish a specific task
  - Beyond visual and textual programming languages, algorithms can be expressed using natural language, flowcharts, and pseudocode
  - Algorithms can be created from an idea, by combining existing algorithms, or by modifying existing algorithms

#### AAP-2.B: Represent a step-by-step algorithmic process using sequential code statements
- **Essential Knowledge:**
  - Sequencing is the application of each step of an algorithm in the order in which the code statements are given
  - A code statement is a part of program code that expresses an action to be carried out

#### AAP-2.C: Evaluate expressions that use arithmetic operators
- **Essential Knowledge:**
  - Arithmetic operators: addition (+), subtraction (-), multiplication (*), division (/), modulus (MOD)
  - The order of operations used in mathematics applies in programming
  - MOD returns the remainder when one integer is divided by another (e.g., 17 MOD 5 = 2)

#### AAP-2.D: Evaluate expressions that manipulate strings
- **Essential Knowledge:**
  - Strings are ordered sequences of characters
  - String operations include concatenation (joining strings), extracting substrings, and finding the length of a string

#### AAP-2.E: For relationships between two variables, expressions, or values
- **Essential Knowledge:**
  - Relational operators: equal (=), not equal (!=), greater than (>), less than (<), greater than or equal (>=), less than or equal (<=)
  - A Boolean value is either true or false
  - The result of a relational operation is a Boolean value

#### AAP-2.F: For relationships between Boolean values
- **Essential Knowledge:**
  - Logical operators: NOT, AND, OR
  - NOT negates a Boolean value
  - AND evaluates to true only when both operands are true
  - OR evaluates to true when at least one operand is true
  - The evaluation of logical operators follows a well-defined order: NOT is evaluated first, then AND, then OR

#### AAP-2.G: Express an algorithm that uses selection without using a programming language
#### AAP-2.H: Determine the result of conditional statements
- **Essential Knowledge:**
  - Selection determines which parts of an algorithm are executed based on a condition being true or false
  - IF(condition) executes a block of statements if the condition is true; otherwise the block is skipped
  - IF(condition) / ELSE executes one block if the condition is true and a different block if the condition is false
  - Nested conditionals: conditional statements within other conditional statements

#### AAP-2.I: Express an algorithm that uses iteration without using a programming language
#### AAP-2.J: Determine the result of iterative statements
- **Essential Knowledge:**
  - Iteration is a repeating portion of an algorithm; iteration repeats a specified number of times or until a given condition is met
  - REPEAT n TIMES: repeats a block of statements n times
  - REPEAT UNTIL(condition): repeats a block of statements until the condition evaluates to true
  - Iteration can be used to traverse data structures such as lists
  - The use of iteration alongside selection and sequencing is sufficient to implement any algorithm

#### AAP-2.K: For lists
- **Essential Knowledge:**
  - A list is an ordered sequence of elements
  - An element is an individual value in a list that is assigned a unique index
  - An index is a common method for referencing the elements in a list (index values are usually positive integers starting at 1 in AP CSP pseudocode)
  - A string can be considered a list of characters

#### AAP-2.L: Compare multiple algorithms designed to accomplish the same task
- **Essential Knowledge:**
  - There are often multiple algorithms that can be used to solve the same problem
  - Algorithms that appear similar can yield different side effects or results
  - Different algorithms can be developed to solve the same problem; each algorithm may have different efficiencies

#### AAP-2.M: For algorithms
- **Essential Knowledge:**
  - Algorithms can be written using sequencing, selection, and iteration
  - Existing algorithms include: finding the sum or average of a list, determining the min or max of a list, and searching or sorting a list
  - Using existing correct algorithms as building blocks for constructing more complex algorithms helps manage complexity

#### AAP-2.N: For list operations
- **Essential Knowledge:**
  - List operations include: accessing elements by index, assigning values to elements, inserting elements, appending elements, removing elements, determining the length of a list
  - Traversing a list means accessing each element in the list one at a time
  - A linear search (or sequential search) checks each element in order until the desired value is found or the end of the list is reached

#### AAP-2.O: For algorithms involving elements of a list
- **Essential Knowledge:**
  - Algorithms can be written to traverse a list and perform operations on each element
  - Common list traversal operations: searching, filtering, counting, summing, finding minimum/maximum
  - The binary search algorithm requires a sorted list and repeatedly divides the search interval in half
  - Binary search is more efficient than linear search for large sorted lists

#### AAP-2.P: Determine the result of algorithms that include sequential, selection, and iterative statements
- **Essential Knowledge:**
  - Knowledge of existing algorithms (searching, sorting) is useful for writing more complex algorithms
  - Data must be in sorted order to use the binary search algorithm
  - The binary search algorithm starts at the middle of a sorted data set and eliminates half of the data in each iteration; this makes binary search more efficient than linear search

---

### AAP-3: Procedures (Functions)

#### AAP-3.A: For procedure calls
- **Essential Knowledge:**
  - A procedure is a named group of programming instructions that may have parameters and return values
  - Procedures are referred to by different names in different languages (method, function, subroutine)
  - Parameters are input variables of a procedure; arguments are the values passed to parameters when a procedure is called
  - A procedure call interrupts the sequential execution of statements, causing the program to execute the statements within the procedure before continuing
  - The use of parameters can make procedures more flexible and reusable

#### AAP-3.B: Explain how the use of procedural abstraction manages complexity in a program
- **Essential Knowledge:**
  - One common type of abstraction is procedural abstraction, which provides a name for a process and allows a procedure to be used only knowing what it does, not how it does it
  - Procedural abstraction allows a procedure to be reused in different contexts without knowing the details of the algorithm
  - Using parameters allows procedures to be generalized, enabling code reuse
  - Using procedural abstraction helps improve code readability
  - The use of libraries and APIs simplifies creating complex programs

#### AAP-3.C: Develop procedural abstractions to manage complexity in a program by writing procedures
- **Essential Knowledge:**
  - A software library contains procedures that may be used in creating new programs
  - Existing code segments can be used as building blocks for new programs
  - APIs (Application Programming Interfaces) provide specifications for how procedures in a library behave and can be used
  - Documentation for an API/library is necessary to understand the behaviors provided by the API/library and how to use them

#### AAP-3.D: Select appropriate libraries or existing code segments to use in creating new programs
- **Essential Knowledge:**
  - A software library contains procedures useful for creating programs
  - An API defines how procedures in a library behave and can be used
  - Documentation is critical for understanding how to use a library or API

#### AAP-3.E: For generating random values
- **Essential Knowledge:**
  - RANDOM(a, b) generates a random integer from a to b inclusive
  - Random number generation can be used to simulate real-world events
  - Using random number generators in a program means the output may differ each time the program is run

---

### AAP-4: Algorithm Efficiency and Limits of Algorithms

#### AAP-4.A: For determining the efficiency of an algorithm
- **Essential Knowledge:**
  - The efficiency of an algorithm is determined by the number of steps it takes to complete, relative to the size of the input
  - An algorithm's efficiency is typically expressed in terms of the size of the input
  - An algorithm with a polynomial efficiency or lower (constant, linear, square, cube, etc.) is said to run in a reasonable amount of time
  - An algorithm with exponential efficiency is said to run in an unreasonable amount of time
  - Some problems cannot be solved in a reasonable amount of time for any input size

#### AAP-4.B: Explain the existence of undecidable problems in computer science
- **Essential Knowledge:**
  - A decidable problem is a decision problem for which an algorithm can be written to produce a correct output for all inputs (e.g., "Is a number even?")
  - An undecidable problem is one for which no algorithm can be constructed that is always capable of providing a correct yes-or-no answer
  - An undecidable problem may have some instances that have an algorithmic solution, but there is no algorithm that can solve all instances of the problem
  - A classic example: the halting problem — it is not possible to write an algorithm that can determine whether an arbitrary program will eventually halt or run forever

---

## Robot Grid Questions (Exam Reference)

The AP CSP exam includes questions using a simulated robot on a grid:
- The robot can move forward, turn left, turn right, and check if it can move forward
- Students must trace through pseudocode to determine the robot's path or final position
- These questions test understanding of sequencing, selection, and iteration in a visual context
