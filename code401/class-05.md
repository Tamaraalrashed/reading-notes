# Linked Listss
## Linked List
A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.



## Terminology:

1. Linked List - A data structure that contains nodes that links/points to the next node in the list.
1. Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
1. Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

1. Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
1. Next - Each node contains a property called Next. This property contains the reference to the next node.
1. Head - The Head is a reference of type Node to the first node in a linked list.
1. Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

## Traversal
When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

## Traversal Big O
The Big O of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

## Linear data structures

 it means that there is a sequence and an order to how they are constructed and traversed. 

 ## Big O Notation

 it is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function.
