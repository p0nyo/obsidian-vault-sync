---
tags:
  - compsci
  - security
links:
  - "[[XOR Ciphers]]"
---
##### Conditions
XOR Cipher becomes a One-time pad if:
1. The length of key = length of plaintext
2. The key is truly random
3. Key is never reused
##### Benefits
- Perfect secrecy
	- Practically impossible to crack but can be proven by theory to have perfect secrey
	- No information about the plaintext, other than possible maximum length
##### Breaking
- Not possible
- If any of the three conditions are broken then it can be broken
	- If the key is repeated with other plaintexts, then the cipher can be broken with a Crib Drag