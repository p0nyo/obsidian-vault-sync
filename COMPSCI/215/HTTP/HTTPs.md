---
tags:
  - compsci
  - networks
links:
---
Request - Response Protocol
- Server will not send anything unless the client sends something
![[Pasted image 20240527152410.png|300]]
- Port 8080
![[Pasted image 20240527152753.png|350]]

- What is the reason for the Content-Type header?
	- Client may ask for an HTML file, but the server could potentially give something different back
	- If other options e.g Error pages, come up, then the client would have to use extra processing power to show the correct webpage
	- If server declares the data type from the beginning then the client wouldn't have to do it 
