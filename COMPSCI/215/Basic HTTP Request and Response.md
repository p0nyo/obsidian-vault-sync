---
tags:
  - compsci
  - networks
links:
  - "[[Basic HTTP Authentication]]"
---
### HTTP Request
![[Pasted image 20240527170148.png|300]]
### HTTP Response
![[Pasted image 20240527170227.png|250]]
- 401 Unauthorized status code
- `WWW-Authenticate: Basic` and `Realm="Mordor"`
	- Realm is the context area, don't need re-authentication
### HTTP Request(2)
![[Pasted image 20240527170557.png|250]]
- Sends the HTTP request back but with a authorisation key
- The long line is basically username+password but encrypted
### HTTP Response(2)
![[Pasted image 20240527170706.png|250]]
- Will check if the user is authorised to use the file
	- `200 OK` is they are
	- `401 Unauthorised` is sent if it is not and the same response is sent back
