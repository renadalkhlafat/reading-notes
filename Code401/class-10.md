# Stacks and Queues

## What is a Stack 
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

+ FILO : First In Last Out
+ LIFO : Last In First Out
+ Stack terminology:
    - Push - Nodes or items that are put into the stack are pushed
    - Pop - Nodes or items that are removed from the stack are popped. 
    - Top - This is the top of the stack.
    - Peek - When you peek you will view the value of the top Node in the stack
    - IsEmpty - returns true when stack is empty otherwise returns false.

![stack](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)


## What is a Queue
A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO)

![queue](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2014/02/Queue.png)

- LILO : Last In Last Out
- FIFO : First In First Out
+ Queue terminology:
    - Enqueue - Nodes or items that are added to the queue.
    - Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an  exception will be raised.
    - Front - This is the front/first Node of the queue.
    - Rear - This is the rear/last Node of the queue.
    - Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
    - IsEmpty - returns true when queue is empty otherwise returns false.

## Operations on Queue: 

- Enqueue: Adds an item to the queue. If the queue is full, then it is said to be an Overflow condition. 

- Dequeue: Removes an item from the queue. The items are popped in the same order in which they are pushed. If the queue is empty, then it is said to be an Underflow condition.

- Front: Get the front item from queue. 
- Rear: Get the last item from queue. 

## Time Complexity :
|Operations |  Complexity |
| ------------ | -------------|
| Enque(insertion) |  O(1)|
| Deque(deletion)  | O(1) |
| Front(Get front) | O(1) |
| Rear(Get Rear)   | O(1) |