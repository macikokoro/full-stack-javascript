# Implementing a Linked List

Designing a linked list requires the creation of two classes. Number one is a Node class for adding nodes to the list and number two a LinkedList class. This last class will provide functions for inserting, removing and deleting nodes plus displaying the list, and basic housekeeping functions.

**Node Class**

The Node class contains two properties, value, to store the node's data, and nexNode to store a link to the next node in the linked list.

The following is a constructor function that sets the values for the two properties.

```text
function Node(data) {
  this.data = data;
  this.nextNode = null;
}
```

**Linked List Class**

Here we add the functionality for a linked list. We have to include functions that will be able to insert, remove or delete nodes, as well as finding data values in the list.

Here is the constructor function necessary to create a new linked list.

```text
function LinkedList() {
  this.head = new Node("head"); //points null to the first element inserted
  this.find = find;
  this.insert = insert;
  this.remove = remove;
  this.display = display;
}
```

