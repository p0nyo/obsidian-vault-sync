---
tags:
  - c
  - compsci
links:
  - "[[Call-By-Value]]"
---

```C
#include <stdio.h>

void swap(int* i, int* j) {
	int temp;
	temp = *i;
	*i = *j;
	*j = temp;
}

int main() {
	int a = 12, b = 13;
	printf("Initial values:\n");
	printf("a = %d b = %d\n\n", a, b);
	swap(&a, &b);
	printf("After swap2:\n");
	printf("a = %d b = %d\n\n", a, b);
}
```
- The addresses of a and b are put into the swap function instead of the values
- \*i is pointing at the address, which means it will manipulate the memory address itself