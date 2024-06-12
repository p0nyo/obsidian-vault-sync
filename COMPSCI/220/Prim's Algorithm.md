---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
![[Pasted image 20240612165925.png|200]]
- Repeat until the subgraph is a spanning tree
- Add the minimum weight edge to the subgraph that is not already used such that
	- Adding the edge does not create a cycle
	- The subgraph remains connected
![[Pasted image 20240612170453.png|200]]
- Choosing the lowest weight for each arc when creating the sub-graph 

#### Running Time
$$O(mlogn)$$
