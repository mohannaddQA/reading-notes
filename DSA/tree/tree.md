# | TREE |

### Analogy

Imagine you have a hierarchical structure of interconnected branches, where each branch can have multiple sub-branches, and so on. This interconnected structure resembles a tree, with the main trunk as the root and branches extending from it. This analogy helps us understand the concept of trees in computer science.

### Definition

A tree is a non-linear data structure that represents a hierarchical structure. It consists of nodes connected by edges, where each node can have zero or more child nodes. The topmost node is called the root, and the nodes at the bottom with no child nodes are called leaves.

### Operations

- Insertion: Add a new node to the tree.
- Deletion: Remove a node and its corresponding subtree from the tree.
- Traversal: Visit each node in the tree in a specific order.

### Key Concepts

- Nodes: Represent elements or data in the tree.
- Root: The topmost node of the tree.
- Parent and Child: Nodes connected by edges, where the parent node has child nodes, and child nodes have a parent node.
- Sibling: Nodes that have the same parent.
- Leaf: Nodes with no child nodes.
- Subtree: A smaller tree rooted at a particular node.
- Depth: The level or distance of a node from the root.
- Height: The maximum depth of any node in the tree.

### Common Applications

- Representing hierarchical data, such as file systems, organization structures, or family trees.
- Searching, sorting, and organizing data efficiently, such as in binary search trees or heaps.

### Tree Implementation

Trees can be implemented using various techniques, including arrays, linked lists, or dynamically allocated nodes.

- Arrays can be used to represent complete binary trees where the index corresponds to a specific node.
- Linked lists can be used to represent arbitrary trees where each node contains references to its child nodes.

### Time Complexity

The time complexity of tree operations can vary depending on the specific implementation and the type of tree structure.

- Insertion: O(1) to O(log n), depending on the type of tree.
- Deletion: O(1) to O(log n), depending on the type of tree.
- Traversal: O(n), where n is the number of nodes in the tree.

### Visualization:

![visualization](./vis.png)
