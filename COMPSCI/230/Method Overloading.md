---
tags:
  - java
links:
  - "[[Primitive Types]]"
---
- Methods can have the **same name** and be declared in the same class as long as their parameters are different
	- Different type and/or order
```java
System.out.printIn(Math.max(10, 20))
System.out.printIn(Math.max(10.5, 20.5))
```
- Math methods are overloaded with 4 different versions
	- two double parameters
	- two float parameters
	- two int parameters
	- two long parameters