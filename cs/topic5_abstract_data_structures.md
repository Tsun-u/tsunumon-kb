# Topic 5: Abstract Data Structures

> HL only

## Key Concepts

### 5.1 Abstract Data Types (ADTs)

- An ADT defines a data type by its behavior (operations) rather than implementation
- Separation of interface from implementation
- Common ADTs: stack, queue, linked list, binary tree

### 5.2 Linked Lists

- **Singly linked list**: each node contains data and a pointer to the next node
  - Head pointer: reference to the first node
  - Null pointer: indicates end of list
- Operations:
  - **Insert**: at head, at tail, at position
  - **Delete**: by value or by position
  - **Search**: traverse from head, checking each node
  - **Traverse**: visit each node in sequence
- Advantages over arrays: dynamic size, efficient insertion/deletion
- Disadvantages: no random access, extra memory for pointers
- **Doubly linked list**: each node has pointers to both next and previous nodes

### 5.3 Stacks

- **LIFO** (Last In, First Out) data structure
- Operations:
  - **Push**: add element to top
  - **Pop**: remove and return top element
  - **Peek/Top**: view top element without removing
  - **isEmpty**: check if stack is empty
- Applications:
  - Undo/redo functionality
  - Expression evaluation (postfix/RPN)
  - Bracket matching
  - Recursion call stack
  - Backtracking algorithms (maze solving, DFS)

### 5.4 Queues

- **FIFO** (First In, First Out) data structure
- Operations:
  - **Enqueue**: add element to rear
  - **Dequeue**: remove element from front
  - **Peek/Front**: view front element without removing
  - **isEmpty**: check if queue is empty
- **Circular queue**: wraps around to use empty spaces at the front
- **Priority queue**: elements dequeued by priority, not arrival order
- Applications:
  - Print job scheduling
  - BFS (breadth-first search)
  - Process scheduling in operating systems
  - Buffer management

### 5.5 Binary Trees

- **Binary tree**: each node has at most two children (left and right)
- **Binary search tree (BST)**: left child < parent < right child
  - Operations: insert, delete, search — all O(log n) average case, O(n) worst case
- **Tree traversal**:
  - **In-order** (LNR): left → node → right → produces sorted output for BST
  - **Pre-order** (NLR): node → left → right → used for copying tree structure
  - **Post-order** (LRN): left → right → node → used for deletion
- Applications: database indexing, file systems, expression parsing, decision trees

### 5.6 Dynamic vs. Static Data Structures

| Feature | Static (e.g., Array) | Dynamic (e.g., Linked List) |
|---------|------|---------|
| Size | Fixed at creation | Can grow/shrink |
| Memory | Allocated in contiguous block | Nodes can be anywhere |
| Access | Random access O(1) | Sequential access O(n) |
| Insertion/Deletion | O(n) (shifting needed) | O(1) at known position |
| Memory efficiency | May waste space | Extra overhead for pointers |

### 5.7 Recursion with Data Structures
- Recursive traversal of linked lists
- Recursive tree traversal
- Recursive definition: a tree is either empty or a node with two subtrees

## Key Terminology

| Term | Definition |
|------|-----------|
| **ADT** | Abstract Data Type; defines behavior through operations, not implementation |
| **LIFO** | Last In, First Out; stack ordering principle |
| **FIFO** | First In, First Out; queue ordering principle |
| **Node** | Element in a data structure containing data and reference(s) to other nodes |
| **Pointer/Reference** | Variable storing the memory address of another data element |
| **BST** | Binary Search Tree; binary tree where left < parent < right |
| **Traversal** | Visiting each node in a data structure in a systematic order |

## Common Misconceptions

1. **"Arrays are always better because of random access"** -- For frequent insertions/deletions, linked lists are more efficient.
2. **"Stacks and queues are fundamentally different from arrays"** -- They are often implemented using arrays (or linked lists); the difference is in the access pattern.
3. **"Binary trees are always balanced"** -- Without balancing algorithms, a BST can degenerate to a linked list (all nodes on one side).
4. **"Recursion is required for tree traversal"** -- Iterative traversal is possible using an explicit stack or queue.

## Comparison with AP CS

- AP CS A covers arrays and ArrayLists but does not cover linked lists, stacks, queues, or trees
- AP CS A's curriculum ends at basic data structures; IB HL provides a mini data structures course
- IB HL coverage of ADTs is more aligned with a university-level data structures course
