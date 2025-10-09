---
class: cse
title: 11 Explain congestion control. What are the affects of congestion?
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
### Congestion Control in Computer Networks

Congestion control is a mechanism used in computer networks to manage the flow of data and prevent the network from becoming overloaded. Congestion occurs when the demand for network resources, such as bandwidth, buffer space, or processing power, exceeds the available capacity, causing performance degradation. Congestion control techniques aim to regulate the data transmission rate, manage queue lengths in routers, and avoid excessive packet loss or delays. These techniques are essential for maintaining network efficiency, stability, and quality of service (QoS), especially in high-traffic networks where multiple devices or applications compete for limited resources. Congestion control ensures that the network can handle traffic smoothly, prevent collapse, and provide reliable communication for all users.

---

**Effects of Congestion:**

1. **Increased Packet Loss:** When a network is congested, buffers in routers and switches become full, causing incoming packets to be dropped. This packet loss forces retransmissions, which add even more traffic to the network and worsen congestion.
    
2. **Longer Transmission Delays:** Congested networks cause packets to wait in queues for longer periods before being transmitted. This leads to higher end-to-end latency, slowing down communication and affecting time-sensitive applications like VoIP, online gaming, and video conferencing.
    
3. **Reduced Throughput:** As congestion increases, the network’s ability to deliver data efficiently decreases. Although more data may be injected into the network, fewer packets reach their destination successfully, lowering overall throughput and performance.
    
4. **Network Instability:** Severe congestion can cause traffic patterns to fluctuate unpredictably, with bursts of packet loss followed by temporary recoveries. This instability can result in oscillations in network load, inefficient use of resources, and, in extreme cases, network collapse.
    
5. **Degraded Quality of Service (QoS):** Applications that require steady and predictable performance, such as video streaming, online gaming, and voice communication, suffer under congestion. Users may experience buffering, jitter, dropped calls, or slow downloads, significantly reducing user experience.
    
6. **Increased Retransmissions:** Because packets are lost or delayed, retransmissions become necessary. These retransmissions consume additional bandwidth and processing resources, creating a feedback loop that further increases network congestion.
    
7. **Higher CPU and Router Load:** Congested networks force routers and switches to handle more traffic than they are designed for, increasing CPU utilization and memory usage. This can slow down the devices themselves, leading to further delays and instability in the network.