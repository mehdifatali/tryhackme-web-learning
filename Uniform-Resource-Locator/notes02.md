# Uniform Resource Locator
A Uniform Resource Locator (URL) is a web address that lets you access all kinds of online content—whether it’s a webpage, a video, a photo, or other media. It guides your browser to the right place on the Internet.

Anatomy of a URL
 <img width="788" height="209" alt="image" src="https://github.com/user-attachments/assets/37f082ef-6782-4736-902c-ed4743efe060" />
URL (Uniform Resource Locator)

## A URL is the address we use to access a website or a specific resource.

Let's imagine it as an address that helps us travel to a specific place on our planet.

A URL has different components:

Example:

https://admin:1234@example.com:443/products?id=10#reviews

1. Scheme

The scheme is the protocol used to access the website.

The most common ones are:

HTTP – HyperText Transfer Protocol.

HTTPS – HyperText Transfer Protocol Secure.

HTTPS is more secure because it encrypts the connection.

Think of it as choosing how we travel to our planet.

2. User

Some URLs can contain login information, such as a username and password.

Example:

https://admin:1234@example.com

admin = Username

1234 = Password

This method is rare nowadays because putting login details in a URL is not safe. It can expose sensitive information.

Think of it as the login information needed to enter a planet.

3. Host/Domain

The host or domain tells us which website we are accessing.

Example:

example.com

Every domain name is unique.

From a cybersecurity perspective, we should be careful about fake domains that look almost like real ones.

Typosquatting: Attackers create fake domain names that look very similar to real websites.

Example:

Real domain: microsoft.com

Fake domain: rnicrosoft.com

Here, the letter m is replaced with r and n. At first glance, they look very similar.

Attackers use this trick to fool users and perform phishing attacks.

Think of the domain as the name of our planet.

4. Port

The port number helps direct the browser to the correct service on the web server.

Think of it as different doors on our planet. Each door can lead to a different service.

Common ports:

Port 80 = HTTP

Port 443 = HTTPS

Port numbers range from 1 to 65,535.

5. Path

The path points to a specific page or resource on the server.

Example:

example.com/login

example.com/about

example.com/products

Think of it as choosing a specific city or place on our planet.

From a cybersecurity perspective, sensitive paths must be protected so that only authorized users can access them.

6. Query String

The query string is the part of a URL that starts with a question mark (?).

It is used to pass additional information, such as search terms or form inputs.

Example:

google.com/search?q=cybersecurity

? = Starts the query string.

q = Parameter name.

cybersecurity = Parameter value.

Another example:

example.com/products?id=10

Here, id=10 is additional information sent with the request.

Users can modify query strings, so the server must handle this information securely to prevent attacks like injection.

Think of it as giving additional information about where we want to go on our planet.

7. Fragment

The fragment starts with a hash symbol (#).

It helps us jump to a specific section of a webpage.

Example:

example.com/article#comments

Here, #comments points to the comments section of the page.

Think of it as choosing a specific point on our planet's map.

The fragment is normally handled by the browser and is not sent to the web server as part of the HTTP request.

4. Questions and Answers

Q1. Which component on a computer is responsible for hosting and delivering content for web applications?

Answer: Web Server.

Explanation: A web server hosts website content and delivers it to the user's browser.

Q2. Which component allows users to access and interact with web applications?

Answer: Web Browser.

Explanation: A web browser allows users to open websites, click buttons, fill out forms, and use website features.

Q3. What part of a URL is used to pass additional information, such as search terms or form inputs, to the web server?

Answer: Query String.

Explanation: The query string starts with ? and passes additional information through URL parameters.

Example: google.com/search?q=cybersecurity
