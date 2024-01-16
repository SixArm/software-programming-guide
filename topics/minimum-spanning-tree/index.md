# Minimum spanning tree (MST)

A minimum spanning tree (MST) is a subset of edges in a connected, undirected graph that connects all the vertices together with the minimum possible total edge weight. MSTs have applications in network design, clustering, and other optimization problems.

One of the most popular algorithms for finding a minimum spanning tree is Kruskal's algorithm.

Kruskal's algorithm works by iteratively adding the smallest weighted edges to the growing MST while avoiding the formation of cycles. The algorithm is efficient and straightforward to implement.

Steps:

1. Sort Edges: Sort all the edges in the graph in non-decreasing order of their weights.

2. Initialize MST: Create an empty set to represent the MST.

3. Iterate Over Edges: Starting with the smallest edge, iterate through the sorted edges. For each edge, check if adding it to the MST would form a cycle. If adding the edge does not create a cycle, include it in the MST. You can use the Union-Find data structure to efficiently check for cycles.

4. Continue: Repeat step 3 until the MST has V-1 edges, where V is the number of vertices in the graph. This ensures that the MST spans all the vertices.

5. Output MST: The result is a minimum spanning tree.
