---
tags:
  - compsci
  - security
links:
  - "[[Decryption]]"
---
A straight forward frequency analysis will not help break a Vigenere Cipher
- Find two instances in the plain text that are the same and count the distance between them
	- The key length could then be the divisors of that number
	- If there are two pairs of identical instances but at different lengths, the common divisor would be the key length (assuming there was only one)
- Then perform frequency analysis on each group
![[Pasted image 20240430173016.png]]
#### Phantom Matches
- When the cipher text fragments match but the plain text fragments don't
![[Pasted image 20240430174530.png]]
![[Pasted image 20240430174545.png]]
