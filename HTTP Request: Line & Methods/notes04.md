HTTP Request Line and Methods

HTTP Request Line

HTTP Request Line is the first line of an HTTP request. It has 3 parts.

Example:

GET /login HTTP/1.1


GET – This is the method. It tells the server what we want to do.

/login – This is the path. It shows which page or resource we want.

HTTP/1.1 – This is the HTTP version.

Path and Query String

Example:

https://example.com/products?id=10

Here:

/products is the Path. It shows which page we want.

?id=10 is the Query String. It sends extra information to the server.

So basically:

Path = Which page?

Query String = Extra information.

HTTP Methods

HTTP methods tell the server what we want to do.

These are the main methods I learned:

Method

What it does

GET

Gets data from the server.

POST

Sends data to the server.

PUT

Replaces or updates a resource.

PATCH

Changes only a part of a resource.

DELETE

Deletes a resource.

HEAD

Gets headers without the response body.

OPTIONS

Shows which methods are available.

TRACE

Sends the request back for debugging.

CONNECT

Creates a tunnel through a proxy, usually for HTTPS.

Simple examples

Imagine we have a user profile:

GET – I want to see my profile.

POST – I want to create a new profile.

PUT – I want to replace my profile information.

PATCH – I want to change only my profile picture.

DELETE – I want to delete my profile.

Some other methods:

HEAD – I want to get only the headers.

OPTIONS – I want to know which methods I can use.

TRACE – I want to check my request.

CONNECT – I want to create a connection tunnel.

What I need to remember

Request Line = Method + Path + HTTP Version.

Path tells us which resource we want.

Query String sends extra information.

GET = Get data.

POST = Send data.

PUT = Replace.

PATCH = Change part.

DELETE = Delete.
