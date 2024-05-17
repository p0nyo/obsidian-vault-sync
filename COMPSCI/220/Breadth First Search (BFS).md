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
![[Pasted image 20240517165525.png|200]]
1. Start BFS at `node 0`
	- Find all white neighbours that `node 0` , starting from a lower