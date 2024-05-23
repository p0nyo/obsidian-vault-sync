---
tags:
  - compsci
  - math
links:
  - "[[Topological Sort]]"
  - "[[Sub-Digraphs]]"
---
A digraph that has no cycles.
- A digraph is acyclic if there are no back arcs when a DFS is performed on it
- If the digraph `G` is a DAG, then listing the nodes in reverse order from DFS of its' finishing times is a topological sort of `G`
	![[Pasted image 20240519175214.png|200]]
	