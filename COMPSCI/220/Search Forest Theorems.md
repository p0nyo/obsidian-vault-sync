---
tags:
  - compsci
  - math
links: []
---
![[Pasted image 20240517145206.png|200]]
##### Theorems
Suppose `F` is a search forest resulting from a traversal
1. `T1` and `T2` in `F`, if `T1` was explored before `T2`, then no arcs go from `T1` to `T2`
2. In a graph, there are no edges between `T1` and `T2`
3. If `V` -> `W` in a tree, if we visit `V` before `W`, then `V` and `W` are in the same tree
4. If `V` -> `W` are in the same tree `T`, then all nodes on any path from `V` to `W` are also in `T`