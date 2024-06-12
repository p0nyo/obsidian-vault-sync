---
tags:
  - compsci
  - math
links:
  - "[[SSSP Problem]]"
---
![[Pasted image 20240612154252.png]]
- Loop `i` from 0 to n-1, which is the number of nodes there are
- For each `i` the algorithm look at each possible arc to see if the cost from travelling from each possible node is shorter than the previous path
#### Running Time
$$O(mn)$$
where `n` is the number of nodes and `m` is the number of arcs
