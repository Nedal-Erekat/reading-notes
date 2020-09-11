# Link list:

- data structures: which are the different ways that we can organize our data

One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. 

- non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

![](https://miro.medium.com/max/700/1*Xokk6XOjWyIGCBujkJsCzQ.jpeg)

### Terminology:
Linked List - A data structure that contains nodes that links/points to the next node in the list.
Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
Next - Each node contains a property called Next. This property contains the reference to the next node.
Head - The Head is a reference type of type Node to the first node in a linked list.
Current - The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.