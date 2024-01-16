# Balanced tree (b-tree)

A balanced tree (b-tree) is a self-balancing tree-like data structure that maintains sorted data and provides efficient operations for insert, delete, and search. B-trees are commonly used in databases and file systems because of their ability to handle large datasets efficiently.

The root node is the topmost node in the b-tree. All leaf nodes are at the same level and contain data entries. They have no children, and they can have between t-1 and 2t-1 keys.

**Key aspects:**

* Split: When a node exceeds its maximum allowed number of keys, it is split into two nodes; the median key is promoted to the parent node.

* Merge: When a node has fewer than t-1 keys after a deletion, it can borrow keys from a sibling node or merge with a sibling node to maintain balance.

* Self-balance: The height of the tree is kept as balanced as possible, so operations like insert and delete are performed in logarithmic time.

* Order: A b-tree has a parameter known as its "order" or "degree" (often denoted as `t`) which determines the maximum number of children a node can have. Typically a node can have between `t-1` and `2t-1` keys.

* Sorted keys: Keys within each node are sorted in ascending order. This allows for efficient searching using binary search within a node.

* Child pointers: Each non-leaf node has one more child pointer than the number of keys. These child pointers guide the traversal of the tree.

* Traversal: b-trees support in-order traversal, which allows efficient retrieval of all keys in sorted order.
