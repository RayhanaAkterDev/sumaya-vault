---
class: cse
title: 07 State the purpose of FECN, BECN fields.
course:
  - Computer Network
chapter:
  - Chapter 2 - Frame Relay
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2017
---

In Frame Relay networks, the **FECN (Forward Explicit Congestion Notification)** and **BECN (Backward Explicit Congestion Notification)** fields are used to **manage and control network congestion**, ensuring smooth data transmission.

- **FECN:** This field is set by a Frame Relay switch when it detects congestion **in the direction the frame is traveling**. When the receiving device sees the FECN bit set, it becomes aware that the path is congested and can take appropriate action, such as notifying the sender or adjusting its own processing. This helps prevent packet loss and maintains efficient traffic flow.
    
- **BECN:** This field works in the opposite direction. It is set by the switch to indicate that **congestion exists in the reverse direction** of the frame’s travel. The sending device can then slow down its transmission rate to avoid worsening the congestion.
    

By using **FECN and BECN**, Frame Relay provides a mechanism for **explicit congestion signaling**, allowing both sender and receiver to react proactively, maintain performance, and reduce packet drops without relying solely on retransmission mechanisms.
