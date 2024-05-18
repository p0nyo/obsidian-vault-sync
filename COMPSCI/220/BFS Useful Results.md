---
tags:
  - compsci
  - math
links:
  - "[[Breadth First Search (BFS)]]"
---
Suppose we are performing a BFS on a digraph, G
- Let `(v,w)` be apart of a digraph and suppose we have chosen the grey node `v`
1. If `(v,w)` is a ==*tree arc*==, `colour[w] = white` and `d[w] = d[v] + 1`
2. If `(v,w)` is a ==*back arc*==, `colour[w] = black` and `d[w] <= d[v] - 1`
3. There are no *==forward arcs==*
4. If `(v,w)` is a ==*cross arc:*==
	1. `d[w] < d[v]-1` & `colour[w] = black`
	2. `d[w] = d[v]` & `colour[w] = black or grey`
	3. `d[w] = d[v]-1` & `colour[w] = black or grey`