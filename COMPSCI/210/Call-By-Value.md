---
tags:
  - c
  - compsci
links:
  - "[[Call-By-Reference]]"
---

```C
#include <stdio.h>

void swap(int i, int j) {
	int temp;
	temp = i;
	i = j;
	j = temp;
}

int main() {
	int a = 12, b = 13;
	printf("Initial values:\n");
	printf("a = %d b = %d\n\n", a, b);
	swap(a, b);
	printf("After swap2:\n");
	printf("a = %d b = %d\n\n", a, b);

}
```
- a and b will remain the same because a new memory address was created for them instead of changing the original one
