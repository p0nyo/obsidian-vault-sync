---
tags:
  - compsci
  - security
links:
  - "[[Encryption]]"
---
Methods of encrypting a piece of plaintext with a key to turn it into a ciphertext.
#### Notes
**Confusion**
- Confusion is when each bit of the ciphertext depends on multiple parts of the key
**Diffusion** 
- When each bit in the plaintext affects multiple bits of the ciphertext
- Perfect diffusion = change in a plaintext bit affects roughly half of the ciphertext bits
**Repetition**
- If the combinations for brute-forcing increases with repeated encryption, then repetition might be useful.
- These repetitions are called rounds
**Stream Ciphers**
- Normally work on a small number of bits (8)
- Would use substitution
**Block Ciphers**
- Normally work on a large number of bits (64)
- Uses a mix of substitution and transposition
