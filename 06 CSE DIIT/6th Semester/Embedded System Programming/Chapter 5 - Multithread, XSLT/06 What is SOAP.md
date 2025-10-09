---
class: cse
title: 06 What is SOAP?
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2020
  - board_2022
---
## SOAP (Simple Object Access Protocol)

**SOAP** is a **protocol for exchanging structured information** in the implementation of web services over computer networks. It allows programs running on different operating systems and using different technologies to communicate and share data using standard protocols like **HTTP** and **XML**. SOAP defines a set of rules for structuring messages so that they can be reliably sent and understood between distributed applications.

---

### Key Features of SOAP

1. **Platform and Language Independent** – SOAP messages are formatted in XML, enabling communication between applications on different platforms and programming languages.
    
2. **Structured Messaging** – SOAP defines a standard message structure with an **envelope**, **header**, and **body**, which ensures that data is packaged in a consistent and understandable way.
    
3. **Extensibility** – SOAP supports additional features such as security, transaction handling, and routing through its headers without affecting the message body.
    
4. **Transport Independence** – While HTTP is most common, SOAP can also work over SMTP, TCP, or other protocols.
    
5. **Error Handling** – SOAP provides standardized error reporting via **fault elements**, allowing the receiving application to identify and respond to issues effectively.
    

---

### Example

A client application can use SOAP to request weather data from a web service. The client sends an XML-formatted SOAP message over HTTP to the server, and the server responds with an XML message containing the requested information. This allows interoperability between different systems, e.g., a Java application on Linux communicating with a .NET service on Windows.