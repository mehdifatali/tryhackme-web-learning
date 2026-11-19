# HTTP Response Headers & Response Body

After sending a request, the server sends a response back to our browser.

The response has headers and a body. Headers give extra information, and the body contains the actual data.

## 1. Response Headers

Response Headers give extra information about the server's response. They also tell the browser how to handle the received data.

### Content-Type

It shows the type of data sent by the server.

Example:

```http
Content-Type: application/json
```

This means the server is sending data in JSON format.

Other examples:
- `text/html` - HTML page
- `text/plain` - Normal text
- `image/png` - PNG image
- `application/pdf` - PDF file

### Content-Length

It shows the size of the response body in bytes.

Example:

```http
Content-Length: 1200
```

This means the response body is 1200 bytes.

### Set-Cookie

The server uses Set-Cookie to send cookies to our browser.

Example:

```http
Set-Cookie: sessionId=abc123
```

The browser saves this cookie and sends it with future requests.

Some important security flags:

- `HttpOnly` - JavaScript cannot access the cookie.
- `Secure` - The cookie is only sent over HTTPS.

### Cache-Control

This header tells the browser how long it can keep a response in cache.

Example:

```http
Cache-Control: max-age=600
```

600 seconds means 10 minutes.

### Location

This header is used for redirection. It shows the new URL where the browser should go.

Example:

```http
HTTP/1.1 301 Moved Permanently
Location: /login
```

This tells the browser to go to the new location.

## 2. Response Body

The Response Body contains the actual data sent by the server.

It can contain HTML, JSON, images and other data.

Example:

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "message": "Login successful!",
  "status": "success"
}
```

Here:
- `200 OK` means the request was successful.
- `Content-Type` tells us that the data is JSON.
- The JSON part is the Response Body.
- The message tells us that login was successful.

## 3. Security - XSS

XSS (Cross-Site Scripting) is a web security problem.

It can happen when a website does not properly handle user input and unsafe JavaScript runs in the browser.

Websites should check user input and escape unsafe content to help prevent XSS.

## What I learned

I started by explaining these topics to myself to understand how they work.

Then I took some notes and used AI to understand the parts that were not clear to me.

Now I understand how response headers give information about the response and how the response body contains the actual data.

I also learned about cookies, caching, redirection and XSS.
