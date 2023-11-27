# Splay tree

A splay tree is a type of self-adjusting binary search tree (BST) that optimizes its structure for frequently accessed elements. It achieves this by bringing recently accessed nodes closer to the root through a process called "splaying". Splaying involves a series of tree rotations and other operations to move the accessed node to the root position. While splay trees do not guarantee a balanced tree structure in the traditional sense (such as AVL trees or Red-Black trees), they exhibit excellent amortized performance.

Key operations:

* Splay: Splaying is the core operation in a splay tree. When you access a node (e.g., by searching for a value), the tree is restructured so that the accessed node becomes the root. Splaying involves a series of rotations, zig-zag and zig-zig operations, and other transformations to move the accessed node closer to the root.

* Search: To search for a value in a splay tree, you perform a standard binary search operation. While doing this, you splay the accessed node to the root to optimize future accesses to that node.

* Insert: When you insert a new element into a splay tree, you first perform a standard binary search to find the insertion point. After inserting the node, you splay it to the root to bring it closer to the root.

* Delete: Deletion in a splay tree follows the standard BST deletion process. After deletion, you splay the parent of the deleted node to the root.
