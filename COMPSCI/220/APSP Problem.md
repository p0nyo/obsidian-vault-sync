---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
**A**ll **P**airs **S**hortest **P**ath (APSP) Problem
- Given a weighted digraph, we must determine for each `u,v` the weight of the minimum path from `u` to `v`
**Dijsktra**
- If the weights were non-negative: Dijsktra from each of the nodes, running time:
$$O(nm logn)$$
![[Pasted image 20240612161928.png|200]]
- Sparse diagram: $$O(n^2logn)$$
- Dense diagram: $$O(n^3logn)$$
**Bellman-Ford**
- Bellman-Ford is already O(nm), therefore to run it n times, it is: $$O(n^2m)$$
