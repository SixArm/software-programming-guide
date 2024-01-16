# Binary search tree (BST)

A Binary search tree (BST) is a binary tree data structure. Each node in the tree has a value. The tree is divided into three parts: the left subtree, the right subtree, and the root node. All elements in the left subtree have values less than the root's value. All elements in the right subtree have values greater than the root's value. A BST maintains an ordered structure, which makes it an efficient data structure for searching, inserting, and deleting elements.

**Key aspects:**

* Search: The tree enables an efficient divide-and-conquer approach. Search time complexity in a balanced BST is `O(log n)`. Worst case, when the tree is unbalanced, is `O(n)`.

* Insert: Inserting an element involves finding the correct place for the element based on its value and then adding it as a leaf node. Insertion time complexity is `O(log n)` on average in a balanced tree.

* Delete: Deleting an element can be more complex than insertion because you need to maintain the binary search tree property. It involves cases where the node to be deleted has zero, one, or two children. Delete time complexity is `O(log n)` in a balanced tree.

* Traverse: You can traverse a BST in various orders, including in-order (ascending order), pre-order, and post-order. In-order traversal of a BST gives you a sorted list of elements.

* Balance: To ensure efficient operations, keep the tree balanced. There are self-balancing binary search tree data structures like AVL trees and Red-Black trees.
