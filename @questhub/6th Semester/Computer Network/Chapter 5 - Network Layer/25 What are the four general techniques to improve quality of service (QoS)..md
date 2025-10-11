---
class: cse
title: 25 What are the four general techniques to improve quality of service (QoS).
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
# Techniques to Improve Quality of Service (QoS)

Quality of Service (QoS) ensures that multimedia and other critical network traffic meet performance requirements like **bandwidth, delay, jitter, and packet loss**. Several techniques are used to improve QoS in networks, particularly for real-time applications such as video streaming, VoIP, and online gaming.

---

**1. Traffic Shaping:**  
Traffic shaping controls the **rate of data transmission** into the network. By regulating the flow of packets, it prevents network congestion, smooths bursts of traffic, and ensures that high-priority applications receive the necessary bandwidth.

**2. Resource Reservation:**  
Resource reservation allocates **dedicated network resources**, such as bandwidth or buffer space, for specific applications. Protocols like **RSVP (Resource Reservation Protocol)** reserve these resources along the path to guarantee that critical data streams meet QoS requirements.

**3. Priority Scheduling:**  
Priority scheduling assigns different **priority levels to network traffic**. High-priority traffic, like voice or video, is transmitted first, while lower-priority traffic waits. Techniques like **Weighted Fair Queuing (WFQ)** or **Priority Queuing** help manage bandwidth effectively and reduce delay for important data.

**4. Congestion Management and Avoidance:**  
Congestion management techniques monitor network load and take action to **prevent or reduce congestion**, such as dropping low-priority packets, rerouting traffic, or implementing **Active Queue Management (AQM)**. This ensures that important packets are delivered with minimal delay and packet loss.

---

**Example:**  
In a VoIP network, priority scheduling ensures voice packets are sent before large file downloads, resource reservation guarantees sufficient bandwidth for calls, traffic shaping smooths bursts of traffic, and congestion management prevents packet loss during high network load.

