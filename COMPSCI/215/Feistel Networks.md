---
tags:
  - compsci
  - security
links:
  - "[[Modern Block Ciphers]]"
---
##### Encryption
![[Pasted image 20240508172302.png]]
- Splits the plaintext into a left half and a right half
$$L_{i+1}=R_i$$
- The new left half is the old right half
$$R_{i+1}=L_i\oplus F(R_i,K_i)$$
- New right half is determined by this equation
- *F* is the feistel cipher function
![[Pasted image 20240508172543.png]]
- The plaintext is typically ran through the feistel network twice
##### Decryption
- After encryption, the L and R are swapped around so that at the end of the decryption the plaintext is the right way around
![[Pasted image 20240508173133.png]]
$$A=L_{i+1}=R_i$$
$$B=R_{i+1}\oplus F(L_{i+1},K_i)=L_i$$

