---
class: cse
title: 04 What are the functions of router, gateway and bridge?
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2021
  - board_2022
---

### **Functions of Router, Gateway, and Bridge**

1. **Router** – A router is a networking device that connects **two or more different networks**, such as LANs, WANs, or the Internet. Its main function is to **forward data packets** from the source network to the destination network by analyzing the **IP address** of each packet. Routers also determine the **best path for data transmission** using routing tables and algorithms. In addition to routing, they **manage network traffic, prevent congestion**, and often provide **security features** such as firewalls or NAT (Network Address Translation). Routers operate at the **network layer (Layer 3)** of the OSI model.

---

2. **Gateway** – A gateway acts as a **bridge between networks that use different protocols or architectures**. It can translate data from one protocol to another, allowing devices on incompatible networks to communicate. For example, a gateway can connect a TCP/IP network to a network using a legacy protocol. Gateways often perform **protocol conversion, data format translation, and sometimes encryption/decryption**, making them essential for interoperability between heterogeneous networks. Gateways operate at **multiple layers** of the OSI model, depending on their function.

---

3. **Bridge** – A bridge connects **two or more segments of the same type of network** to make them appear as a single logical network. It **filters and forwards data frames** based on MAC addresses, ensuring that traffic is only sent to the segment where the destination device resides. This helps **reduce network congestion** and **divide collision domains** while maintaining network transparency. Bridges operate at the **data link layer (Layer 2)** of the OSI model. There are also **transparent bridges**, which learn the MAC addresses automatically, and **source-routing bridges**, which rely on the sender to specify the path.
