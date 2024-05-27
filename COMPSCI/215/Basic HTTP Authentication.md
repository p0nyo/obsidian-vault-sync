---
tags:
  - compsci
  - networks
links:
  - "[[HTTP Authentication]]"
---
### Encoding
- The key that is being sent from client to server is encoded with Base64 Encoding

![[Pasted image 20240527164803.png]]
1. Client asks to access the secret file
2. Server sends back authorization request
	- Client is asked to authenticate themselves, which the server will then check to see if they are authorized to access the file
3. Client sends back the same GET method but with the `Authorization:` header
4. Server sends `200 Ok` if it is authenticated and authorised
When username+password reaches server, the hash obtained from username+password will be checked against the stored hash
