---
tags:
  - math
  - compsci
links:
  - "[[Graphs]]"
  - "[[Graph ADTs]]"
---
$$G = (V,E)$$
- Graphs that have direction
	1. Vertices are now a set of **nodes**
	2. Edges are an ordered set of pairs representing **arcs**

![[Pasted image 20240502133234.png|150]]
#### Example
$$V=\{0,1,2,3,4\}$$
$$E=\{(0,2),(1,0),(1,3),(1,4),(3,4),(4,1)\}$$
*Definitions*
- For the pair (0,2) where 0 -> 2
	- 2 is **adjacent** to 0 and 2 is an **out-neighbour** of 0
	- 0 is an **in-neighbour** of 2
- **Order** (n) is the magnitude of |V|
	- Example above, n = 5
- **Size** (m) is the magnitude of |E|
	- Example above, m = 6
- **Sparse** if a graph is small 
	- O(n)
- **Dense** if a graph is large
	- O(x^2)
- **Out-degree** is the number of arcs leaving a node
	- For graph, u, (u, - )
- **In-degree** is the number of arcs pointing into a node
	- For graph, u, ( - , u)
- **Sink** is a node with out-degree of 0
- **Source** is a node with in-degree of 0
- A **walk** from nodes 1 -> 2 means there is an arc from 1 to 2
	- 3, 4, 1, 0 is a walk from example above
	- **Length of Walk** is the number of arcs involved in a walk
	- A **path** is a walk that has no nodes repeated
	- A **cycle** is when a walk where the first and last nodes are the only repeated ones
- The **distance** is the length of the shortest path from u -> v
	- Length is infinite or undefined if it does not exist

$$d(u,v)$$

*note*s
- Curly brackets for unordered pairs
- Round brackets for ordered pairs
- No loops, cannot node 1 -> node 1
- Maximum number of arcs in a digraph with order n:
$$maximum\ m=n(n-1)$$ ^d3f6c5
