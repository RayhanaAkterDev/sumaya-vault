---
class: cse
title: 01 What is API. Explain the uses of API with block diagram.
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2022
topic: Set 01
---

**Definition of API**:

An **Application Programming Interface (API)** is a set of rules, protocols, and tools that allows different software applications to communicate with each other. It acts as an **interface between two software components**, enabling one system to use the functionalities or services of another without knowing its internal details. In simple terms, an API works like a **bridge** that allows applications to talk to each other.

**Block Diagram of API**

```pgsql
+-------------+        API Request        +-------------+  
|             |  --------------------->   |             |  
|   Client    |                           |   API       |  
| (App/User)  |   <---------------------  | (Interface) |  
|             |        API Response       |             |  
+-------------+                           +-------------+  
                                                |  
                                                v  
                                          +-------------+  
                                          |   Server    |  
                                          | (Database / |  
                                          |  Service)   |  
                                          +-------------+  
```

- The **Client Application** (e.g., mobile app or website) sends an **API Request** asking for data or services.    
- The **API Layer** acts as a **bridge**. It receives the request, checks permissions, and forwards it to the server.    
- The **Server/Service Provider** processes the request (accessing database, performing calculation, or executing function).    
- After processing, the **Server sends a Response** back through the API Layer.    
- Finally, the **Client Application** receives the **API Response** and displays or uses the data.

---

### Uses of API

> NOTE: _see exam kit page no. 316 different table_

1. **Software Communication**  
    APIs allow two applications to exchange data easily.  
    _Example: A weather app fetches live weather data from a weather service API._    
2. **Service Integration**  
    APIs integrate external services into applications.  
    _Example: Google Maps API used in delivery or ride-sharing apps for navigation._
3. **Cloud Services**
	APIs are the backbone of cloud computing, giving access to storage, databases, and AI models.
	 _Example: AWS, Azure, and Google Cloud services provide APIs for developers._
4. **Abstraction**  
    Developers can use functionalities without knowing the internal working of a system.  
    _Example: A payment gateway API (like PayPal or Stripe) handles complex banking processes securely._    
5. **Automation**  
    APIs enable tasks to run automatically between systems.  
    _Example: Social media APIs allow auto-posting of content across platforms._    
6. **Platform Independence**  
    APIs make interaction possible across different platforms (web, mobile, cloud).  
    _Example: Travel booking websites use APIs to fetch flight, hotel, and rental data from various providers._    
7. **Advanced Features**  
    APIs give access to powerful tools like AI and machine learning.  
    _Example: Image recognition and natural language processing APIs are used in modern apps._
8. **Web and Mobile Applications**  
	 APIs allow mobile or web apps to fetch data from servers.  
	 _Example: Weather apps use APIs to get live weather data._