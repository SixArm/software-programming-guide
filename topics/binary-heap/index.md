# Binary heap

A binary heap data structure is a specialized tree that is efficient for maintaining a dynamically changing collection of elements with efficient insertion, deletion, and retrieval of the minimum element or maximum element. 

A binary heap is commonly used for implementing priority queues, and is a component in other algorithms, including heapsort.

Key aspects…

Heap Property: 

* In a min-heap, for any given node, the value of that node is less than or equal to the values of its children. 

* In a max-heap, for any given node, the value of that node is greater than or equal to the values of its children.

Basic Operations:

* Insert: To insert a new element into a binary heap, you typically add it as a leaf node and then "bubble it up" or "percolate it up" by swapping it with its parent until the heap property is restored.

* Delete: To remove the top (root) element from a binary heap, you replace it with the last leaf node, remove the last leaf, and then "bubble it down" or "percolate it down" by swapping it with its smaller (in a min-heap) or larger (in a max-heap) child until the heap property is restored.

* Peek: To access the top element without removing it, you simply return the root element.

Binary heaps can be represented as arrays, where each element's index i has left and right children at indices 2i+1 and 2i+2, respectively, and the parent is at index floor((i-1)/2).

