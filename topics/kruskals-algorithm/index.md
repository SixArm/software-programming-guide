# Kruskal's algorithm

Kruskal's algorithm is a popular greedy algorithm used for finding the minimum spanning tree (MST) of a connected, undirected graph. The minimum spanning tree is a subset of the graph's edges that forms a tree, connecting all vertices while minimizing the total edge weight. If the graph is disconnected, Kruskal's algorithm can be modified to find a minimum spanning forest.

Steps:

1. Initialize: Start with an empty set (forest) of edges, which will gradually form the minimum spanning tree. Initially, the set contains no edges.

2. Sort Edges: Sort all the edges of the graph in ascending order of their weights.

3. Iterate Through Edges: Starting with the smallest weighted edge, iterate through the sorted list of edges.

4. Add Edges: For each edge in the sorted list, check if adding it to the forest will create a cycle. A cycle is formed if the two vertices connected by the edge are already in the same connected component (tree) of the forest. To check this, you can use techniques like disjoint-set data structures (e.g., union-find). If adding the edge creates a cycle, skip it; otherwise, add the edge to the forest, which means this edge is now part of the minimum spanning tree;

5. Repeat: Continue iterating through the sorted edges, adding edges that do not create cycles and skipping those that do, until you have added (V - 1) edges, where V is the number of vertices in the graph. At this point, the forest of edges forms a minimum spanning tree.

6. Minimum Spanning Tree: The edges that you have added to the forest now constitute the minimum spanning tree of the graph. Return this tree as the output.


