---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
##### Weighted Digraph (G,C)
`G` -> Graph
`C` -> C is a function that takes an arc and maps it to a real number (the cost of using arc `(u,v)`)
![[Pasted image 20240523181712.png|200]]
Formal Writing:
- C(0,2) = 3, C(1,0) = 1
###### Adjacency Matrix Representation
![[Pasted image 20240523181943.png|200]]
- Replacing the 1's in the matrix with the weight of the arc]
- If 0 happens to be a legal weight for an arc, then will have to use -1 or null to represent the absence of an arc
###### Adjacency List Representation
![[Pasted image 20240523182140.png|200]]
*(bottom representation)*
- Stating the weight of the arc right after the neighbour is stated
##### Definitions