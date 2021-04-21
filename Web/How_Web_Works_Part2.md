### Concepts

**HTTP (Hypertext Transfer Protocol)**

- A set of rules that tells browser and server how to communicate with each other.
- HTTPS or HTTP Secure
  - How browsers and servers communicate with encryption

**Response Codes**

- 200 = OK
- 301 = What you reqeusted is elsewhere
- 404 = Not found - Client Error Response
- 500 = Server had an internal problem

Typically, web browser communicate with server by requesting information. This is called GET method. Then, the server side will process requested information/documents in the DB server. Then server will send response back to the browser.

So what is in a typical Request?

- Method (e.g. Get)
- HTTP protocol version (almost always 1.1)
- Resource URL you want
- Headers
  - Hostname you're asking about
  - Date your browser think it is
  - Language your browser wants information in
  - Any cookies that server has sent

Wht is in a Response?

- HTTP protocl version (almost always 1.1)
- Response Status Code (200, 404, etc.)
- Headers
  - Content Type (text./html)
  - Date/time the server thinks it is
  - Any cookies server wants to set
  - Any caching information
