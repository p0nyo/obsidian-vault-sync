---
tags:
  - compsci
  - security
links:
  - "[[Block Cipher Mode of Operation]]"
---
![[Pasted image 20240508171047.png]]
- This mode uses an initialisation vector
- The IV is first encrypted with the Key before it is XOR with the plaintext to create the ciphertext
- The parameter passed from Stage M to M+1 is the resulting ciphertext