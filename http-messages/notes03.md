## HTTP Messages

There are two types of HTTP messages: **Request and Response.**

**1. Request Message**

A Request Message is sent by the user (usually through the web browser) to the server to request something.

Think of it as asking the planet for something we need.

**2. Response Message**

A Response Message is the answer sent by the server back to the user in response to the request.

Think of it as the planet giving us an answer to our request.

### Simple Example

- Request = User asks the server for a webpage.
- Response = Server sends the webpage back to the user.

### Remember

- Request = User → Server
- Response = Server → User


<img width="1110" height="255" alt="image" src="https://github.com/user-attachments/assets/412aa8ab-d9ad-4464-86ce-055a57855849" />

### HTTP Message Structure

Each HTTP message follows a specific format. It has 4 main parts:

1. Start Line

The Start Line is the beginning of the message. It tells us what type of message is being sent and provides important information.

There are two types:

Request Start Line:

Example:

GET /login HTTP/1.1

GET = Request Method (we want to receive information).

/login = Path (the page we want to access).

HTTP/1.1 = HTTP version.

Response Start Line:

Example:

HTTP/1.1 200 OK

HTTP/1.1 = HTTP version.

200 = Status Code (the request was successful).

OK = Status Message.

2. Headers

Headers provide additional information about the HTTP message. They use a key-value format.

Example:

Host: example.com
User-Agent: Chrome
Content-Type: application/json

Host = The website we want to access.

User-Agent = Information about the browser or client.

Content-Type = The format of the message body.

3. Empty Line

The Empty Line separates the Headers from the Body.

It shows where the Headers end and where the Body begins.

4. Body

The Body contains the actual data of the message.

Request Body = Data sent by the user to the server.

Response Body = Data sent by the server back to the user.

For example, when we fill out a login form, the information can be sent inside the Request Body.

Complete HTTP Examples

Example 1: HTTP Request

GET /login HTTP/1.1
Host: example.com
User-Agent: Chrome


Here:

GET /login HTTP/1.1 = Start Line.

Host and User-Agent = Headers.

Empty Line = Separates Headers and Body.

There is no Body in this example.

Example 2: HTTP Response

HTTP/1.1 200 OK
Content-Type: text/html

<h1>Welcome!</h1>

Here:

HTTP/1.1 200 OK = Start Line.

Content-Type = Header.

Empty Line = Separates Headers and Body.

Why Understanding HTTP Messages Matters

They are the foundation of communication between web applications.

They help us understand how browsers and servers communicate.

They help us find problems in web communication.

They are important for understanding web application security.

Key Things to Remember

Part

Meaning

Start Line

Message type and important information

Headers

Additional information

Empty Line

Separates Headers and Body

Body

Actual message data

Remember:

Request = Browser → Server

Response = Server → Browser

GET /login HTTP/1.1 = Request Start Line

HTTP/1.1 200 OK = Response Start Line
