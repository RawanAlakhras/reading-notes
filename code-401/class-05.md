# Linked Lists

* A Linked List is a sequence of Nodes that are connected/linked to each other. 
* The most defining feature of a Linked List is that each Node references the next Node in the link.
* There are two types of Linked List - Singly and Doubly.
* Linked List - A data structure that contains nodes that links/points to the next node in the list.
* Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
* Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
* Node - Nodes are the individual items/links that live in a linked list. 
* Next - Each node contains a property called Next. This property contains the reference to the next node.
* Head - The Head is a reference of type Node to the first node in a linked list.
* Current - The Current is a reference of type Node to the node that is currently being looked at. 
* One characteristic of linked lists is that they are linear data structures.


## Traversal

* When traversing a linked list, you are not able to use a foreach or for loop.
*  We depend on the Next value in each node to guide us where the next reference is pointing. 
* The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.
* The best way to approach a traversal is through the use of a while() loop. 
* When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

# Traversal Big O

* The Big O of time for Includes would be O(n).
* The Big O of space for Includes would be O(1).

## linear data structures

*  is a sequence and an order to how they are constructed and traversed. 

## non-linear data structures,

* items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

## Memory management

* The biggest differentiator between arrays and linked lists is the way that they use memory in our machines. 
*  when a linked list is born, it doesn’t need 7 bytes of memory all in one place. One byte could live somewhere, while the next byte could be stored in another place in memory altogether! Linked lists don’t need to take up a single block of memory; 

