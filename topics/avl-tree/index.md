# AVL tree

An AVL tree, also known as a self-balancing binary search tree, is a data structure designed to maintain balance in a binary search tree to ensure efficient operations like insert, delete, and search. In an AVL tree, the balance factor of each node, defined as the height of its left subtree minus the height of its right subtree, is limited to be in the range `[-1, 0, 1]`. If the balance factor of a node violates this constraint, the tree is rebalanced through rotations.

Key operations:

* Insert: When inserting a new element, it's added to the tree like a regular binary search tree insertion. After the insertion, the balance factors of the nodes along the insertion path are updated. If any node becomes unbalanced, the appropriate rotation(s) are performed to restore balance.

* Delete: When deleting a node, it's removed like a regular binary search tree deletion. After the deletion, the balance factors of the nodes along the path from the deleted node to the root are updated, and rotations are applied if necessary to rebalance the tree.

* Search: Searching in an AVL tree follows the standard binary search tree search operation.

* Rotate: To maintain balance, AVL trees use four types of rotations: Left Rotation (LL Rotation), Right Rotation (RR Rotation), Left-Right Rotation (LR Rotation), Right-Left Rotation (RL Rotation)
