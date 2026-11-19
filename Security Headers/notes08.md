# HTTP Security Headers

Today I learned about HTTP Security Headers. These headers help protect websites from different types of attacks.

## 1. Content-Security-Policy (CSP)

CSP helps protect websites against XSS attacks.

It controls where the browser can load content from, such as JavaScript, CSS and images.

Example:

```http
Content-Security-Policy: default-src 'self'
```

`'self'` means the browser can load content from the same website.

## 2. Strict-Transport-Security (HSTS)

HSTS tells the browser to use HTTPS when connecting to the website.

It helps protect communication between the browser and the server.

Example:

```http
Strict-Transport-Security: max-age=63072000
```

`max-age` tells the browser how long to remember this rule.

## 3. X-Content-Type-Options

This header helps prevent MIME sniffing.

MIME sniffing happens when the browser tries to guess a file type instead of using the type sent by the server.

Example:

```http
X-Content-Type-Options: nosniff
```

`nosniff` tells the browser not to guess the file type.

## 4. Referrer-Policy

This header controls how much information about the previous page is sent to another website.

Example:

```http
Referrer-Policy: strict-origin-when-cross-origin
```

It helps protect private URL information when visiting other websites.

## 5. Other Security Headers

Some other useful headers are:

- `X-Frame-Options`: Helps protect against Clickjacking.
- `Permissions-Policy`: Controls browser features like camera, microphone and location.

## What I learned

Today I learned that HTTP Security Headers add extra protection to web applications.

I also learned about CSP, HSTS, MIME sniffing and Referrer-Policy.

These headers do not fix every security problem, but they help make websites safer.
