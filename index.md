## Welcome to GitHub Pages
### Temporary While I figure out how to add a nav bar.
# Week 3 Lecture 2
## HTTP (HyperText Tranfer Protocol)
#### Web Terminology
- Webpage (document): Consists of objects
- Objects: files (html, jpeg, mp3, mp4 etc) that are addressable by a single url.
- If a web page contains html text and five images, then the webpage has 6 objects
- http://www.someschool.edu/someDepartment/picture.gif
- www.someschool.edu : the hostname
- /someDepartment/picture.gif : path name
- Web browsers implement the client side of HTTP (so web browser = client)
- Socket: Acts like a door between the client process and the TCP or UDP etc connection. Also door between the server and the TCP connection.


- HTTP is implemented in two programs: The Client and the Server. They communicate with each other through HTTP messages. HTTP defines the structure of these messages.
- User requests a web page, browser sends HTTP request message for the objects on a webpage, server receives the requests and responds with a HTTP response message containing the objects.
- The client and server send the HTTP requests and responses into their socket information. 
- Since TCP provides reliable data transfer service to HTTP,  the request or response will eventually arrive intact on the other side without needing to worry about it.
- HTTP is a stateless protocol as it maintains no information about clients. e.g. If a client request the same objects again after a couple seconds the server will resend the entire object without remembering it already did that a second ago.
### Non-Persistent and Persistent Connections
Usually a client and server are connected for a long period of time, and the client often makes a lot of requests to the server etc. The series of requests may be made back-to-back, periodically or intermittently (it depends on the application). 
The application developer needs to make the decision about whether each request/response is sent over different TCP connections or over the same one?
- non-persistent connections: Each request/response is sent over a different TCP or UDP connection.
- persistent connections: Each of them are sent over the same connection.
#### Non-Persistent









