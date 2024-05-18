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
	- Find all white neighbours that `node 0` , starting from a lower index
2. Then choose node that has been grey the longest amount of time, `node 1`
	- Then go from `node 1`
##### Function: BFS
![[Pasted image 20240518191931.png|200]]
- Initialise three arrays, colour, pred and d (depth)
- Initialise a Queue ADT
- For loop through nodes in the digraph, if it is white then BFSVisit
##### Function: BFSVisit
![[Pasted image 20240518192148.png|200]]
- Colour visited node grey
- Enter the depth, 0, into the depth array corresponding to node `s`
- Queue node into the queue
- While the Queue is not empty, peek into the queue and for loop through each of the node's neighbours
- Colour neighbour grey and put down the predecessor
- Then set the depth travelled to be the predecessor's depth from `node 0 + 1`
- If no more neighbours then delete node from Queue and colour node black