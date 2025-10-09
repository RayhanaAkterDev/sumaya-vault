---
class: cse
title: 07 Define WWW & HTTP. Describe basic architecture of HTTP.
course: Embedded System Programming
chapter:
  - "ch6: WWW, Kernel, ASP"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - ESP/Ch6
---
### World Wide Web (WWW)

The **World Wide Web (WWW)** is a system of interlinked hypertext documents and multimedia resources that can be accessed over the internet using web browsers. It was introduced by Tim Berners-Lee in 1989 and is built on three main technologies: **HTML** (for creating web pages), **HTTP** (for communication between client and server), and **URL** (for locating resources). The WWW is different from the internet itself—it is a service that runs on the internet and allows users to access and share information in the form of text, images, audio, video, and interactive content through hyperlinks.

> The **World Wide Web (WWW)** is a collection of interconnected documents and resources, linked together through hyperlinks and identified by URLs, which can be accessed via the internet using a web browser. It was developed by Tim Berners-Lee in 1989 and is based on key technologies such as **HTML** for creating content, **HTTP** for communication, and **URL** for addressing. Unlike the internet itself, which is the global network of computers, the WWW is a service running on top of it that allows users to browse, share, and interact with information in text, images, videos, and other multimedia formats.

---

### HyperText Transfer Protocol (HTTP)

**HTTP (HyperText Transfer Protocol)** is the standard protocol used on the WWW for communication between clients (browsers) and servers. It follows a request–response model where the client sends an HTTP request, and the server replies with an HTTP response. HTTP is a **stateless protocol**, meaning each request is independent and does not retain past interaction history. This simplicity makes HTTP lightweight, but additional technologies like cookies and sessions are used to maintain continuity.

---

### Basic Architecture of HTTP

The **HTTP architecture** follows a **client-server model**, where clients (web browsers) request resources and servers deliver them. Its main components and functions are:

1. **Client (Web Browser or Application)** – The client is responsible for sending requests to the server. A user types a URL into the browser, and the browser formats the request according to HTTP standards. It then interprets the response (such as HTML, CSS, JavaScript, or images) and displays it to the user.
    
2. **DNS Resolution** – Before connecting to a server, the client needs the server’s IP address. The Domain Name System (DNS) translates human-readable domain names (like `www.example.com`) into numeric IP addresses (like `142.250.72.196`). This step ensures the client knows the exact destination server to contact.
    
3. **Web Server** – A web server is software (like Apache, Nginx, or IIS) running on a machine that listens for HTTP requests. When the server receives a request, it processes it (possibly interacting with databases or applications) and then generates an HTTP response containing data such as web pages or files.
    
4. **Request–Response Cycle** – HTTP communication always follows this cycle:
    
    - The client sends a **request** that includes method (GET, POST, PUT, DELETE, etc.), headers, and sometimes a body.
        
    - The server replies with a **response** that contains a status code (200 OK, 404 Not Found, 500 Internal Server Error), headers, and the requested content.
        
5. **Transport Layer (TCP/IP)** – HTTP itself is an application-layer protocol, but it relies on TCP/IP at the transport and network layers to establish a reliable connection between client and server. TCP ensures that data packets arrive correctly and in order.