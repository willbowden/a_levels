# Trees
- A **tree** is a **connected, undirected graph with no cycles**. 
- Connected means there is always a possible path from one node to another.
- No Cycles means it is not possible to traverse from any node back to the start node without having to traverse the same edge twice.

### Structures Of A Tree
| Structure | Purpose                                                                |
| --------- | ---------------------------------------------------------------------- |
| Node      | Contains the tree data                                                 |
| Edge      | Links two nodes                                                        |
| Root      | Only node that has no incoming edges                                   |
| Child     | The nodes that have incoming edges from the same node                  |
| Parent    | A node is a parent of all the nodes it connects to with outgoing edges |
| Subtree   | A parent and all its child nodes.                                      |
| Leaf node | A node that has no children                                            |

### Binary Search Trees
- A binary tree is a rooted tree in which each node has as maximum of two children. A **binary search tree** holds items in such a way that the tree can be searched quickly and easily for a particular item.
- A binary search tree is constructed by starting at the root node, and if the value is less than the root node, navigate left. Otherwise, navigate right. Once there are no more nodes to navigate, a new node is created in that place with the value. The new node will be placed on the left or right depending on its value.
- Visiting the nodes of a binary tree using **in-order** traversal results in the nodes being printed in ascending order.

### Implementation Of Trees
- Trees can be implemented using an array of records, or three separate arrays. Each node needs to have information on its value, the node left of it, and the node right of it.
- If there is not a child node attached to a node, a pointer of -1 is typically used.
