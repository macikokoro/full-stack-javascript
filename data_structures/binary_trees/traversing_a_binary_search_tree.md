# Traversing a Binary Search Tree

Our previous BST class can only insert nodes into the tree. In order to be able to display the data in different orders, we need to able to traverse the tree.

There are three traversal functions used with BSTs: inorder, preorder, postorder.

**inorder:** visits all of the nodes of a BST in ascending order of the node key values.

**preorder:** visits the root node first, followed by the nodes in the subtrees under the left child of the root node, followed by the nodes in the subtrees under the right child of the root node.

**postorder:** visits all the child nodes of the left subtree up to the root node, and then visits all of the child nodes of the right subtree up to the root node.

**Inorder traversal function**

```text
function inOrder(node) {
  if (node !== null) {
    inOrder(node.left);
    putstr(node.show() + " ");
    inOrder(node.right);
  }
}
```

**Test**

```text
load("bst.js");
var nums = new BST();
nums.insert(23);
nums.insert(45);
nums.insert(16);
nums.insert(37);
nums.insert(3);
nums.insert(99);
nums.insert(22);
nums.inOrder(nums.root);
```

The output would be: Inorder traversal: 3 16 22 2 3 37 45 99

