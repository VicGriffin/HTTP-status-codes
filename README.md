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

