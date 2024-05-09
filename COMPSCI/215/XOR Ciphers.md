---
tags:
  - compsci
  - security
links:
  - "[[XOR (Exclusive OR)]]"
  - "[[Caeser Cipher]]"
---
XOR Ciphers utilise the important XOR property of [[XOR (Exclusive OR)#^a0a3e4|symmetry]].
$$C=P\oplus K$$
$$P=C\oplus K$$
$$K=P\oplus C$$
Where P: Plaintext, C: Ciphertext, K: key.
##### Implementation
$$C=P\oplus K=(P+K)\ mod\ 2$$
- Use XOR on bits in the ASCII representation of the plaintext
##### Breaking
Frequency Analysis
- Needs reasonable amount of plaintext to work
- Gives possible keys, still have to check which one works
Bruteforcing
- e.g if key is only 8 bits then only(?) 256 keys to brute force
##### Extending
- 

*notes*
$$X\oplus X=0$$
$$X\oplus 0 =X$$
- Cipher cannot be cracked if *the length of key = length of plaintext*, *key is truly random and key is never reused*
	- This becomes known as a [[One-time Pad (Vernam Cipher)]]


