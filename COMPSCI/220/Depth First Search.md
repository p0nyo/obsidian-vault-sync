---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
![[Pasted image 20240510160949.png|300]]
- White: Nodes that haven't been visited
- Grey: Nodes that have been visited but not their outneighbours
- Black: Nodes that have been visited including their outneighbours
![[Pasted image 20240517152416.png|200]]
1. Graph starts empty
	- Start with node with the lowest index
	- Traverse from `node 0` until there are no more white neighbours to traverse to
	- When traversing, always use the lowest index white out-neighbour
![[Pasted image 20240517152522.png|200]]
2. Then choose all grey neighbours and if they have no white out-neighbours then colour them black
![[Pasted image 20240517152750.png|200]]
- If there is a white out-neighbour then travel to that out-neighbour
- In this case `node 6` was a white out-neighbour of `node 5` and `node 3` was a white out-neighbour of `node 1`
##### Function: DFS
![[Pasted image 20240517153039.png|200]]
- Initialise 4 different lists
- 







##### Running Time
![[Pasted image 20240517153003.png]]
- Running time of the graph if using adjacency lists