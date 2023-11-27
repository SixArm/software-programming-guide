# Topological sort algorithm

Topological sort is an algorithm used to linearly order the vertices of a directed acyclic graph (DAG) in such a way that for every directed edge (u, v), vertex u comes before vertex v in the ordering. In other words, it arranges the vertices in a linear order that respects the direction of edges, ensuring that there are no cycles in the resulting order.

Topological sort is commonly used in applications where you need to schedule tasks with dependencies, such as in project scheduling or build systems.

It's important to note that topological sorting is only defined for directed acyclic graphs (DAGs). If the input graph contains cycles, the algorithm will not produce a valid topological order. Therefore, it's crucial to ensure that the input graph is acyclic before applying topological sorting.

Steps:

1. Initialization: Start with an empty result list and an empty set or array to keep track of visited vertices.

2. Choose a Start Vertex: Select any unvisited vertex as the starting point. This can be done by traversing the graph and finding a vertex with no incoming edges (in-degree of 0).

3. Depth-First Search (DFS): Starting from the chosen vertex, perform a depth-first search (DFS) on the graph, visiting unvisited neighbors. During the DFS, add vertices to the result list once you've visited all of their neighbors.

4. Backtrack: After completing the DFS from a vertex, you backtrack to the parent node and repeat the process for any unvisited neighbors. Continue this process until all vertices have been visited.

5. Result: The result list will contain the topologically sorted order of the vertices, with the vertices that have no incoming edges coming first.

