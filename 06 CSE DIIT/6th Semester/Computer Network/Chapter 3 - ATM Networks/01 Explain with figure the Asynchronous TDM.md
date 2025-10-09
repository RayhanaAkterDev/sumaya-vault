---
class: cse
title: 01 Explain with figure the Asynchronous TDM
course:
  - Computer Network
chapter:
  - Chapter 3 - ATM Networks
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2019
  - board_2020
---

## Asynchronous Time Division Multiplexing (ATDM)

**Asynchronous Time-Division Multiplexing (ATDM)**, also called statistical TDM (STDM), is a method where time slots are assigned to devices only when they have data to send. Unlike synchronous TDM, which gives every device a fixed slot regardless of activity, ATDM only uses slots for active devices. This makes it more efficient for irregular or bursty data. Each frame contains an **address field** to identify the device and a **data field** for its information. Devices with no data are skipped, saving bandwidth and reducing wastage.

---

### Key Features of ATDM

- Efficient bandwidth utilization: Only active devices are allocated slots, preventing wastage.    
- Suitable for bursty or irregular data traffic.    
- Requires additional address information in each slot.    
- More complex circuitry and processing compared to synchronous TDM.    
- May introduce variable delays, depending on the number of active devices.    

**Difference from Synchronous TDM:** While synchronous TDM wastes bandwidth during idle periods, ATDM eliminates this by dynamically assigning slots. However, this flexibility increases frame overhead and design complexity.

---

### ATDM Frame Structure

![[atdm2.jpg]]   

![[atdm1.jpg]]

+-------+-------+-------+-------+  
| Addr1 | Data1 | Addr2 | Data2 |  
+-------+-------+-------+-------+  

- **Addr1, Addr2, …** → Identifiers of active devices sending data in that frame    
- **Data1, Data2, …** → Corresponding data from each device    

> **Working:**

1. A multiplexer checks which input lines have data ready.    
2. It assigns slots only to active lines and includes their addresses in the frame.    
3. The de-multiplexer at the receiver reads the address and delivers the data to the correct output.

---

### Working of Asynchronous TDM

1. **Buffering:** Each input line stores data in a buffer while waiting for transmission.    
2. **Dynamic Scanning:** The multiplexer continuously scans all input buffers and identifies lines with data ready to send.    
3. **Frame Building:** Active input lines are assigned time slots dynamically. Each slot contains the device’s address and its data. This allows the frame to efficiently carry only the active data.
4. **Transmission:** The assembled frame is sent over the high-speed communication link.    
5. **Demultiplexing:** At the receiver, the de-multiplexer reads the address field of each slot and forwards the data to the correct output line.
