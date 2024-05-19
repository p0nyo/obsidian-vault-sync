---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
A topological sort of a digraph `G` is a linear ordering of the nodes in `G`, such that if `u` comes before `v` in the ordering, then the arc `(v,u)` would not exist in `G`
![[Pasted image 20240519161403.png]]
- All the arcs would be going from left to right
- Any cycle in a graph will prevent us from finding a topological sort
##### Proof
![[Pasted image 20240519162105.png]]
- Use