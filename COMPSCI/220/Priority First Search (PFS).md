---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
A generalisation of DFS and BFS
- The smaller the key, the higher the priority, e.g node 0 looking at all neighbours before visiting deeper 
1. Rule for choosing grey node is to choose one with the smallest key
##### Mimicking BFS
- Set the key for the node `v` to be the time that `v` turns grey, it will always remain as the lowest key until it turns black
##### Mimicking DFS
- Set the key for the node `v` to be `-seen[v]`, so that the most recently seen node has the lowest key
##### Function: PFS
![[Pasted image 20240519160219.png|200]]
##### Function: PFSVisit
![[Pasted image 20240519160253.png|200]]
