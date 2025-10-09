---
class: cse
title: 03 Sketch the frame relay frame format and describe its different fields.
course:
  - Computer Network
chapter:
  - Chapter 2 - Frame Relay
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2019
  - board_2020
Note: checkout exam kit page no. 164 for the figure
topic: "Topic 4: X.25 and Frame Relay"
---
## Frame Relay Frame Format and Description of Fields

The Frame Relay frame structure is based on the LAPD (Link Access Procedure for the D-channel) protocol and is used to transmit data efficiently over a Frame Relay network. Each frame consists of several fields that provide addressing, control, and error checking. A simplified representation of the frame is:

`Flag | Address | Information | FCS | Flag`

The **Address field** itself contains multiple subfields that manage virtual circuits and congestion control.

---

### Description of Fields

1. **Flag**  
    The Flag field marks the **beginning and end of a frame**. It uses a fixed bit pattern `01111110` (or hexadecimal `7E`) to help the receiver detect frame boundaries and distinguish separate frames in the data stream.
    
2. **Address Field**  
    The Address Field contains the **Data Link Connection Identifier (DLCI)**, which identifies the virtual circuit between the Data Terminal Equipment (DTE) and the network switch. It also includes several control subfields:
    
    - **Extended Address (EA):** Indicates whether the current byte is the last addressing byte. If EA = 1, it marks the final DLCI octet.
        
    - **Command/Response (C/R):** This bit follows the most significant DLCI byte and distinguishes command or response frames.
        
    - **Congestion Control Bits:** These consist of three bits—**FECN** (Forward Explicit Congestion Notification), **BECN** (Backward Explicit Congestion Notification), and **DE** (Discard Eligibility)—which help manage congestion in the network.
        
3. **Data (Information) Field**  
    The Data field carries the **user information or payload**. This is a variable-length field that can include up to 16,000 octets of data, encapsulating higher-layer protocol information for transmission across the network.
    
4. **FCS (Frame Check Sequence)**  
    The FCS field ensures the **integrity of the transmitted data**. A cyclic redundancy check (CRC) value is computed by the sender and verified by the receiver to detect any errors during transmission.
