Theory:

Queue is a data structure in which the elements are added at one end, called the rear, and deleted from the other end, called the front. It is a First In First Out data structure (FIFO). The rear of the queue is accessed whenever a new element is added to the queue, and the front of the queue is accessed whenever an element is deleted from the queue. The middle elements in a queue are inaccessible even if queue elements are sorted in an array unlike a stack.

There are two basic operations which can be implemented on the linked queues. The operations are Insertion and Deletion.
Insertion operation:
The insertion operation append the queue by adding an element to the end of the queue. The new element will be the last element of the queue. There can be the two scenario of insertion into the linked queue.

enQueue(value) - Inserting an element into the Queue
We can use the following steps to insert a new node into the queue...

Step 1 - Create a newNode with given value and set 'newNode ? next' to NULL.
Step 2 - Check whether queue is Empty (rear == NULL)
Step 3 - If it is Empty then, set front = newNode and rear = newNode.
Step 4 - If it is Not Empty then, set rear ? next = newNode and rear = newNode.

deQueue() - Deleting an Element from Queue
We can use the following steps to delete a node from the queue...

Step 1 - Check whether queue is Empty (front == NULL).
Step 2 - If it is Empty, then display "Queue is Empty!!! Deletion is not possible!!!" and terminate from the function
Step 3 - If it is Not Empty then, define a Node pointer 'temp' and set it to 'front'.
Step 4 - Then set 'front = front ? next' and delete 'temp' (free(temp)).

Insertion Operation:
In the first scenario, we insert element into an empty queue. In the second case, the queue contains more than one element. With each insertion the position of REAR is incremented by 1. In linked list implementation of a queue a new element is always added at the tail of the list and d-eleted from the head of the linked list.  The essential condition which is checked before insertion in a linked queue is overflow.

Deletion operation:
Deletion operation removes the element that is first inserted among all the queue elements. There are again two cases that whether the list is empty or the list contains some elements. With each deletion the position of FRONT is incremented by 1. The essential condition which is checked before insertion in a linked queue is overflow.
