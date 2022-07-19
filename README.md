# day01


Difference between HTTP 1 and HTTP2:

HTTP stands for hypertext transfer protocol, and it is the basis for almost all web applications. More specifically, HTTP is the method computers and servers use to request and send information. For instance, when someone navigates to GUVI on their laptop, their web browser sends an HTTP request to the GUVI servers for the content that appears on the page. Then, GUVI servers send HTTP responses with the text, images, and formatting that the browser displays to the user.

The first usable version of HTTP was created in 1997. Because it went through several stages of development, this first version of HTTP was called HTTP/1.1. This version is still in use on the web. In 2015, a new version of HTTP called HTTP/2 was created.

HTTP/2 solves several problems that the creators of HTTP/1.1 did not anticipate. In particular, HTTP/2 is much faster and more efficient than HTTP/1.1. One of the ways in which HTTP/2 is faster is in how it prioritizes content during the loading process.

HTTP/1.1: For better understanding, let’s assume the situation when you make a request to the server for the GUVI.html page & server responds to you as a resource GUVI.html page. before sending the request and the response there is a TCP connection established between client & server. again you make a request to the server for image img.jpg & the server gives a response as an image img.jpg. the connection was not lost here after the first request because we add a keep-alive header which is the part of the request so there is an open connection between the server & client. there is a persistent connection which means several requests & responses are merged in a single connection. These are the drawbacks that lead to the creation of HTTP/2: The first problem is HTTP/1.1 transfer all the requests & responses in the plain text message form. The second one is head of line blocking in which TCP connection is blocked all other requests until the response does not receive. all the information related to the header file is repeated in every request.

HTTP/2: HTTP/2 was developed over the SPDY protocol. HTTP/2 works on the binary framing layer instead of textual that converts all the messages in binary format. it works on fully multiplexed that is one TCP connection is used for multiple requests. HTTP/2 uses HPACK which is used to split data from header. it compresses the header. The server sends all the other files like CSS & JS without the request of the client using the PUSH frame.

Difference between HTTP/1.1 and HTTP/2 are:

HTTP/1.1

i.textual format.
ii.There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.
iii.It uses requests resource Inlining for use getting multiple pages
iv.It compresses data by itself.

HTTP2
i.binary protocol.
ii.It allows multiplexing so one TCP connection is required for multiple requests.
iii.It uses PUSH frame by server that collects all multiple pages 
iv.It uses HPACK for data compression.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

OBEJECTS IN JAVASCRIPT:

Objects, in JavaScript, is the most important data-type and forms the building blocks for modern JavaScript. These objects are quite different from JavaScript’s primitive data-types(Number, String, Boolean, null, undefined and symbol) in the sense that while these primitive data-types all store a single value each (depending on their types).

Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object, is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.
Objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, in the form of “key: value” pairs. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

syntax:

variable vaiablename= {
    keyname : value;
}

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------






