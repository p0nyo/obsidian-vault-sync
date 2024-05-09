---
tags:
  - compsci
  - security
links:
  - "[[Block Ciphers]]"
---
*Other Names*
- Mode of Operation
- Multi-Stage Encryption
![[Pasted image 20240508165423.png]]
- Using a parameter from Stage M to encrypt the plaintext in Stage M+1
- The input the very first stage gets is called an *Initialization Vector* (IV)
###### Non-Parallel
- When Stage M+1 relies on Stage M, the stages can't be done in parallel
- If Stage M gets an error, it propagates to all stages
###### Parallel 
- [[Electronic Code Book (ECB)]] and [[Counter Mode (CTR)]] can go parallel and errors are not propagated
- ECB has problems with repeated patterns while CTR does not.
