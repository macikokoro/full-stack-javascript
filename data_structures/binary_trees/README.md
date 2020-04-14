# Binary Trees

A binary tree is a tree structure such that each node, apart from the final nodes, have exactly two children. This type of non-linear data structure is used to store data in a hierarchichal manner, for instance lists of data. Binary trees can be searched very quickly \(as opposed to a linked list\) and data can be inserted or deleted very quickly \(as opposed to an array\).

To specify the element of the tree we have to give it two indices - the level or how far down the tree and the node number at that lever - how far to the right the node is.

Each value is associated with a value that takes n bytes to store.

## Anatomy

Trees are made up of a set of nodes connected by edges. A good example would be an organizational chart.

The top of node of a tree is called root node. If a node is connected to other nodes below it, the preceding node is called the parent node, and the nodes following it are called child nodes.

A node can have zero, one, or more child nodes connected to it. A node without any child nodes is called a leaf node.

In the case of binary trees the number of child nodes is restricted to no more than two.

It is possible to travel from one node to other nodes that are not directly connected. The series of edges needed to get from one node to the other are called a path. Visiting all the nodes in a tree in some particular order is known as a tree traversal.

A tree can be broken down into two levels. The root node is at level 0, its children are at level 1, those nodes' children are at level 2, and so on. We can define the depth of a tree as the number of layers in the tree.

Each node in a tree has a value associated with it. This value is referred as the key value.

## Binary Tree Efficiency

Because of their limiting nature, no more than two children, it is possible to write efficient programs for inserting, searching, and deleting data.

## Tree Lingo

The child nodes of a parent node are referred to as the left node and the right node.

