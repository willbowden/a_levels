# Graphs
- A **graph** is a set of **vertices or nodes** connected by **edges or arcs**.
- The edges may be one-way or two-way.
- In an **undirected graph**, all the edges are bidirectional.
- A digraph or directed graph has one-way arcs.
- The edges may be **weighted** to show a cost to traverse from one vertex to another (this is usually distance or time)
- A graph can be implemented using an **adjacency matrix** or an **adjacency list.**

### Adjacency Matrix
- A two-dimensional array can be used to store information about a directed or undirected graph.
- Each of the rows and columns represents a node, and a value stored in the cell at the interesction indicates that there is an edge connecting those nodes. In these cells, the weight of the edge will be stored.
- In an undirected graph, 0 and 1 are used, meaning the matrix will be symmetrical.
- An adjacency matrix is very convenient to work with, but a sparse graph will leave most of the cells empty.
- Also, a large graph will cause a considerable amount of memory wastage.

### Adjacency List
- An adjacency list is a more space-efficient way to implement a sparsely connected graph.
- A list of all the nodes is created, and each node points to a list of all the adjacent nodes to which it is direcly linked.
- The adjacency list can be implemented as a list of dictionaries, with the key in each dictionary being the node and the value the edge weight.
- For unweighted graphs, a list would be used instead of a dictionary.

### Applications Of Graphs
- Graphs can be used to represent computer networks, roads between towns, sequential tasks in a project, states in a finite state machine, or web pages and links.

