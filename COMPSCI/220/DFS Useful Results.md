---
tags:
  - compsci
  - math
links:
  - "[[Depth First Search (DFS)]]"
---
##### Ancestor Relationships
Let `v`, `w` are a part of digraph `G` and supposed that `seen[v]` < `seen[w]`
- If `v` is an ancestor of `w` in digraph `G`, then:
	- $$seen[v]<seen[w]<done[w]<done[v]$$
- If `v` is not an ancestor of `w` in digraph `G`, then:
	- $$seen[v]<done[v]<seen[w]<done[W]$$
##### Arc Classification
Let `v`, `w` are a part of digraph `G` 
- `(v,w)` is a tree or forward arc only if:
	- $$seen[v]<seen[w]<done[w]<done[v]$$
- `(v,w)` is a back arc only if:
	- $$seen[w]<seen[v]<done[v]<done[w]$$
- `(v,w)` is a cross arc only if:
	- $$seen[w]<done[w]<seen[v]<done[v]$$
	- 
