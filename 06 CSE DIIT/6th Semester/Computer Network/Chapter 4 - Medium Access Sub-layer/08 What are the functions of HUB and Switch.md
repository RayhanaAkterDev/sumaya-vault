---
class: cse
title: 08 What are the functions of HUB and Switch?
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - CN/Ch4
---

### **Functions of Hub and Switch**

1. **Hub** – A hub is a basic networking device that **connects multiple devices** in a LAN, allowing them to communicate. Its main function is to **receive data from one device and broadcast it to all other connected devices**, regardless of the intended destination. Hubs operate at the **physical layer (Layer 1)** of the OSI model and **do not filter, manage, or prioritize traffic**. Because they broadcast data to all ports, hubs can lead to **network congestion, collisions, and lower overall efficiency**. Hubs are simple, inexpensive, and mainly used in **small, legacy, or less demanding networks** where high performance is not critical.
---

2. **Switch** – A switch is a more intelligent networking device that **connects multiple devices** in a LAN and **forwards data only to the intended recipient device**. It operates at the **data link layer (Layer 2)** and uses **MAC addresses** to determine the correct destination for each data frame. By doing this, switches **reduce collisions and improve network efficiency**, as each port effectively forms its own collision domain. Many modern switches also support advanced features such as **VLANs (Virtual LANs), Quality of Service (QoS), port security, and even Layer 3 routing**, making them suitable for **larger, complex, and high-performance networks**. Switches are widely used in modern LANs to ensure **fast, secure, and efficient communication** between devices.
