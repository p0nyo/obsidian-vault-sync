---
tags:
  - compsci
  - networks
links:
  - "[[HTTP]]"
---
### HTTP 1.0
- Does not require any request headers
- Server closes connection once the resource is sent
### HTTP 1.1 
- Requires a request header with mandatory `Host: header field`
- Server keeps the connection alive until a timeout period
	- Default: Keep alive, but can opt for connection: close
- Widely compatible
### HTTP 0.9
- First implementation of HTTP
- No version information used in the request line
### HTTP 2.0
