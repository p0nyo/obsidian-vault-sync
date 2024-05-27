---
tags:
  - compsci
  - networks
links:
  - "[[HTTP]]"
---
**Authentication**: Proves who we say we are
- What we know, username and password
- What we have: security token
- What we are: fingerprint scanner
**Authorization**: Checks to see if we have the rights to do what we want to do
- Passport authenticates us, visa gives us the right to enter the country
#### CIA of Security
- Confidentiality, Integrity, Availability
	- Confidentiality provides privacy and secrecy
	- Integrity is to ensure tamper-free storage and transmission of information
	- Availability is to provide undisruptive services
- Cannot satisfy all the elements'
![[Pasted image 20240527164803.png]]
1. Client asks to access the secret file
2. Server sends back authorization request
	- Client is asked to authenticate themselves, which the server will then check to see if they are authorized to access the file
3. Client sends back the same GET method but with the `Authorization:` header