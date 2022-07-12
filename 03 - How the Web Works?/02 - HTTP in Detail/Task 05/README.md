# Task 5 - Headers

Headers are additional bits of data you can send to the web server when making requests.

Although no headers are strictly required when making a HTTP request, you’ll find it difficult to view a website properly.

## Common Request Headers

These are headers that are sent from the client (usually your browser) to the server.

- **Host:** Some web servers host multiple websites so by providing the host headers you can tell it which one you require, otherwise you'll just receive the default website for the server.

- **User-Agent:** This is your browser software and version number, telling the web server your browser software helps it format the website properly for your browser and also some elements of HTML, JavaScript and CSS are only available in certain browsers.

- **Content-Length:** When sending data to a web server such as in a form, the content length tells the web server how much data to expect in the web request. This way the server can ensure it isn't missing any data.

- **Accept-Encoding:** Tells the web server what types of compression methods the browser supports so the data can be made smaller for transmitting over the internet.

- **Cookie:** Data sent to the server to help remember your information (see cookies task for more information).

## Common Response Headers

These are the headers that are returned to the client from the server after a request.

- **Set-Cookie:** Information to store which gets sent back to the web server on each request (see cookies task for more information).

- **Cache-Control:** How long to store the content of the response in the browser's cache before it requests it again.

- **Content-Type:** This tells the client what type of data is being returned, i.e., HTML, CSS, JavaScript, Images, PDF, Video, etc. Using the content-type header the browser then knows how to process the data.

- **Content-Encoding:** What method has been used to compress the data to make it smaller when sending it over the internet.

# Answer the following questions

1. What header tells the web server what browser is being used?
```
User-Agent
```
2. What header tells the browser what type of data is being returned?
```
Content-Type
```
3. What header tells the web server which website is being requested?
```
Host
```




