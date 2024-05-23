---
tags:
  - compsci
  - math
links:
  - "[[Girth]]"
---
- Uses BFS
Idea: First find the shortest cycle through the vertex, `V`
1. Perform BFSVisit starting at `V`
2. If current vertex is `x` and crosses arc `{x,y}` then `v...xy...v` is a cycle
3. Length of the cycle is:
$$l =d[x]+d[y]+1$$![[Pasted image 20240523162705.png|100]]
##### Running Time
$$O(n(n+m))$$
