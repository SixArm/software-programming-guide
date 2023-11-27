# Queue data structure

A queue is a fundamental data structure in computer science that follows the First-In-First-Out (FIFO) principle. It is used to store and manage a collection of elements, and its primary operations include adding elements (enqueue) and removing elements (dequeue). The element that was added to the queue first is the first one to be removed.

Think of a queue like a line of people waiting at a ticket counter: the person who arrives first gets served first, and as new people arrive, they join the back of the line. Similarly, in a queue data structure, elements are enqueued at the back and dequeued from the front.

Key operations of a queue:

* Enqueue: Adding an element to the back of the queue. The new element becomes the last element.
* Dequeue: Removing the front element from the queue. The element that was behind the front element becomes the new front.
* Front (or Peek): Viewing the front element without removing it.
* IsEmpty: Checking if the queue is empty.
* Size: Counting the number of elements in the queue.

Common use cases for queues include managing tasks in scheduling algorithms, implementing breadth-first search in graph traversal, and handling request processing in computer systems.

Example scenarios illustrating queue behavior:

* Task Scheduling: In an operating system, a queue can be used to manage tasks in a scheduling algorithm, where the task at the front is the one currently being executed.

* Breadth-First Search: Queues are used to explore levels of a graph in breadth-first search, where nodes at a given distance from the start node are explored before nodes farther away.

* Print Job Management: In a printer queue, print jobs are processed in the order they are received, with the first job enqueued being the first one printed.

* Request Handling: In web servers or computer systems, incoming requests are enqueued in a queue and processed in the order they were received.

Queues can be implemented using arrays or linked lists. Arrays provide constant-time access to elements, but their size may need to be managed. Linked lists provide dynamic sizing and efficient enqueue and dequeue operations.

The queue data structure is crucial in various applications, particularly when order matters and tasks or data need to be processed in a sequential manner based on their arrival time.