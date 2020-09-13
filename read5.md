# Linked Lists
A linked list is a sequence of data structures, which are connected together via links.

Linked List is a sequence of links which contains items. Each link contains a connection to another link. Linked list is the second most-used data structure after array. Following are the important terms to understand the concept of Linked List.

* __Link__ − Each link of a linked list can store a data called an element.
* __Next__ − Each link of a linked list contains a link to the next link called Next.
* __LinkedList__ − A Linked List contains the connection link to the first link called First.
## Parts of a linked list
A linked list can be small or huge, but no matter the size, the parts that make it up are actually fairly simple. A linked list is made up of a series of nodes, which are the elements of the list.

The starting point of the list is a reference to the first node, which is referred to as the head. Nearly all linked lists must have a head, because this is effectively the only entry point to the list and all of its elements, and without it, you wouldn’t know where to start! The end of the list isn’t a node, but rather a node that points to null, or an empty value.
## Hey, so, what even is Big O?
Big O Notation is a mathematical function used in computer science to describe how complex an algorithm is — or more specifically, the execution time required by an algorithm. In software engineering, it’s used to compare the efficiency of different approaches to a problem.

With Big O Notation, you express the runtime in terms of how quickly it grows relative to the input, as the input gets arbitrarily large. Essentially, it’s a way to draw insights into how scalable an algorithm is. It doesn’t tell you how fast or how slow an algorithm will go, but instead about how it changes with respect to its input size.
**Developers typically solve for the worst case scenario, Big O,** because you’re not expecting your algorithm to run in the best or even average cases. It allows you to make analytical statements such as, “well, in the worst case scenario, my algorithm will scale this quickly”.
