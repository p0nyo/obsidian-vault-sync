---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
Graph is bipartite if the vertices of graph `G` can be partitioned into two non-empty disjoint sets, `V0` and `V1` such that each edge has one endpoint in `V0` and one in `V1`
![[Pasted image 20240523180725.png|200]]
- There are no edges going from `black` to `black` and there are no edges going from `white` to `white`
##### K-Colouring
- When a graph `G` can be partitioned into `k` nonempty disjoint subsets such that edge of `G` joins two vertices in different subsets
	- e.g Tripartite
##### Proving Bipartite Graphs
- If it a graph doesn't contain an odd-length cycle
- Perform a BFS on graph `G` and colour nodes depending on their distance away from the starting node
![[Pasted image 20240523181207.png|200]]
- For a graph with node `u` and node `v`, if there is an arc between them, then it is an odd-length cycle
$$ 2(d[u]) + 1$$
