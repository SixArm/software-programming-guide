# Queue data structure

A queue is a fundamental data structure in computer science that follows the First-In-First-Out (FIFO) principle. It is used to store and manage a collection of elements, and its primary operations include adding elements (enqueue) and removing elements (dequeue). The element that was added to the queue first is the first one to be removed.

Think of a queue like a line of people waiting at a ticket counter: the person who arrives first gets served first, and as new people arrive, they join the back of the line. Similarly, in a queue data structure, elements are enqueued at the back and dequeued from the front.

Common ways to implement queues are with arrays or linked lists. Arrays provide constant-time access to elements, but their size may need to be managed. Linked lists provide dynamic sizing and efficient enqueue and dequeue operations.

Common use cases for queues include managing tasks in scheduling algorithms, implementing breadth-first search in graph traversal, and handling request processing in computer systems.

Key operations…

Enqueue: Adding an element to the back of the queue. The new element becomes the last element.

Dequeue: Removing the front element from the queue. The element that was behind the front element becomes the new front.

Peek: View the front element without removing it.

Empty: Check if the queue is empty.

Size: Count the number of elements in the queue.
