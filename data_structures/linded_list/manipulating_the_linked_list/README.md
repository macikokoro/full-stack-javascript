# Manipulating a Linked List

**Node Insertion**

First we need a helper function that searches through the linked list looking for specified data, when this data is found, the function returns the node storing the data. This function is also a good example of moving through a linked list.

The function is built as follows.

* Create a new node and assign it as the head node.
* Loop through the linked list, from one node to the next when the current node's property is not equal to the data we are looking for.
* When this data is found return the node storing the data.
* If the data isn't found return null.

```text
function find(item) {
  var currentNode = this.head;
  while (current.element != item) {
    currentNode = currentNode.next;
    }
    return currentNode;
  }
```

The insert function.

