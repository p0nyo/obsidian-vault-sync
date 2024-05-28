---
tags:
  - compsci
  - networks
  - security
links:
  - "[[HTTP Authentication]]"
---
![[Pasted image 20240527175330.png]]
- Digest only difference

### HTTP Request
![[Pasted image 20240527180806.png|250]]
### HTTP Response
![[Pasted image 20240527180826.png|250]]
![[Pasted image 20240527181522.png|200]]
- Extra headers, nonce and opaque
	- `Opaque` = timestamp
- Secret string: only server knows
- userHostAddress: IP address of the client
### HTTP Request(2)
![[Pasted image 20240527181028.png]]
![[Pasted image 20240527181231.png|200]]
- ha1 =  ("bond007:Mordor:bond007psswrd)
- Method: the method the client used to request the server
### HTTP Response(2)
![[Pasted image 20240527181138.png|250]]
