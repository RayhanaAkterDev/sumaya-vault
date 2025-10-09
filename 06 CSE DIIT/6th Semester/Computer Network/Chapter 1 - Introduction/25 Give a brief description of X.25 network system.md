---
class: cse
title: 25 Give a brief description of X.25 network system]
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-08-05
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2020
  - board_2019
  - board_2018
topic: "Topic 4: X.25 and Frame Relay"
---

## X.25 network system

**X.25 network system** is an early packet-switched wide area network (WAN) protocol standard developed by the ITU-T (International Telecommunication Union – Telecommunication Standardization Sector). It provides reliable data communication over over public data networks by using virtual circuits. It operates at the **physical, data link, and network layers** of the OSI model and manages the establishment, maintenance, and termination of virtual circuits between devices.

X.25 breaks data into packets, sends them through a series of switches, and ensures error detection and correction, making it suitable for noisy or unreliable telephone lines. It was widely used before newer technologies like Frame Relay and IP networks became popular.

---

### **Main Characteristics of X.25**

1. **Packet-Switched Technology:** X.25 divides data into small packets that travel independently, using bandwidth efficiently.
    
2. **Virtual Circuits:** Communication uses logical paths called virtual circuits, either permanent (PVC) or switched (SVC), to ensure packets arrive in order.
    
3. **Error Detection and Correction:** Strong error detection and correction at data link and network layers makes X.25 reliable over poor-quality lines.
    
4. **Layer Coverage:** X.25 works at the physical layer (X.21), data link layer (LAPB), and network layer, leaving higher layers to applications.
    
5. **Connection-Oriented Service:** A virtual circuit must be established before data transfer, ensuring reliable delivery.
    
6. **Flow Control:** Sliding window techniques prevent receiver overflow and maintain smooth transmission.
    
7. **Performance and Speed:** Designed for low-speed links (2.4 kbps to 64 kbps), suitable for telephone lines.
    
8. **Applications:** Used in banking, airline reservation, and financial systems from the 1970s–1990s where reliability was more important than speed.