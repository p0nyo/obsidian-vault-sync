---
tags:
  - compsci
  - security
links:
  - "[[Caeser Cipher]]"
---
Vigenere ciphers are *polyalphabetic ciphers* as it uses multiple substitution alphabets
##### Implementation
- Uses a series of Caesar Ciphers for encryption
![[Pasted image 20240430170646.png]]
- The plain text is broken down into the length of the key, in this example len(key) = 5
- Each group is shifted by the same shift amount as dictated by the key
![[Pasted image 20240430170901.png|200]]
EXAMPLE
- For the key {14, 1, 12, 24, 1}
- Plaintext = VIGENERE CIPHER USES A SERIES OF CAESAR CIPHERS
##### Breaking
A straight forward frequency analysis will not help break a Vigenere Cipher
- Find two instances in the plain text that are the same and count the distance between them
	- The key length could then be the divisors of that number
	- If there are two pairs of identical instances but at different lengths, the common divisor would be the key length (assuming there was only one)
- Then perform frequency analysis on each group
![[Pasted image 20240430173016.png]]
##### Phantom Matches
- When cipher text fragments match but the plain text fragments don't
