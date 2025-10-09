---
class: cse
title: 10 What different types of architectural styles exist for s/w design.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐
tags:
  - board_2022
---

### Types of Architectural Styles in Software Design

In software design, an architectural style shows how a system is built, how its parts work together, and who does what. It helps organize the system and affects how easy it is to maintain, scale, and run. Different styles are used for different types of software.

1. **Layered Architecture**  
    In a layered architecture, the system is divided into layers, each with a specific responsibility. Higher layers depend on lower layers, but not vice versa. This style promotes separation of concerns, easier maintenance, and scalability. A typical example is the **presentation, business, and data access layers** in enterprise applications.
    
2. **Client-Server Architecture**  
    Client-server architecture divides the system into **clients**, which request services, and **servers**, which provide services. Clients handle user interaction, while servers handle processing and data storage. This style is commonly used in web applications, databases, and networked systems.
    
3. **Pipe-and-Filter Architecture**  
    In this style, data flows through a sequence of **filters** (processing units) connected by **pipes** (data channels). Each filter performs a transformation on the data and passes it to the next. This is suitable for **data processing systems**, compilers, and streaming applications.
    
4. **Event-Driven Architecture**  
    Event-driven architecture organizes the system around **events** and **event handlers**. Components react to events asynchronously, enabling high flexibility and responsiveness. This style is commonly used in **GUIs, real-time systems, and messaging systems**.
    
5. **Microservices Architecture**  
    Microservices architecture structures a system as a set of **independent, loosely coupled services**, each responsible for a specific functionality. Services communicate through APIs. This style improves **scalability, maintainability, and deployment flexibility** in large applications.
    
6. **Repository Architecture**  
    In repository architecture, all system data is stored in a **central repository**, and multiple components access or modify this data. It is widely used in **database systems, version control systems, and content management systems**.
    
7. **Peer-to-Peer (P2P) Architecture**  
    In P2P architecture, each node (peer) can act as both a client and a server. Nodes share resources and communicate directly without a central server. This style is commonly used in **file-sharing networks, blockchain, and distributed computing systems**.
    
8. **Model-View-Controller (MVC) Architecture**  
    MVC architecture separates the system into three components: **Model** (data), **View** (user interface), and **Controller** (business logic). This separation allows independent development, testing, and maintenance of each component, commonly used in **web and desktop applications**.
