---
class: cse
title: 14 Describe CGI (Common Gateway Interface)
course:
  - Embedded System Programming
chapter:
  - "ch4: Web server and API"
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - ESP/Ch4
---

### **Common Gateway Interface (CGI)**

**Common Gateway Interface (CGI)** is a standard protocol that allows a **web server to communicate with external programs or scripts** to generate dynamic content for web pages. When a client sends a request (like submitting a form), the web server executes a CGI script, which processes the input, performs necessary operations, and sends back the result (HTML, JSON, or other data) to the client’s browser.

CGI enables web applications to **respond to user input**, interact with databases, perform calculations, and produce customized content dynamically, instead of serving the same static page to every visitor. Scripts used in CGI can be written in languages like **Perl, Python, PHP, or C**, making it flexible and widely supported.

---

### **Key Features of CGI**

1. **Dynamic Content Generation:**  
    CGI allows web servers to create web pages dynamically based on user input or other factors.
    
2. **Server-Side Processing:**  
    Scripts are executed on the server, ensuring that the client receives only the output and not the underlying code.
    
3. **Support for Multiple Languages:**  
    CGI scripts can be written in Perl, Python, C, PHP, or other compatible languages.
    
4. **Form Handling:**  
    CGI can process data submitted via HTML forms, such as login details, surveys, or feedback.
    
5. **Database Interaction:**  
    CGI scripts can access databases to retrieve, update, or manipulate data dynamically.
    
6. **Platform Independence:**  
    CGI is supported by most web servers and operating systems, allowing scripts to be executed across different platforms.
    
7. **Security and Logging:**  
    Properly configured CGI scripts can validate input, control execution, and log user interactions for monitoring and troubleshooting.
    

---

✅ **Example:**  
When a user searches for a product on an **online shopping site**, a CGI script can receive the search term, query the database for matching products, and dynamically generate an HTML page displaying the results.
