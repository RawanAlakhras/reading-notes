# Trees

* Type of tree:

1. Binary Trees
2. Binary Search Trees
3. K-ary Trees.

## Common Terminology

* Node - A Tree node is a component which may contain it’s own values, and references to other nodes
* Root - The root is the node at the beginning of the tree
* K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
* Left - A reference to one child node, in a binary tree
* Right - A reference to the other child node, in a binary tree
* Edge - The edge in a tree is the link between a parent and child node
* Leaf - A leaf is a node that does not have any children
* Height - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals

* There are two categories of traversals when it comes to trees:

1. Depth First
2. Breadth First

## Depth First

* use stack 
* three methods for depth first traversal:

1. Pre-order: root >> left >> right
2. In-order: left >> root >> right
3. Post-order: left >> right >> root

## Breadth First

* use queue
* Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

## Binary Tree Vs K-ary Trees

* Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).
* If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree.

