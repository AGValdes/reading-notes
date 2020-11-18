# Class 13 Reading Notes: Sending Form Data

- Once the form data has been validated on the client-side, it is okay to submit the form
### Client-Server Architechture
a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.
- An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. 

### Defining How To Send the Data:
- The `<form>` element defines how the data will be sent. 
- All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are **action** and **method**.
- **Action:** defines where the data gets sent
- **Method:** defines how data is sent

### GET method:
- The **GET method** is the method used by the browser to ask the server to send back a given resource: **"Hey server, I want to get this resource."**
- The data is appended to the URL as a series of name/value pairs

### POST method:
- the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: **"Hey server, take a look at this data and send me back an appropriate result."**

### Viewing HTTP Requests:
- HTTP requests are never displayed to the user (if you want to see them, you need to use tools such as the Firefox Network Monitor or the Chrome Developer Tools)

### Retrieving the Data:
- Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs

[<-- Back](301readingnotes.md) [Back to Home](README.md)
