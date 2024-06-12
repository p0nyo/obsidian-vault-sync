---
tags:
  - compsci
  - math
links:
  - "[[APSP Problem]]"
---
Solves it in time:
$$O(n^3)$$
![[Pasted image 20240612163257.png|200]]
- Looks through the cost matrix
- `x` is the intermediate node
- Checks to see if the path from `u -> v` is shorter than the path from `u -> x -> v`
![[Pasted image 20240612164250.png|200]]

