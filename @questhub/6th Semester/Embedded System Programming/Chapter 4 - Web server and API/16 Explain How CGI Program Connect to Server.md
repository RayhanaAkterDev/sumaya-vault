---
class: cse
title: 16 Explain How CGI Program Connect to Server?
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

### **How a CGI Program Connects to a Server**

A **CGI (Common Gateway Interface) program** allows a web server to execute external scripts or programs to generate dynamic content. The process ensures that the client receives customized output while keeping the underlying logic on the server.

---

### **Step-by-Step Explanation**

1. **Client Sends Request:**  
    The process begins when a user interacts with a web page, such as submitting a form, clicking a link, or performing a search. The browser sends an HTTP request to the web server, including any input data the user has provided.
    
2. **Server Identifies CGI Request:**  
    The web server examines the request URL or file extension (commonly `.cgi`, `.pl`, or `.exe`) to determine that it should be handled by a CGI program. If it is a CGI request, the server prepares to execute the corresponding script.
    
3. **Passing Environment Variables and Input Data:**  
    The server sets environment variables that convey request details to the CGI program, such as the request method (GET or POST), query string, client IP, and server information. For POST requests, the server passes form data via standard input so the CGI script can access it.
    
4. **Execution of CGI Program:**  
    The server launches the CGI script in a separate process. The program reads the input data, performs necessary operations—such as calculations, business logic, or database queries—and prepares output in the required format (usually HTML, XML, or JSON).
    
5. **Returning Output to Server:**  
    The CGI program writes its output to **standard output**, which the web server captures. This output includes headers (like `Content-Type`) and the content to be displayed in the client’s browser.
    
6. **Server Sends Response to Client:**  
    After capturing the CGI program’s output, the web server sends it as the HTTP response to the client’s browser. The user sees the dynamically generated web page or results based on their input.
    
7. **Logging and Termination:**  
    The server may log the transaction for monitoring or debugging purposes. Once the CGI program finishes execution, its process terminates, freeing server resources for other requests.
    
8. **Security and Validation:**  
    Throughout this process, the server and CGI program should validate input to prevent malicious data from causing security breaches, such as SQL injection or unauthorized access. Proper configuration ensures that scripts run in a controlled environment.
