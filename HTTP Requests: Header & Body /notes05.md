HTTP Request Headers and Body

Request Headers

Headers give extra information about the HTTP request. They help the server understand the request.

Example:

POST /login HTTP/1.1
Host: example.com
User-Agent: Chrome
Content-Type: application/json
Content-Length: 35

Some important headers:

Host – Shows which website we are sending the request to.

User-Agent – Shows which browser or application we are using.

Content-Type – Tells the server what format the body uses.

Content-Length – Shows the size of the body in bytes.

Request Body

The Request Body is where we put the data we want to send to the server.

For example, when we register or log in to a website, our information can be sent inside the body.

There are different ways to format this data:

1. URL Encoded

Data is written in key=value format. Different values are separated by &.

Example:

name=Ali&age=20&country=AZ

I can remember it by seeing the = and & symbols.

2. Form Data

This format is used when we need to send different types of data, for example text and files.

It is also useful for uploading images or other files.

Its Content-Type looks like this:

Content-Type: multipart/form-data

The data is separated into different parts using a boundary.

3. JSON

JSON is a common format for sending data, especially when working with APIs.

Data is written inside curly brackets {} using key and value pairs.

Example:

{
  "name": "Ali",
  "age": 20,
  "country": "AZ"
}

Its Content-Type is:

Content-Type: application/json

4. XML

XML uses tags to organize data. Each tag has an opening and a closing part.

Example:

<user>
    <name>Ali</name>
    <age>20</age>
    <country>AZ</country>
</user>

Its Content-Type is:

Content-Type: application/xml

What I need to remember

Headers = Extra information about the request.

Body = The data we send to the server.

Content-Type = The format of the body.

Content-Length = The size of the body in bytes.

Body formats:

URL Encoded = name=Ali&age=20

Form Data = Used for forms and file uploads.

JSON = { "name": "Ali" }

XML = <name>Ali</name>
