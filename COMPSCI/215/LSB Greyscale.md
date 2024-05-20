---
tags:
  - compsci
  - security
links:
  - "[[Steganography]]"
---
![[Pasted image 20240520144426.png|350]]
- Each pixel is 8 bits long (0 - 255 Values)
- 0 = white and 255 = black
- If we were to increment or decrement the pixel with value 140 by 1 to 141 or 139, we wouldn't be able to tell difference
##### Implementation
- Uses the least significant bit of the pixel
- ![[Pasted image 20240520145351.png|200]]
- Can use two different ways to pick the pixels that are changed
	1. Sequential
		- Easy to crack
		![[Pasted image 20240520145453.png|100]]
	2. Random
		![[Pasted image 20240520145507.png|100]]
- Two ways to alter the pixel values
	1. Replace (LSB Replacement)
	2. Add/Subtract One (LSB Matching)
###### LSB Replacement
![[Pasted image 20240520145757.png|200]]
- Replace the LSB as needed according to the message that you want to encrypt
- Only LSB changed
###### LSB Matching
![[Pasted image 20240520150154.png|200]]
- Add or subtract 1 to/from the pixel value if the LSB of the cover pixel does not match the bit we want to hide
- Choose randomly for whether or not we add or subtract
- Many pixel bits can change depending on the number
	- E.g 01111111 + 1 = 10000000
