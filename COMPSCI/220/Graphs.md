---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
$$G=(V,E)$$
- Graphs are a pair of two sets
	1. A non-empty vertex set
	2. A set of edges represented as unordered pairs of the end vertices
![[Pasted image 20240502131849.png|200]]
#### Example
$$V=\{0,1,2,3,4\}$$
$$E=\{\{0,1\},\{0,3\},\{1,2\}, \{1,3\},\{1,4\},\{2,4\}\}$$
*Definitions*
- For the set {0,1}, 0 and 1 are **neighbours**
- **Order** (n) is the magnitude of |V|
	- Example above, n = 5
- **Size** (m) is the magnitude of |E|
	- Example above, m = 6
- **Degree** is the number of neighbours that a vertex has
*notes*
- Graph of n order will always have 0 to n-1 nodes
- Cannot have repeated elements
- Maximum number of edges in a graph with order, n:
$$Maximum\ m=(n(n-1))/2$$
$$\in\ means\ is\ an\ element\ of$$