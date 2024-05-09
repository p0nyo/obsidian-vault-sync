---
tags:
  - compsci
  - security
links:
  - "[[Simple Transposition Ciphers]]"
---
##### Implementation
![[Pasted image 20240505163942.png]]
- Assign a number to each row and rearrange in order to form a new matrix
- Ciphertext = YOIABTAWPSNELLHWOE
![[Pasted image 20240505164156.png]]
- If there are enough characters for the matrix, then replace the spaces with z
##### Breaking
![[Pasted image 20240505164526.png]]
- Find most likely distance between the two Z's
![[Pasted image 20240505164809.png|200]]
- Then create matrix based off estimation
