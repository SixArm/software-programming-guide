# Strongly Connected Components (SCC)

Strongly Connected Components (SCCs) are subsets of vertices in a directed graph such that, within each subset, there is a path from every vertex to every other vertex. In other words, if you pick any two vertices within an SCC, you can reach one from the other by following the edges in the graph. SCCs provide a way to analyze the connectivity of directed graphs.

SCCs are essential in various applications, such as optimizing network flows, analyzing program control flow, and identifying communities in social networks.

One of the most commonly used algorithms to find SCCs is Kosaraju's algorithm. 

Steps…

1. Compute the Reverse Graph. Create a new graph with the same vertices as the original graph, but with all edges reversed. This is done by reversing the direction of each edge.

2. Depth-First Search (DFS) on the Reverse Graph. Perform a depth-first search on the reverse graph. Start from any unvisited vertex, and keep track of the vertices encountered during the DFS.

3. When the DFS is completed, the vertices encountered in this pass form the first SCC.

4. Repeat the process by selecting an unvisited vertex, but this time explore a different SCC.

5. Continue until all vertices are visited.
