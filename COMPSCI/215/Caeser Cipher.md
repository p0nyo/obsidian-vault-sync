---
tags:
  - compsci
  - security
links:
  - "[[Ciphers]]"
---
Caeser ciphers are *monoalphabetic ciphers* as they only use a single substitution over the plain text
![[Pasted image 20240430154615.png]]
- Moves letter to letter depending on the key:
$$y=(x+key)\;mod\;26$$
![[Pasted image 20240430154656.png|200]]
#### Encryption
A = 65, ASCII for A
Y = 89, ASCII for Y
- Assume key = 4
Y becomes:
$$Y = 65+(((89-65)+4)mod\;26)$$
- 89-65=24 to find the index of the character
- Add 4 (mod 26), get 2
- To get ASCII value of C, add 65 to 2
#### Decryption
Must have the same key = 4
- Assume we read the letter C, ASCII code 67
- Convert to index by subtracting 65, giving index 2
- Subtract the key: 2 - 4 = -2
- Apply the modulus: (-2) mod 26 = 24
- Add 65 offset to get the ASCII code: 24 + 65 = 89 = C
General Decryption Formula:
$$x=65+((y-65)-key)\;mod\;26$$
