
# HTTP Response & Status Codes

When we send a request to a web server, the server sends back an HTTP response.

The response tells us if our request was successful or if there was a problem.

### Status Line

The first line of an HTTP response is called the Status Line.

It contains 3 things:
- **HTTP Version:** Shows the HTTP version.
- **Status Code:** Shows the result of the request.
- **Reason Phrase:** A short message about the result.

### Status Code Categories

- **100-199:** Informational responses.
- **200-299:** The request was successful.
- **300-399:** The resource moved to another URL.
- **400-499:** There is a problem with the client request.
- **500-599:** There is a problem on the server side.

### Common Status Codes

- **100 Continue:** The server is ready to receive the rest of the request.
- **200 OK:** Everything worked successfully.
- **301 Moved Permanently:** The resource moved to a new URL.
- **404 Not Found:** The requested page was not found.
- **500 Internal Server Error:** Something went wrong on the server.

#### Status Line Example

The Status Line is the first line of an HTTP response. It contains the HTTP version, status code and reason phrase.

Example:

```http
HTTP/1.1 200 OK
```

- **HTTP/1.1:** Shows which HTTP version the server uses.
- **200:** The status code. It means our request was successful.
- **OK:** The reason phrase. It gives a short explanation of the result.

Another example:

```http
HTTP/1.1 404 Not Found
```

Here, the server tells us that the requested page was not found.

# What I learned

I learned that HTTP responses tell us what happened after we send a request. The Status Line gives us the main information about the response.

I also learned the five status code categories and some common codes like 200, 301, 404 and 500.
