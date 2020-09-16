# Stacks and Queues
## Stacks
**Stack:** is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.
**Stack common terminology/functions:** 
1. Push (Add)
2. Pop (Remove)
3. Top (refers to the top of the stack)
4. Peek (view the value of the top)
5. isEmpty (returns boolean result)

Stacks follow these concepts: First In Last Out,Last In First Out

In the pushdown stacks only two operations are allowed: push the item into the stack, and pop the item out of the stack. A stack is a limited access data structure - elements can be added and removed from the stack only at the top. push adds an item to the top of the stack, pop removes the item from the top. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top.
## Queue
Common terminology for a queue is
1. Enqueue (Add)
2. Dequeue (Remove)
3. Front (refers to the first Enqueued item/node)
4. Rear (refers to the last Enqueued item/node))
5. Peek (view the value of the Front)
6. isEmpty (returns boolean result)
Queues follow these concepts: First In First Out, Last In Last Out

An excellent example of a queue is a line of students in the food court of the UC. New additions to a line made to the back of the queue, while removal (or serving) happens in the front. In the queue only two operations are allowed enqueue and dequeue. Enqueue means to insert an item into the back of the queue, dequeue means removing the front item. The picture demonstrates the FIFO access. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added. 
