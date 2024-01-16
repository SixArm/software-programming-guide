# Depth-First Search (DFS)

Depth-First Search (DFS) is a graph traversal algorithm used to explore and search through a graph or tree data structure.

DFS starts at a selected node (usually the root node) and explores as far as possible along each branch before backtracking.

DFS can be implemented using either recursion or an explicit stack data structure. When using recursion, the function calls itself for each unvisited neighbor. With an explicit stack, the nodes are pushed onto the stack and popped off as they are visited.

DFS can be adapted for various tasks: finding a path, cycle detection, topological sorting in directed acyclic graphs (DAGs), and finding connected components.

DFS is unlike Breadth-First Search (BFS), which explores the graph level by level, ensuring that nodes closer to the starting node are visited before nodes farther away. However, DFS may not guarantee the shortest path or the most optimal solution in some scenarios. Also, if the graph is not a DAG, recursive DFS could run into issues with stack overflow for very deep graphs.
