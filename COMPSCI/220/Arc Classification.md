---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
![[Pasted image 20240517145206.png|200]]
- Anything that is not a tree arc, e.g a -> c, can be classified as a the arcs listed below:
##### Forward Arc
- A -> E is a forward arc because E is a descendant of A
##### Back Arc
- E -> A is a back arc because A is an ancestor of E
##### Cross Arc
- B -> E is a cross arc because there is no ancestor or descendant relationship between them
- B -> A is a cross arc because there is no ancestor or descendant relationship between them