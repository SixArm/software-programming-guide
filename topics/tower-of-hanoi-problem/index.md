# Tower of Hanoi problem

The Tower of Hanoi problem is a classic puzzle in computer science and mathematics. It consists of three pegs and a series of disks of different sizes that can slide onto any peg. The problem begins with the disks in a neat stack in ascending order of size on one peg, the smallest at the top, creating a conical shape. The objective of the puzzle is to move the entire stack to another peg, obeying the following simple rules:

* Only one disk can be moved at a time.

* Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack or on an empty peg.

* No disk may be placed on top of a smaller disk.

The Tower of Hanoi problem can be solved recursively. Suppose there are n disks on the first peg, and the objective is to move them to the third peg. We can break down the problem as follows:

* Move n-1 disks from the first peg to the second peg, using the third peg as an auxiliary.

* Move the largest disk (disk n) from the first peg to the third peg.

* Move the n-1 disks from the second peg to the third peg, using the first peg as an auxiliary.

This algorithm can be visualized as a tree of recursive function calls, where each node represents a subproblem and the edges represent the function calls. The base case is when n=1, in which case the problem is trivial and can be solved in one move.

The Tower of Hanoi problem is an example of a problem that can be solved recursively but has an exponential time complexity, meaning that the number of steps required to solve the problem grows exponentially with the size of the input. Therefore, for large values of n, the problem becomes impractical to solve using a recursive algorithm.
