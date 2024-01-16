# Stack data structure

A stack is a fundamental data structure in computer science that follows the Last-In-First-Out (LIFO) principle. It is used to store and manage a collection of elements, and its primary operations include adding elements (push) and removing elements (pop). The element that was most recently added to the stack is the first one to be removed.

Imagine a physical stack of plates: you can add a new plate on top of the stack, and when you want to remove a plate, you take it from the top. Similarly, in a stack data structure, elements are added and removed from the top of the stack.

Implementations of stacks can vary. In programming, stacks are often implemented using arrays or linked lists. Arrays provide constant-time access to elements, but their size may need to be managed. Linked lists provide dynamic sizing, but access time is linear in the worst case.

Common use cases for stacks include managing function calls and recursion in programming, tracking states in algorithms, implementing undo/redo functionality in applications, and backtracking capabilities for algorithms.

**Key aspects:**

Push: Add an element to the top of the stack. The new element becomes the top element.

Pop: Remove the top element from the stack. The element that was below the top element becomes the new top.

Peek: View the top element without removing it.

Empty: Check if the stack is empty.

Size: Count the number of elements in the stack.
