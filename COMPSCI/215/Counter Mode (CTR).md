---
tags:
  - compsci
  - security
links:
  - "[[Block Cipher Mode of Operation]]"
---
![[Pasted image 20240508171459.png]]
- Nonce = IV
- Counter value increments the nonce value so that each stage will result in a different encryption pattern
- Advantage: Can work on plaintext blocks in parallel since there are no dependencies 