# Bellman-Ford algorithm 

The Bellman-Ford algorithm is used to find the shortest paths from a single source vertex to all other vertices in a weighted directed graph, even when the graph contains negative weight edges. The algorithm iteratively refines the distance estimates until they converge to the correct values.

The Bellman-Ford algorithm has a time complexity of `O(V*E)`, where V is the number of vertices and E is the number of edges in the graph. It's a versatile algorithm for finding shortest paths in graphs with negative weights, but it may not be as efficient as Dijkstra's algorithm for graphs with non-negative weights.

If there is a negative weight cycle in the graph, the algorithm can detect it. In the presence of a negative weight cycle reachable from the source vertex, the algorithm reports that no shortest path exists, as the shortest path can have an infinite negative weight.

Steps:

1. Initialize: The algorithm initializes the distance to the source vertex as 0 and the distance to all other vertices as infinity. It maintains a list of distances and updates them iteratively.

2. Iterate: The algorithm performs a series of iterations, where each iteration relaxes the distances for all edges. Relaxing an edge means improving the estimate of the distance from the source to the destination vertex if a shorter path is found.

3. Relax: For each edge `(u, v)` in the graph, if the distance estimate to vertex `v` through vertex `u` (`distance[u] + weight(u, v)`) is shorter than the current estimate for `v` (`distance[v]`), then `distance[v]` is updated to the new, shorter value.

4. Converge: Repeat the relaxation step for all edges for a total of `V-1` iterations, where `V` is the number of vertices in the graph. After `V-1` iterations, the distances have converged to their correct values if there are no negative weight cycles.
