---
tags:
  - compsci
  - math
links:
  - "[[Topological Sort]]"
---
```python
while V(G) is not empty
	Find u, a source in G
	Place u next in ordering
	Remove u from G

```
- Keep finding sources until none left
#### Running Time
$$O(n+m)$$