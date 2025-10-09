---
class: cse
title: 09 Explain the seven layers of OSI system with diagram
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
importance: ⭐⭐
tags:
  - board_2022
topic: Topic 02 - Reference Models (OSI and TCP/IP)
---

## 7 Layers of OSI System

The OSI model is a way to understand how data moves through a network. It divides communication into seven layers, each with a clear role that helps devices talk to each other without confusion.

**1. Physical Layer:** This is the foundation where actual data travels as electrical or optical signals through cables or wireless. It deals with hardware like cables, connectors, and network cards. Without this layer, no data can move at all.

**2. Data Link Layer:** This layer takes raw bits from the physical layer and turns them into frames, ensuring that data between devices on the same network is sent correctly. It uses MAC addresses to identify devices and checks for errors during transmission.

**3. Network Layer:** Here, data is packed into packets with logical addresses called IP addresses. This layer decides the best route to send data across multiple networks, like guiding a letter through the postal system.

**4. Transport Layer:** The transport layer makes sure the data arrives safely and in order. It splits large data into smaller pieces, handles error checking, and controls how fast data is sent. TCP is reliable and waits for confirmation; UDP is faster but less certain.

**5. Session Layer:** This layer manages the connections between computers. It starts and ends communication sessions, keeping the conversation organized, like a phone operator connecting and disconnecting calls.

**6. Presentation Layer:** The presentation layer translates data into a common format so both sender and receiver understand it. It also handles encryption to keep data secure and compression to reduce size for faster transmission.

**7. Application Layer:** The top layer where users interact with the network. It provides services like web browsing, email, and file sharing using protocols such as HTTP and FTP. This layer makes the network useful for everyday applications.


![[96fe0be1f5e8f2e6cfbc6d6cd8950f34.jpg]]

The word **“synch”** is an **informal abbreviation** of “synchronize” or "synchronization.”
