# HTTP RESPONSE STATUS CODES
- HTTP response status codes indicate whether a specific HTTP request has been successfully completed.   
    - There are five groups of responses
        1. Informational responses (100-199)
        2. Successful responses (200-299)
        3. Redirects (300-399)
        4. Client errors (400-499)
        5. Server errors (500-599)   

## 1. INFORMATION RESPONSE
1.1 __100 Continue__ - this response shows the client to continue the request or ignore the response if the request is already finished.  

1.2 __101 Switching protocols__ -this code is dent in response to an upgrade request header from the client and indicates the protocol the server is switching to.  

1.3 __102 processiing__(WebDAV) -This indicates that the server has received and is processing the request, buut no response is available yet.

1.4 __Early Hints__ -It is supposed to be used with the link header, letting the user agent start preloading resources while the server prepares a response or preconnect to an origin from which the page will need resources.

## 2 Successful responses
2.1 __200 OK__ - The request succeeded, which also depends on the HTTP method that are GET, HEAD, PUT OR POST and TRACE.

2.2 __201 Created__ - The request succeeded, and a new resource is created as a result. T his is the response sent after POST and some PUT request.

2.3 __202 Accepted__ - the request received has not been acted upon

2.4 __203 Non- Authoritative Information__ - This response code 

2.5 __204 No content__- Shows that there is no content to send for the request, though headers may be useful.

2.6 __205 Reset content__ -Communicates to the user agent to reset the document which the request sent.

2.7 __206 Partial Content__ - used when the range header is sent from the client to request only part of a resource.

2.8 __207 Multi Status__ - conveys info about multiple resoources, for situations where multiple status codes might be appropriate.

2.9  __208 Already Reported__ -used to avoid repeatedly enumerating the internal members of multiple bindings to the same collection.

2.10 __226 IM Used__ - the server has fullfilled a get request for the resource.


## Redirection Messages

- **300 Multiple Choices**: Multiple possible responses; user should choose one.
  
- **301 Moved Permanently**: Resource URL has permanently changed; new URL provided.

- **302 Found**: Resource temporarily at a different URI; original URI should be used in future requests.

- **303 See Other**: Client should use a GET request to another URI to retrieve the resource.

- **304 Not Modified**: Resource not modified; use cached version.

- **305 Use Proxy (Deprecated)**: Requested response must be accessed by a proxy; deprecated due to security concerns.

- **306 (Unused)**: Reserved for future use.

- **307 Temporary Redirect**: Resource temporarily at a different URI; same method must be used.

- **308 Permanent Redirect**: Resource permanently at a different URI; same method must be used.

## Client Error Responses

- **400 Bad Request**: Server cannot process request due to client error.

- **401 Unauthorized**: Client must authenticate to get the requested response.

- **402 Payment Required (Experimental)**: Reserved for future use; intended for digital payment systems.

- **403 Forbidden**: Client does not have access rights to the content.

- **404 Not Found**: Server cannot find the requested resource.

- **405 Method Not Allowed**: Request method is known but not supported by the resource.

- **406 Not Acceptable**: No content that conforms to the criteria given by the user agent.

- **407 Proxy Authentication Required**: Client must authenticate with a proxy.

- **408 Request Timeout**: Server timed out waiting for the request.

- **409 Conflict**: Request conflicts with the current state of the server.

- **410 Gone**: Requested content has been permanently deleted.

- **411 Length Required**: Content-Length header field is required.

- **412 Precondition Failed**: Server does not meet one of the preconditions in the request.

- **413 Payload Too Large**: Request entity is larger than server limits.

- **414 URI Too Long**: URI is too long for the server to process.

- **415 Unsupported Media Type**: Media format is not supported by the server.

- **416 Range Not Satisfiable**: Range specified by the Range header cannot be fulfilled.

- **417 Expectation Failed**: Server cannot meet the requirements of the Expect header field.

- **418 I'm a teapot**: Server refuses to brew coffee with a teapot.

- **421 Misdirected Request**: Request was directed at a server unable to produce a response.

- **422 Unprocessable Content (WebDAV)**: Request is well-formed but unable to be followed due to semantic errors.

- **423 Locked (WebDAV)**: Resource is locked.

- **424 Failed Dependency (WebDAV)**: Request failed due to failure of a previous request.

- **425 Too Early (Experimental)**: Server is unwilling to process a request that might be replayed.

- **426 Upgrade Required**: Client should upgrade to a different protocol.

- **428 Precondition Required**: Server requires the request to be conditional to prevent conflicts.

- **429 Too Many Requests**: Client has sent too many requests in a given time.

- **431 Request Header Fields Too Large**: Server is unwilling to process the request due to large header fields.

- **451 Unavailable For Legal Reasons**: Resource cannot be provided due to legal reasons.

## Server Error Responses

- **500 Internal Server Error**: Server encountered a situation it doesn't know how to handle.

- **501 Not Implemented**: Request method is not supported by the server.

- **502 Bad Gateway**: Invalid response from the upstream server.

- **503 Service Unavailable**: Server is not ready to handle the request; often due to maintenance or overload.

- **504 Gateway Timeout**: Server, acting as a gateway, cannot get a response in time.

- **505 HTTP Version Not Supported**: HTTP version used in the request is not supported by the server.

- **506 Variant Also Negotiates**: Internal server configuration error.

- **507 Insufficient Storage (WebDAV)**: Server unable to store the representation needed to complete the request.

- **508 Loop Detected (WebDAV)**: Server detected an infinite loop while processing the request.

- **510 Not Extended**: Further extensions to the request are required for the server to fulfill it.

- **511 Network Authentication Required**: Client needs to authenticate to gain network access.
