---
class: cse
title: 02 Why CSMD/CD is not applicable for Wireless LAN?
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2022
---

### **Why CSMA/CD is Not Applicable for Wireless LAN**

In wired Ethernet networks, CSMA/CD works effectively to detect and handle collisions. However, in wireless LANs, the same method cannot be applied due to the unique characteristics of wireless communication.

1. **Collision Detection Problem** – In wireless networks, a station cannot reliably detect collisions while transmitting because the **signal strength of its own transmission is much stronger** than signals from other stations, making it difficult to sense overlapping transmissions.
    
2. **Hidden Node Problem** – Two stations may be out of each other’s range but still communicate with the same access point. If both transmit simultaneously, a collision occurs at the access point, but the stations cannot detect it.
    
3. **Exposed Node Problem** – A station may sense another nearby transmission and unnecessarily defer its own transmission, even though sending would not cause a collision. This reduces efficiency.
    
4. **Signal Attenuation and Interference** – Wireless signals are affected by **attenuation, fading, and interference** from obstacles or other devices. These factors make it difficult to distinguish between a collision and natural signal loss.
    
5. **No Dedicated Medium** – Unlike wired LANs, wireless networks **share a broadcast medium without physical isolation**, so stations cannot sense all ongoing transmissions effectively.
    
6. **Alternative Approach Needed** – Due to these challenges, wireless LANs use **CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)**, which **prevents collisions before they occur** instead of detecting them after transmission.
