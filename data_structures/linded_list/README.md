# Linked List

Arrays are not always the optimal solution for organizing data. Whenever the operations performed in an array are too slow for practical use, it is usually best to use a linked list. They can be used in almost any case where a one-dimensional array is used, except when random access to the list is needed. An array is the best choice in this situation.

A linked list is a collection of nodes or objects, linked to a successor node in the list using and object reference. This references are called links.

Linked list elements unlike array elements are not referenced by their position, rather by their relationship to the other elements of the linked list. For instance Robin follows Batman.

The beginning of a linked list is marked with a head node and the end with a null node.

Header -&gt; Alfred -&gt; Robin -&gt; Batman -&gt; Null

**Inserting a new node** in a linked list requires pointing the link before the inserted node to the new node, and the new node's link is set to the node the previous node was pointing to before insertion.

**Removing nodes** the link of the node before the removed node is redirected to point to the node tehremoved kinothe removed node was pointing to, while also pointing the removed node to null.

