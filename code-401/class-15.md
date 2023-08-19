# Class 15 Reading

> Trees

### Vocab/Definitions List

- **Node**: contains its own values and references to other nodes

- **Root**: node at the beginning of the tree

- **K** - specifies max # of children any node may have in a tree; binary tree --> k = 2

- **Left**: reference to one child node in a binary tree

- **Right**: reference to other child node

- **Edge**: link between a parent and a child node

- **Leaf**: node with no children

- **Height**: number of edges from the root to the furthest tree

- **Traversals**: traversing allows us to search for a node, print contents of the tree, etc.

- **Depth First**: traversal prioritizing going through the height of the tree first
  - *Pre-order*: root>>left>>right
  - *In-order*: left>>root>>right
  - *Post-order*: left>>right>>root

- **Recursion**: rely on a call stack to navigate back up the tree when we've reached the end of a sub-path

- **Breadth First**: traversal iterates through the tree by going through each level of the tree node by node

- **Binary Tree**: restricts number of nodes to 2; no specific sorting order

- **K-ary Tree**: Tree where nodes are able to move more than 2 child nodes