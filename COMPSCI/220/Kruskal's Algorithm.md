---
tags:
  - compsci
  - math
links:
  - "[[Prim's Algorithm]]"
---
- Repeat until the subgraph is a spanning tree
- Add the minimum weight edge to the subgraph that is not already used such that
	- Adding the edge does not create a cycle
- Same as Prim's Algorithm but the subgraph does not have to remain connected
![[Pasted image 20240612174546.png|200]]
- Look at the weights in the graph starting from weight = 1
#### Running Time
$$O(mlogn)$$

