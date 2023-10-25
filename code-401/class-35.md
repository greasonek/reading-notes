# Class 35 Reading Notes

## Graphs

### VOCAB

- **Graph** - non-linear data structure that can be looked at as a collection of *vertices* (nodes) potentially connected by line segments named edges

- **Vertex** - node, can have 0+ adjacent vertices

- **Edge** - connection between 2 nodes

- **Neigbor** - neigbor of a node is it's adjacent nodes (connected via an edge)

- **Degree** - degree of a vertex is the number of edges connected to that vertex

- **Undirected Graph** - graph where edges are undirect or bi-directional (graph does not have any direction)

![undirected-graph](./imgs/Screenshot%202023-10-24%20at%209.09.08 PM.png)

- **Directed Graph** - (*Digraph*) has direction, specified direction of which node to be referenced next

![direct-graph](./imgs/Screenshot%202023-10-24%20at%209.10.03 PM.png)

- **Complete Graph** - all nodes connect to other nodes

- **Connected Graph** - all vertices have at least one edge; a *tree* is a form of a connected graph

- **Undirected Graph** - graph where some vertices don't have edges

- **Cycle** - When a node can be traversed through and possibly end up back at itself

- **Acyclic** - (*DAG*) directed graph without cycles; *Trees* are an example of this

- **Cyclic** - A graph that has cycles - starts and ends at the same vertex

- **Adjacency Matrix** - represented through 2D array; each row and column represent a vertex, the elements of each must add up to 1 if they're connected or a 0 if not; can be sparce or dense

![adjacent-matrix](./imgs/Screenshot%202023-10-24%20at%209.19.17 PM.png)

- **Adjacency List** - most common way to represent graphs; collection of linked lists or arrays hat lists of all vertices are connected

![adj-list](./imgs/Screenshot%202023-10-24%20at%209.21.16 PM.png)

- **Weighted Graph** - graph with numbers assigned to its edges; (numbers are the weights)

- Traversals - can be breadthFirst or depthFirst
  
  - breadthFirst - like that of a tree; need to keep track of nodes that have been visited to prevent an infinite loop in the case of a cyclic graph; uses a queue to visit all children closest to the head node first moving out

  - depthFirst - uses a Stack to visit all children in a subtree; push the root node into the stack and mark it as visited, while loop - pop the top node off and check neighbors then push it to the stack
  