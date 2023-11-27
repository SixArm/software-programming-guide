# Dijkstra's algorithm

Dijkstra's algorithm is a popular algorithm for finding the shortest path from a starting node to all other nodes in a weighted, directed graph with non-negative edge weights. It is useful for solving problems involving network routing and finding the shortest distance between two locations on a map.

The algorithm works by maintaining a set of nodes for which the shortest path from the starting node is known, and a set of nodes for which the shortest path is yet to be determined. It iteratively selects the node with the smallest known distance and updates the distances to its neighbors, gradually building the shortest path tree.

Steps:

1. Initialize: Initialize a list or array to store the shortest distance from the starting node to each node. Initialize the distance to the starting node as 0 and set the distance to all other nodes as infinity. Initialize a priority queue or min-heap to store nodes by their distance values, then add the starting node with a distance of 0 to the queue. Initalize a set or array to keep track of visited nodes.

2. While the priority queue is not empty: Extract the node with the smallest distance from the priority queue. This node is the current node. Mark the current node as visited (i.e., move it from the "unvisited" set to the "visited" set).

3. For each neighbor of the current node that is still unvisited: Calculate the distance from the starting node to the neighbor through the current node. If this calculated distance is shorter than the previously recorded distance to the neighbor, update the distance. Add the neighbor to the priority queue with its updated distance.

4. When the algorithm finishes, the list or array of shortest distances will contain the shortest distance from the starting node to every other node in the graph.

