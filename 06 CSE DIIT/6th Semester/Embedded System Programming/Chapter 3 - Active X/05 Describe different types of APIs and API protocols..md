---
class: cse
title: 05 Describe different types of APIs and API protocols.
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2021
topic: Set 01
---

### Types of APIs

> NOTE: _see exam kit page no. 309 different table_

1. **Open/Public API**  
    Open APIs are accessible to external developers and the general public. They allow third-party applications to use the services or data of a platform without accessing its internal code. For example, the Google Maps API lets apps display maps, calculate routes, and show locations.
    
2. **Private/Internal API**  
    Private APIs are used internally within an organization to connect its own applications and systems. They help streamline processes and maintain secure communication between software modules, such as integrating a company’s HR and payroll systems.
    
3. **Partner API**  
    Partner APIs are shared with selected business partners under controlled access. They enable trusted partners to interact with a system while keeping it hidden from the public. For instance, a payment gateway API provided only to approved e-commerce websites.
    
4. **Composite API**  
    Composite APIs combine multiple APIs or services into a single request, reducing the number of separate calls and improving efficiency. For example, an API could fetch a user’s profile, recent transactions, and notifications all at once.
    

---

### API Protocols

1. **REST (Representational State Transfer)**: REST APIs communicate using **HTTP methods** like GET, POST, PUT, and DELETE. They are **stateless**, lightweight, and suitable for web and mobile applications. Data is often exchanged in **JSON** or XML format. **Example:** Twitter API, Google Maps API.
2. **SOAP (Simple Object Access Protocol)**: SOAP uses **XML messages** for communication and provides **strict standards and high security**. It is commonly used in enterprise systems like banking or insurance services where reliability and data integrity are important.    
3. **XML-RPC (XML Remote Procedure Call)**: XML-RPC allows clients to execute functions on a **remote server** using XML to encode requests and HTTP to transport them. It is simpler than SOAP and used for basic remote procedure calls over the internet.    
4. **JSON-RPC (JSON Remote Procedure Call)**: JSON-RPC is similar to XML-RPC but uses **JSON** for request and response formatting. It is **lightweight and fast**, making it popular in modern web applications for client-server communication.    
5. **GraphQL**: GraphQL is a **query language** that lets clients request **only the data they need**, avoiding over-fetching or under-fetching. It is widely used in apps like Facebook to efficiently manage structured data.    
6. **gRPC (Google Remote Procedure Call)**: gRPC uses **HTTP/2** and **Protocol Buffers** for **high-performance communication** between distributed services. It is suitable for **microservices and real-time applications** where speed and efficiency are crucial.    
7. **WebSockets**: WebSockets enable **continuous two-way communication** over a single TCP connection. They are ideal for **real-time applications** like live chat, online gaming, or stock market updates.