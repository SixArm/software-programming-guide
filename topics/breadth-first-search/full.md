# Breadth-First Search (BFS)

Breadth-First Search (BFS) is a graph traversal algorithm used to explore and search through a graph or tree data structure. Unlike Depth-First Search (DFS), which explores as far as possible along a single branch before backtracking, BFS systematically explores the vertices (nodes) of a graph layer by layer, moving outward from the starting node. BFS is often used in applications like shortest path finding, connected component analysis, and exploring the structure of graphs.

Here's how the Breadth-First Search algorithm works:

* Starting Node: Begin with a selected starting node (or root node) as the initial node.

* Initialization: Create a queue data structure to store nodes to be visited. Enqueue the starting node into the queue.

* Exploration: While the queue is not empty, repeat the following steps:
* * Dequeue a node from the front of the queue.
* * Explore all unvisited neighbors (adjacent nodes) of the dequeued node. Enqueue these neighbors into the queue if they have not been visited.
* * Mark the dequeued node as visited.

* Repeat: Continue the exploration until the queue becomes empty, meaning all reachable nodes have been visited.

BFS systematically explores the graph level by level, ensuring that nodes closer to the starting node are visited before nodes farther away. This makes BFS particularly useful for finding the shortest path from a start node to a goal node in unweighted graphs.

BFS can be adapted for various tasks:

* Shortest Path Finding: BFS guarantees that the first path found from the start node to the goal node is the shortest path.
* Connected Component Analysis: BFS can identify all nodes reachable from a given starting node.
* Web Crawling: BFS can be used to systematically explore and discover web pages by following links in a structured manner.
* Maze Solving: BFS can be used to find the shortest path from the entrance to the exit of a maze.

BFS is generally implemented using a queue data structure, with nodes enqueued and dequeued in the order they were added. This ensures that nodes at the same distance from the start node are visited before nodes farther away.

While BFS is efficient for finding shortest paths in unweighted graphs, it might be less efficient than DFS in terms of memory and time complexity for large and deep graphs. However, BFS guarantees the shortest path, making it a valuable tool in various graph-related tasks.