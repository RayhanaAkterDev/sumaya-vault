---
class: cse
title: 26 Describe the various approaches for controlling network congestion.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-07
status: pending 🛑
tags:
  - CN/Ch5
---
# Approaches for Controlling Network Congestion

Network congestion occurs when the demand for network resources exceeds the available capacity, leading to **packet loss, increased delay, and degraded performance**. Controlling congestion is crucial to maintain reliable and efficient network operation. Several approaches are used to prevent, avoid, or control congestion in networks.

---

**1. Congestion Prevention:**  
Congestion prevention techniques **proactively manage network resources** to avoid congestion before it occurs. This includes **admission control**, where the network limits the number of active connections, and **traffic shaping**, which regulates data transmission rates to smooth out bursts and prevent overload.

**2. Congestion Avoidance:**  
Congestion avoidance uses **feedback mechanisms** to detect early signs of congestion and take corrective action. For example, routers can monitor **queue lengths** and use algorithms like **Random Early Detection (RED)** to drop packets selectively, signaling sources to reduce their transmission rate before congestion becomes severe.

**3. Congestion Detection and Control:**  
Congestion detection identifies **existing congestion** using network indicators such as **high packet loss, long queue lengths, or excessive delays**. Once detected, control measures are applied, such as **reducing the sending rate**, rerouting traffic, or **prioritizing important packets** to alleviate the congestion.

**4. Traffic Management and Scheduling:**  
Traffic management techniques like **priority queuing, weighted fair queuing, and resource allocation** ensure that high-priority traffic receives timely service even during congestion. These techniques prevent critical applications from being affected while controlling overall network load.

---

**Example:**  
In an online video streaming service, congestion prevention limits the number of concurrent high-definition streams, congestion avoidance drops non-essential packets when the router queue is filling, congestion control slows down sending rates from certain users, and traffic scheduling ensures live video streams get priority over downloads.