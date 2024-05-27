---
tags:
  - compsci
  - networks
links:
  - "[[HTTP]]"
---
**Four Stages to an HTTP Connection**
1. Client connects to the server at IP address and port number given by URL
	![[Pasted image 20240527153457.png|200]]
	- Will perform a three-way hand shake to establish connection
2. Client send the request for the resource as indicated in the URL
3. Server response with the response
4. Server closes the connection
	- Default for HTTP 1.0 is to close the connection 
	- Default for HTTP 1.1 is to keep the connection open
### HTTP Request
![[Pasted image 20240527154237.png|200]]
Request Line
- GET / HTTP / 1.1
General Header
- Can be found on both the HTTP request and response
	- Connection header
	- Date header
	- Cache Control (Expiry Dates)
Request Header
- Host: `www.nzherald.co.nz`
- User-Agent: `Firefox`
Entity Header + Entity Body
- Payload/Data if it was being used to upload information onto the server
- Optional fields
### HTTP Response
![[Pasted image 20240527154659.png|200]]
Status Line
- HTTP / 1.1 200 OK
General Header
- Same as request general header
Response Header
- Server: `Apache`
Entity Header
- Content-Type: `text/html`
	- Since it is telling us about the data we are sending
Entity Body
- Sending an HTML file
 