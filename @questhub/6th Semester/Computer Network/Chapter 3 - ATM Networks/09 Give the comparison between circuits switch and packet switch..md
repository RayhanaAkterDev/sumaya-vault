---
class: cse
title: 09 Give the comparison between circuits switch and packet switch.
course:
  - Computer Network
chapter:
  - Chapter 3 - ATM Networks
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - CN/Ch3
---

**Comparison between Circuit Switching and Packet Switching**

Circuit switching and packet switching are two fundamental methods of data communication. They differ in how data is transmitted, how network resources are used, and the efficiency and reliability of communication.

|Feature|Circuit Switching|Packet Switching|
|---|---|---|
|**Path**|A dedicated end-to-end path is established before communication starts.|No dedicated path; data is divided into packets, which are sent independently.|
|**Resource Utilization**|Resources are reserved for the entire duration, even during idle periods, leading to inefficient use.|Network resources are shared among multiple users, improving efficiency, especially for bursty traffic.|
|**Transmission**|Data flows continuously once the circuit is established, suitable for real-time communication.|Data is transmitted in discrete packets, which may take different paths and be reassembled at the destination.|
|**Setup Time**|Requires setup time to establish a dedicated circuit before communication.|No setup time is required; packets can be sent immediately.|
|**Reliability**|Provides a predictable and continuous connection, but if the dedicated path fails, communication is interrupted.|More fault-tolerant; packets can be rerouted if a link fails.|
|**Handling Bursty Data**|Less efficient for irregular or bursty traffic; resources remain idle during pauses.|Highly efficient for bursty or irregular data.|
|**Cost**|Higher cost due to dedicated resource allocation.|Lower cost as resources are shared dynamically.|
|**Applications**|Traditional telephone networks, some leased line communications.|Internet, computer networks, VoIP, video streaming.|