---
tags:
  - compsci
  - math
links:
  - "[[Digraph Representation]]"
---
Adjacency Matrices are better for dense graphs
![[Pasted image 20240502144325.png|200]]
- Form x and y columns of adjacency matrix with the amount of nodes available, len(rows) = len(columns)
$$ \begin{bmatrix}  
0 & 0 & 1\\  
1 & 0 & 1\\
1 & 0 & 0
\end{bmatrix}
$$
- If an arc exists, then write 1, if it doesn't then write 0
- Conventionally, arcs go from y side to x side of the matrix