* HTTP Basics [Link] (https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177)
  * HTTP allows for communication between distributed systems.
  * HTTP takes place over TCP/IP with a default port of 80.
  * Messages are received in a Request/Response pair.
  * ![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-url-structure.png)
  * Makes use of the verbs GET, POST, PUT, and DELETE.
  * Response typically include status codes:
    * 1xx - Mostly deprecated response code
    * 2xx - Success
    * 3xx - Redirect
    * 4xx - Client Error
    * 5xx - Server Error
  * ![](https://cdn.tutsplus.com/net/authors/jeremymcpeak/http1-req-res-details.png)
  * There are various types of headers that are send between the request and response.
  * Chrome/Webkit inspector and ExpressJS are tools to view HTTP traffic.

* How DNS Works [Link] (https://howdns.works/)
  * The Domain Name System (DNS) allows IP addresses to be resolved as words that are more human readable.
  * If your operating system or browser is not familiar with a domain then it will reach out to a resolver.
  * The resolver is normally hosted by your Internet Service Provider (ISP) at the root and will redirect to the Top-level Domain (TLD), such as .COM.
  * There are currently twelve root servers (such as .COM, .ORG, and .NET).
  * This will then direct to an authoritative name server for the domain (www.google.com) which then gives the IP address.
  * This information is then returned to the client and cached if access is needed again.

* HTTP & REST [Link] (https://www.youtube.com/watch?v=Q-BpqyOT3a8)
  * Web Application Program Interfaces (APIs) are promises between two different pieces of software consisting of a structured request and response.
  * Analogy - waiter is the API whereas the dinner guest is the client and the kitchen cook is the server.
  * Representational State Transfer (ReST) is a stateless client-server protocol similar to HTTP.
  * Curl is a tool that can transfer HTTP requests.
  * Some requests require authentication.

* References
  * HTTP [Link] (https://code-maze.com/the-http-reference/)
  * REST [Link] (https://www.restapitutorial.com/lessons/httpmethods.html)