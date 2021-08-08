# Evolution-of-HTTP
HTTP/0.9 — The One-line Protocol
•	Initial version of HTTP — a simple client-server, request-response, telenet-friendly protocol
•	Request nature: single-line (method + path for requested document)
•	Methods supported: GET only
•	Response type: hypertext only
•	Connection nature: terminated immediately after the response
•	No HTTP headers (cannot transfer other content type files), No status/error codes, No URLs, No versioning


TP/1.0 — Building extensibility
•	Browser-friendly protocol
•	Provided header fields including rich metadata about both request and response (HTTP version number, status code, content type)
•	Response: not limited to hypertext (Content-Type header provided ability to transmit files other than plain HTML files — e.g. scripts, stylesheets, media)
•	Methods supported: GET , HEAD , POST
•	Connection nature: terminated immediately after the response


HTTP/1.1 — The standardized protocol
•	This is the HTTP version currently in common use.
•	Introduced critical performance optimizations and feature enhancements — persistent and pipelined connections, chunked transfers, compression/decompression, content negotiations, virtual hosting (a server with a single IP Address hosting multiple domains), faster response and great bandwidth savings by adding cache support.
•	Methods supported: GET , HEAD , POST , PUT , DELETE , TRACE , OPTIONS
•	Connection nature: long-lived


HTTP/2.0 and the future
All above features are being used by major web servers and browsers today. But modern enhancements like HTTP/2.0, Server Side Events (SSE), and Websockets have changed the way that the traditional HTTP works. In my next article on Web API Design with HTTP and Websockets, we will discuss how we should choose them in real-world projects.

1
