---
tags:
  - compsci
  - security
links:
  - "[[Block Cipher Mode of Operation]]"
---
![[Pasted image 20240508170817.png]]
- This mode uses an initialisation vector
- The parameter being passed from Stage M to M+1 is the XOR of the plaintext and corresponding ciphertext
$$Parameter=Plaintext\oplus Ciphertext$$
