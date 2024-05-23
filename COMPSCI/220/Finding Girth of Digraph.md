---
tags:
  - compsci
  - math
links:
  - "[[Girth]]"
---
- Uses BFS
Finding the directed girth
1. Run BFS starting `v` 
2. When back arc `(x,v)` is found, `v...xv` is a cycle of length `d[x] + 1`
3. Return length
4. Run for all the nodes present in the digraph and return the minimum length
###### Back Arc Identification
- If `(v,w)` is a ==*back arc*==, `colour[w] = black` and `d[w] <= d[v] - 1
- Can also check if neighbour node = starting node
##### Running Time
$$O(n(n+m))$$