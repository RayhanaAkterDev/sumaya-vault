---
class: cse
title: 12 What is traffic shipping in congestion control? Describe traffic shipping algorithm in congestion control.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2018
---
### Traffic Shaping in Congestion Control

Traffic shaping is a congestion control technique used in computer networks to regulate the flow of data packets entering a network. It ensures that data is transmitted at a controlled rate, preventing sudden bursts from overloading network resources like bandwidth and buffers. By smoothing traffic and enforcing a predictable data flow, traffic shaping helps reduce packet loss, minimize delays, and maintain overall network efficiency. It is especially useful for networks with multiple users or applications competing for limited resources, and it helps maintain the quality of service (QoS) for time-sensitive applications such as video streaming, VoIP, and online gaming.

---

### Traffic Shaping Algorithm in Congestion Control

Traffic shaping algorithms control the rate at which data packets are sent into a network to prevent congestion and ensure smooth traffic flow. These algorithms regulate traffic by delaying or buffering packets when the transmission rate exceeds a predefined limit, helping maintain network stability and improve performance. The two most commonly used traffic shaping algorithms are:

1. **Leaky Bucket Algorithm:**    
    - The network is treated as a bucket that leaks at a constant rate.        
    - Incoming packets are added to the bucket. If packets arrive faster than the leak rate, excess packets are either queued or dropped.        
    - Packets are transmitted at a steady, fixed rate, which smooths bursty traffic and prevents sudden congestion.        
    - **Use Case:** Suitable for networks requiring a constant output rate, such as voice or video calls.
        
2. **Token Bucket Algorithm:**    
    - Tokens are generated at a fixed rate and stored in a bucket.        
    - A packet can be transmitted only if a token is available. If no tokens are present, packets are delayed until tokens accumulate.        
    - This algorithm allows short bursts of traffic while maintaining a controlled average transmission rate.        
    - **Use Case:** Useful for networks that need flexibility to handle occasional traffic spikes, like web browsing or file transfers.