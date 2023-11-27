# Kruskal's algorithm

Kruskal's algorithm is a popular greedy algorithm used for finding the minimum spanning tree (MST) of a connected, undirected graph. The minimum spanning tree is a subset of the graph's edges that forms a tree, connecting all vertices while minimizing the total edge weight. Kruskal's algorithm was developed by Joseph Kruskal in 1956 and is widely used in network design, circuit design, and other applications that involve connecting a set of points with the least possible total edge weight.

Steps…

Initialize: Start with an empty set (forest) of edges, which will gradually form the minimum spanning tree. Initially, the set contains no edges.

Sort Edges: Sort all the edges of the graph in ascending order of their weights.

Iterate Through Edges: Starting with the smallest weighted edge, iterate through the sorted list of edges.

Add Edges: For each edge in the sorted list, check if adding it to the forest will create a cycle. A cycle is formed if the two vertices connected by the edge are already in the same connected component (tree) of the forest. To check this, you can use techniques like disjoint-set data structures (e.g., union-find). If adding the edge creates a cycle, skip it; otherwise, add the edge to the forest, which means this edge is now part of the minimum spanning tree;

Repeat: Continue iterating through the sorted edges, adding edges that do not create cycles and skipping those that do, until you have added (V - 1) edges, where V is the number of vertices in the graph. At this point, the forest of edges forms a minimum spanning tree.

Minimum Spanning Tree: The edges that you have added to the forest now constitute the minimum spanning tree of the graph. Return this tree as the output.

Kruskal's algorithm is efficient and works well on sparse graphs. It ensures that the minimum spanning tree is created by selecting edges with the smallest weights first. It doesn't depend on the starting vertex, and it guarantees a minimum spanning tree in the end.

One important note is that if the graph is disconnected, Kruskal's algorithm can be modified to find a minimum spanning forest, which is a collection of minimum spanning trees, one for each connected component of the graph.