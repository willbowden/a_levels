# Stacks
- A **stack** is a **Last In, First Out (LIFO)** data structure.
- Stacks are used in calculations, and hold return addresses when subroutines are called.
- They are also used for undo buttons.
- A stack can be implemented as static or dynamic, and is usually done with an array along with a pointer to the top of the stack and a variable holding the maximum size of the stack.

### Operations On A Stack
| Operation  | Description                      |
| ---------- | -------------------------------- |
| push(item) | Add new item to top              |
| pop()      | Remove and return item from top  |
| peek()     | Return without removing top item |
| isEmpty()  |                                  |
| isFull()   |                                  | 

### Overflow & Underflow
- An attempt to push an item onto a full stack will cause an **overflow error**.
- If the pointer is -1, the stack is empty and an **underflow error** would occur should someone try to pop an item.

### The Call Stack
- The call stack is covered in Chapter 8 - Algorithms


