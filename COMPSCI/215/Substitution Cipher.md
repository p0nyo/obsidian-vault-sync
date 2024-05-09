---
tags:
  - compsci
  - security
links:
  - "[[Ciphers]]"
---
Substitution ciphers are *monoalphabetic ciphers* as they only use a single substitution over the plain text
##### Implementation
A substitution cipher uses a permutation of the English alphabet
For example:
- A maps to anyone of the 26 characters
- B maps to any character that A isnt
- C maps to any character A and B isnt
- Etc.
**Key for Cipher**
The key is the mapping of the source alphabets to target
- Form a key phrase and use it as a basis for formulating a unique mapping![[Pasted image 20240430165011.png]]
![[Pasted image 20240430165011.png]]
- Copy all unique letters from key phrase to mapping in order
- Then copy all leftover letters in the alphabet in order
#### Cracking 
- Brute force is impossible
- Frequency analysis can break substitution ciphers