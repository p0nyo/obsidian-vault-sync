---
tags:
  - compsci
  - security
links:
  - "[[Ciphers]]"
---
Takes a *block out of the plaintext* and uses an encryption algorithm and key to *output a block of ciphertext.*
- Length of plaintext = Length of ciphertext
 ![[Pasted image 20240508164744.png]]
 - Slice plaintext into multiple blocks
 - Advantage: Can process them parallel
##### Transposition Cipher
 If the plaintext is very long, can divide it into blocks of 18 characters and follow the transposition logic
 ![[Pasted image 20240508165029.png]]
- Need to pad the last transposition block if it is smaller than the size of the block
	- This becomes a weakness
 
