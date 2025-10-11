---
class: cse
title: 11 SNMP;
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
tags:
  - CN/Ch7
---
# SNMP (Simple Network Management Protocol)

SNMP is a **standardized protocol used for monitoring, managing, and controlling network devices** in an organized and efficient manner. It enables network administrators to collect real-time information about network performance, detect faults, and configure devices such as routers, switches, servers, and printers. By providing a structured framework through which devices can communicate status and performance data, SNMP helps maintain the reliability, efficiency, and security of large networks.

**Example:**  
A network administrator can use SNMP to monitor CPU usage, memory utilization, and network traffic on all routers, switches, and servers, and receive alerts if any device goes down or exceeds thresholds.

---

**Key Points:**

1. SNMP operates over **UDP**, typically using ports 161 (for management) and 162 (for traps).    
2. Works on a **manager-agent model**, where the manager queries devices (agents) and receives responses or alerts.    
3. Uses a **Management Information Base (MIB)** to define the objects and data that can be monitored or controlled.    
4. Helps in **fault detection, performance monitoring, and network configuration**.
5. Lightweight and widely supported, making it suitable for large and heterogeneous networks.

