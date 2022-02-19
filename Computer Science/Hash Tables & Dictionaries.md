# Hash Tables & Dictionaries
### Hashing
- For large collections of data, individual records can be accessed quickly by holding an index of the physical address on the file where the data is held. 
- This index is created using a **hashing algorithm**, which takes a value, applies some mathematical functions on it, and creates an address.
- If two values result in the same hash, they are known as **synonyms**. Attempting to put two values in the same address causes a **collision**.
- In the case of a collision, often the item will be stored in the next available space.

### Hash Tables
- A **hash table** is a collection of items stored in such a way that they can quickly be located. The hash table could be implemented as an array or a list with a given size.

### Other Hashing Algorithms
##### Folding Method
- Divide a number into equal parts, then sum them to find the hash.
- If the number exceeds the maximum length of the hash table, further action can be taken, such as dividing by 100 and taking the remainder.

##### Hashing A String
- Use the ASCII code for each character.

### Collision Resolution
- The more items in a table, the more likely a collision becomes.
- The size of a table could be designed so that when all the items are stored, only 70% of the table's cells are occupied.
- **Rehashing** is the process of finding an empty slot when a collision has occurred.
- Usually, slots are checked sequentially until a free one is found, but an alternative method, such as checking every 3 cells, could be used instead.

### Uses Of Hash Tables
- Hash tables are primarily used for efficient lookup.
- For example, to find a person's telephone number given their name, or vice versa.
- They can also be used to store data such as user codes and encrypted passwords that need to be looked up and verified quickly.

### Dictionaries
- Hash tables are used in the implementation of dictionaries.
- A **dictionary** is an abstract data type consisting of associated pairs of items, where a pair consists of a **key** and a **value**. 
