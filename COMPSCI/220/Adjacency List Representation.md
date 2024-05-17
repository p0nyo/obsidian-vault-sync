---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
Adjacency Lists are better for sparse graphs
![[Pasted image 20240502144325.png|200]]
- Lists all the outneighbours for each node
	- 0: 2
	- 1: 0, 2
	- 2: 0
- Could also remove the headers for each row
	- 2
	- 0, 2
	- 0
- This representation is sorted by convention
In a file format:
- (order of the graph, how many nodes)
- (0th node out-neighbours)
- (1st node out-neighbours)
- (2nd node out-neighbours)
- (nth node out-neighbours)
- ('0' to end the file)