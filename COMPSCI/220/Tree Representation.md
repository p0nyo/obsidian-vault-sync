---
tags:
  - compsci
  - math
links:
  - "[[Digraphs]]"
---
For special types of graphs that can be represented in a tree format
- This will improve storage and access time
How to store a general tree in an array:
- A general rooted tree of n nodes can be stored in an array `pred` of size `n`
- `pred[i]` is the parent of node `i`
- Root has no parent so assign it null or `-1` if we number nodes from `0` to `n-1` in the usual way 
- This is a form of adjacency list but using in-neighbours instead of out-neighbours
`pred = [-1,0,0,1,2,2,2,3]`
![[Pasted image 20240502154855.png|200]]
- The nodes are the indexes