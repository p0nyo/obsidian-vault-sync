---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
![[Pasted image 20240510160949.png|300]]
- White: Nodes that haven't been visited
- Grey: Nodes that have been visited but not their outneighbours
- Black: Nodes that have been visited including their outneighbours
![[Pasted image 20240510161251.png|200]]
1. Graph starts empty, choose any white node
	- Choose `node 0`  and colour grey
2. Now go to its' white outneighbours
	- Go to `node 1`
3. Now choose a grey node
	- Choose `node 0` 
4. Now go to its' white outneighbours
	- Go to `node 3` and colour grey
	- Colour `node 0` black since all outneighbours have been reached
	-  ![[Pasted image 20240510163115.png|100]]
5. Now choose the grey node
	 - Choose `node 1`
6. Now go to its' white outneighbours
	- Go to `node 2` and colour grey
7. Now everything in the graph is white
	-  ![[Pasted image 20240510163310.png|100]]

###### Function: Traverse
![[Pasted image 20240517144124.png|200]]
- Keeps track of two arrays, colour and pred (predecessor)
- For each node in the digraph, if the colour is white, then call the visit function 
###### Function: Visit
![[Pasted image 20240517144623.png|200]]
- Colour the visited node with grey, then make the predecessor null as this was the first node picked in the current visit traversal
- While there is a grey node, choose a grey node, if it has a white neighbour, then choose it
- If there are no white neighbours, then colour the node black
![[Pasted image 20240517145206.png|200]]
![[Pasted image 20240517145314.png|200]]
- [[Search Forest Proofs|Search Forest]]
##### Running Time
![[Pasted image 20240517150656.png]]
