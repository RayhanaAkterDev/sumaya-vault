---
class: cse
title: 13 Describe API's Working Method.
course: Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - ESP/Ch3
---

### API’s Working Method

> NOTE: _see exam kit page no. 307 different table_

1. **Client Sends Request**  
    The process starts when a client application, such as a web app, mobile app, or another program, sends a request to the API. The request specifies the action the client wants to perform, like retrieving data, updating information, or executing a function. The request must follow the API’s defined format and protocol.
    
2. **API Receives and Processes Request**  
    The API acts as an intermediary between the client and the server. It validates the request, checks for authentication and permissions, and determines which server or service should handle it. This ensures secure and controlled access to resources.
    
3. **Server Performs Action**  
    The server or service receives the request from the API and executes the required operation. This may include querying a database, performing calculations, or processing data. The server prepares a response based on the requested action.
    
4. **API Sends Response to Client**  
    Once the server completes the task, the API receives the response and forwards it to the client application. The response contains the requested data, confirmation of an action, or error messages if something went wrong.
    
5. **Client Uses the Response**  
    Finally, the client application receives the response from the API. It uses the data to display information to the user, perform further processing, or trigger other operations within the application.
    

---

**Example:**  
A weather app requests the current temperature for a city. First, the app sends a request to the weather API. The API validates the request and forwards it to the server. The server retrieves the temperature, sends it back to the API, and the API returns it to the app, which displays it to the user.
