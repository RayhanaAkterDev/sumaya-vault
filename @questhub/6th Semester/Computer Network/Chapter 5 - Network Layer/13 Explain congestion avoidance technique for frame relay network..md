---
class: cse
title: 13 Explain congestion avoidance technique for frame relay network.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2019
---
### Congestion Avoidance Technique for Frame Relay Network

Congestion avoidance in a Frame Relay network is a set of mechanisms designed to prevent network congestion before it occurs, rather than reacting after congestion has already happened. Since Frame Relay is a high-speed packet-switched network that relies on virtual circuits, uncontrolled traffic can quickly overload switches, causing packet loss, delays, and reduced network performance. Congestion avoidance techniques monitor network load and regulate traffic flow to ensure smooth operation.

---

**Congestion Avoidance Techniques:**

1. **Forward Explicit Congestion Notification (FECN):**    
    - FECN is a bit in the Frame Relay frame header that indicates congestion in the direction of the frame.        
    - When a switch detects congestion, it sets the FECN bit, signaling the receiving device that congestion is occurring in the path.        
    - The receiver can then inform the sender to slow down transmission, preventing further congestion.

2. **Backward Explicit Congestion Notification (BECN):**    
    - BECN is another bit in the frame header used to notify the sender about congestion in the reverse direction.        
    - When a switch experiences congestion, it sets the BECN bit in frames traveling back to the sender.        
    - The sender, upon receiving BECN-marked frames, reduces its data transmission rate to alleviate congestion.

3. **Committed Information Rate (CIR):**    
    - Frame Relay networks often use a Committed Information Rate, which guarantees a minimum bandwidth for a virtual circuit.        
    - Traffic exceeding the CIR is considered "excess" and may be delayed or discarded, helping prevent congestion in the network.

4. **Traffic Policing:**    
    - Traffic entering the network is monitored against agreed limits.        
    - Frames exceeding the committed rate may be dropped or marked for lower priority, preventing excessive load on switches and maintaining network stability.