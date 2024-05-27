---
tags:
  - compsci
  - networks
links:
  - "[[HTTP Request and Response]]"
---
### GET Method
![[Pasted image 20240527155102.png]]
- First slash is the document root
- File that is looking for is `$DOCUMENT_ROOT` + `compsci/lectures.html`
### HEAD Method
![[Pasted image 20240527155627.png]]
- Basically only getting the resource of the content being requested for
	- E.g the content is the HTML file, then only the headers about the file would be sent back
- Useful for verifying link status (dead or live)
- Can check if the resource has been updated etc.
### PUT Method
- Tells the server to place the data in the request body at the URL specified
- Not used due to security concerns
### DELETE Method
- Tells the server to delete the data at the resource specified in the URL
- Not used due to security concerns
### OPTIONS Method
- Used by a client to find out the capabilities of the server
- E.g Methods allowed on the server 
### TRACE Method
- Useful for finding routes, will return the entire request message back in the body of the response to the client
### POST Method
- Used for submitting data to an application running on the server
- Data is stored in the body of the POST after the HTTP headers are used
- 