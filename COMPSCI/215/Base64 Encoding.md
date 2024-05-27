---
tags:
  - compsci
  - networks
  - security
links:
  - "[[Basic HTTP Authentication]]"
---
- Turns a 24-bit sequence into a 4 character sequences
- 24-bit sentence is divided into four 6-bit groups
- Turn each 6-bit grouping into character from the BASE64 Alphabet

![[Pasted image 20240527171652.png]]
### Padding
- Length of a base64 string is always a multiple of 4
- When short of characters in the base64 string, add the padding character '=' to the end to make it /4
- '=' is equal to '00'
##### Example
- Encode the string 'Cat'
	1.  'C' is 01000011
	2.  'a' is 01100001
	3. 't' is 01110100
	4. Concatenate the 3 ASCIIs
		- 01000011 01100001 01110100
	5. Break into groups of 6 bits
		- 010000 110110 000101 1101100
		- 'Q2F0'