---
tags:
  - compsci
  - math
links:
  - "[[General Graph Traversal Algorithm]]"
---
![[Pasted image 20240510160949.png|300]]
- White: Nodes that haven't been visited
- Grey: Nodes that have been visited but not their outneighbours
- Black: Nodes that have been visited including their outneighbours
![[Pasted image 20240517152416.png|200]]
1. Graph starts empty
	- Start with node with the lowest index
	- Traverse from `node 0` until there are no more white neighbours to traverse to
	- When traversing, always use the lowest index white out-neighbour
![[Pasted image 20240517152522.png|200]]
2. Then choose all grey neighbours and if they have no white out-neighbours then colour them black
![[Pasted image 20240517152750.png|200]]
- If there is a white out-neighbour then travel to that out-neighbour
- In this case `node 6` was a white out-neighbour of `node 5` and `node 3` was a white out-neighbour of `node 1`
##### Function: DFS
![[Pasted image 20240517153039.png|200]]
- Initialise 4 different lists
- Initialise a stack
- Initialise time variable to zero
- Loop through the nodes of the digraph, if it is white then DFS visit it
##### Function: DFSVisit
![[Pasted image 20240517163450.png|200]]
- Colour the visited node grey, seen time set to the current time variable and increment time by 1
- Push the node into the stack
- While the stack is not empty, peek at the top value, `U`
- If `U` has a white neighbour, `V`, then colour it grey, set the predecessor to `U` and set seen time to current time and increment time by 1,
- If there are no white neighbours then pop from the stack, colour the node black and enter current time into done time list
##### Function: RecursiveDFSVisit
![[Pasted image 20240517163843.png|200]]
- Traversal can also be done recursively 


##### Code
```python
# Recursive
def dfs(digraph):
# define function in function to access all the defined arrays
	def rdfsvisit(node, digraph):
		colour[node] = 'g'
		seen[node] = time[0]
		time[0] += 1
		for neighbour in digraph[node]:
			if colour[neighbour] == 'w':
				pred[neighbour] = node
				rdfsvisit(neighbour, digraph)
		colour[node] = 'b'
		done[node] = time[0]
		time[0] += 1
colour = ['w']*len(digraph)
pred = [-1]*len(digraph)
seen = [0]*len(digraph)
done = [0]*len(digraph)
time = [0]
# print(colour, pred, seen, done, time)
for node in range(len(digraph)):
	if colour[node] == 'w':
	rdfsvisit(node, digraph)
# print(colour, pred, seen, done, time)
treearc = len([i for i in pred if i != -1])
print(str(treearc) + ' ', end = '')
crossarc = 0
for node in range(len(digraph)):
	for neighbour in digraph[node]:
		if seen[neighbour] < done[neighbour] < seen[node] < done[node]:
crossarc += 1
print(crossarc)

```


##### Running Time
![[Pasted image 20240517153003.png]]
- Running time of the graph if using adjacency lists