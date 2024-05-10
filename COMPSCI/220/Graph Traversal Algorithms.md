---
tags:
  - compsci
  - math
links:
  - "[[Graph ADTs]]"
---
![[Pasted image 20240510160949.png|300]]
- White: Nodes that haven't been visited
- Grey: Nodes that have been visited but not their outneighbours
- Black: Nodes that have been visited including their outneighbours
![[Pasted image 20240510161251.png|200]]
1. Graph starts empty, choose any white node
	- Colour `node 0` grey
2. Now choose a grey node
	- Choose `node 0` 
3. Now go to its' white outneighbours
	- Go to `node 1`
4. Now choose a grey node
	- Choose `node 0` and colour grey
5. Now go to its' white outneighbours
	- Go to `node 3` and colour grey
	- Colour `node 0` black since all outneighbours have been reached
	-  ![[Pasted image 20240510163115.png|100]]
6. Now choose the grey node
	 - Choose `node 1`
7. Now go to its' white outneighbours
	- Go to `node 2` and colour grey
8. Now everything in the graph is white
	-  ![[Pasted image 20240510163310.png|100]]
	- 


