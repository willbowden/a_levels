# Lists
- A **list** is an abstract data type consisting of a number of items in which the same item may occur more than once. The list is sequenced so we can refer to the first, second, etc item and we can also refer to the last element of the list. 
- It can be used, for example, to implement a queue, stack or tree.

### Operations On Lists

| Operation         | Description                          | Return Value |
| ----------------- | ------------------------------------ | ------------ |
| isEmpty()         |                                      | None         |
| append(item)      | Adds item to end of list             | None         |
| remove(item)      | Removes first occurrence of an item  | None         |
| search(item)      | Search for item in a list            | Bool         |
| length()          | Return number of items               | Int          |
| index(item)       | Return positoin of item              | Int          |
| insert(pos, item) | Insert item at position              | None         |
| pop()             | Remove and return last item in list  | List Item    |
| pop(pos)          | Remove and return item from position | List Item    | 

- An ordered list can be implemented using a **linked list**.
- A **linked list** is where pointers are used to denote the order of items in the list, with pointers being dynamically updated if/when memory is pulled from / returned to the **heap**.
