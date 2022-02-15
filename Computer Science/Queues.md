# Queues
### Data Types
- **Elementary data types** are built-in types such as integer, real, Boolean and char
- **Composite data types** are made of elementary types, such as string ay or list.
- **Abstract data types** such as queues, stacks, trees and graphs can easily be shown in graphical form. 
- An abstract data type is a logical description of how the data is viewed and the operations that can be performed on it, but how this is to be done is not necessarily known to the user. 
- This is a good example of **data abstraction**, and by providing this level of abstraction we are creating an **encapsulation** around the data, hiding the details of implementation from the user. This is called **information hiding**.

### Queues
- A **queue** is a **First In First Out (FIFO)** data structure. 
- It is an ordered collection of items which are added at the rear of the queue, and removed from the front.
- Queues are used in a variety of applications: 
	- Printer queues
	- Keyboard buffer
	- Simulating real life situations (e.g customers at supermarket)

### Operations On A Queue
	- enQueue(item)    Add new item to rear
	- deQueue(item)    Remove item from front of queue and return it
	- isEmpty()        Check if list is empty (use before removing item)
	- isFull()         Check if list is full (use before adding item)

### Dynamic vs Static
- A **dynamic data structure** has the ability to grow or shrink its size in memory.
- It does this with the aid of the **heap**, which is a portion of memory from which space is automatically allocated or de-allocated as required.

### Linear vs Circular Queues
- In a **linear queue**, when an item is removed from the front, all other items in the queue need to be moved forward one item. With long queues, this can incur significant processing time.
- In a **circular queue**, pointers are used to denote the location of the first and last element of the queue, as well as its length being stored. An item is added after the rear pointer, with the final position wrapping back around to the front of the queue, like a circle.
- A circular queue takes a bit more effort to implement, and is less flexible if the maximum numbe of items is not known in advance, but it does significantly cut down on processing time.

### Priority Queues
- A **priority queue** acts like a queue but the logical order of items within the queue is determined by their priority. 
- A priority queue may, for example, be used in a printer queue, with shorter printing jobs taking higher priority.