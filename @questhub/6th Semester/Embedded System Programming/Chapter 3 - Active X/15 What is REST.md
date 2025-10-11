---
class: cse
title: 15 What is REST?
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - ESP/Ch3
---

### Definition of REST

**REST (Representational State Transfer)** is an architectural style for designing networked applications. It allows systems to communicate over the web using standard HTTP methods such as **GET, POST, PUT, and DELETE**. REST focuses on **stateless communication**, meaning each request from a client to a server contains all the information needed to process it, without relying on stored context on the server.

REST is widely used because it is **lightweight, scalable, and flexible**, making it ideal for web services, mobile apps, and cloud-based applications. REST APIs allow clients to perform operations on resources, which are represented in formats like **JSON or XML**, making data exchange simple and consistent.

---

### Example

A REST API for a library system might allow a client to fetch details of a book using a **GET** request (`/books/123`), add a new book with a **POST** request, update book details with **PUT**, or delete a book with **DELETE**.