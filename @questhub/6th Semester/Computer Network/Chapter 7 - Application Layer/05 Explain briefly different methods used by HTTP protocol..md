---
class: cse
title: 05 Explain briefly different methods used by HTTP protocol.
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2019
---
# Different Methods Used by HTTP Protocol

The **Hypertext Transfer Protocol (HTTP)** defines several methods that specify the type of action a client wants to perform on a resource. Each method has a particular purpose, governing how data is sent, retrieved, or modified on the server. Understanding these methods is crucial for web communication and API development.

---

## Main HTTP Methods

1. **GET**  
    The GET method is used to **retrieve data from the server** without modifying it. This method is safe and idempotent, meaning multiple identical requests produce the same result without side effects. GET requests can be cached and bookmarked. It is commonly used for fetching web pages, images, or other static resources.  
    _Example: Loading a homepage or accessing www.example.com/index.html._
    
2. **POST**  
    The POST method **submits data to the server** to create or update a resource. Unlike GET, it can change server-side data and is not cached or bookmarked. POST is commonly used for sending form data, uploading files, or submitting user inputs. It allows sending complex data in the request body, such as JSON or XML.  
    _Example: Submitting a registration form or posting a comment on a blog._
    
3. **PUT**  
    The PUT method **updates an existing resource** or creates it if it does not exist. It is idempotent, meaning sending the same request multiple times has the same effect. PUT is used when the client wants to replace the current representation of a resource with new data.  
    _Example: Updating user profile information on a website or replacing an entire document in a database._
    
4. **DELETE**  
    The DELETE method **removes a specified resource** from the server. Like PUT, it is idempotent. DELETE ensures that the targeted resource is permanently removed, and the server confirms the operation with an appropriate status code.  
    _Example: Deleting a comment, post, or account from a web application._
    
5. **HEAD**  
    The HEAD method retrieves **only the headers of a resource** without its body. It is useful for checking metadata, such as content type, content length, or last modification date, before deciding to download the full resource. This saves bandwidth and improves efficiency.  
    _Example: Checking if a file has been updated before downloading it._
    
6. **PATCH**  
    The PATCH method is used to **apply partial modifications to a resource** rather than replacing it entirely. It is more efficient than PUT when only a small portion of the resource needs updating. PATCH is commonly used in RESTful APIs to update specific fields of an object.  
    _Example: Updating only the email address of a user profile without changing other details._
    
7. **OPTIONS**  
    The OPTIONS method requests the server to **describe the communication options** available for a resource. It is often used for testing, debugging, or for CORS (Cross-Origin Resource Sharing) preflight requests in web applications. OPTIONS helps the client understand what methods and headers are supported.  
    _Example: Checking which HTTP methods are allowed for an API endpoint before making a POST request._
    
8. **TRACE**  
    The TRACE method **echoes back the received request** for diagnostic purposes. It allows the client to see how the request is modified by intermediaries such as proxies or gateways. TRACE is mainly used for debugging and testing network paths.  
    _Example: Diagnosing whether a firewall or proxy is altering HTTP requests._
    
9. **CONNECT**  
    The CONNECT method **establishes a tunnel** to the server, often used for secure HTTPS connections through a proxy. Once the connection is established, data can flow between the client and server securely over the tunnel.  
    _Example: Browsing a secure website via an HTTP proxy using SSL/TLS._