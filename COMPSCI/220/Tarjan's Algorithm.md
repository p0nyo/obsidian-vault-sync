---
tags:
  - compsci
  - math
links:
  - "[[Connectivity]]"
---
![[Pasted image 20240523172624.png]]
- From graph `G` make new graph, `H` where `c1,c2...ck` are all the strong components of graph `G`, which become the nodes of graph `H`
- The arcs are all pointing in one direction meaning the graph is also a DAG
- 
![[Pasted image 20240523172845.png]]
- From graph `Gr` can make new graph, `Hr`
- Topological order of graph `H` from using DFS on graph `G` and listing the node done times in reverse
	- `Ck, Ck-1...C2, C1`
 - Loop through the C stages, producing a search forest as a result, which would correspond to the strong components of graph `G`
### Algorithm
1. Run DFS on graph `G` and record the done times for all nodes
2. List nodes of `G` in reverse order of done times
3. Run DFS on `Gr` choosing starting nodes in the order of the node list from step 2
4. Produces forest `Fr`, where trees correspond to the strong components of `G` 
![[Pasted image 20240523175749.png|250]]
##### Running Time
$$O(n+m)$$
