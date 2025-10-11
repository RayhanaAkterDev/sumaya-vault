---
class: cse
title: 22 How can NAT help in address depletion?
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
# How NAT Helps in Address Depletion

IP address depletion occurs because the number of devices connected to the Internet is growing rapidly, but the number of **IPv4 addresses** is limited to about 4.3 billion. **NAT (Network Address Translation)** is a technique used in routers and firewalls to **conserve public IP addresses** by allowing multiple private devices to share a single public IP address.

---

**Working Principle:**  

NAT translates **private IP addresses** used within a local network into **public IP addresses** when communicating with external networks, and vice versa. This allows many devices on a local network to access the Internet without each device requiring a unique public IP address. NAT can operate in several ways:

1. **Static NAT:** Maps one private IP to one public IP. Useful for servers needing a fixed public IP.    
2. **Dynamic NAT:** Maps private IPs to public IPs from a pool. Addresses are allocated as needed.    
3. **PAT (Port Address Translation / NAT Overload):** Maps multiple private IPs to a single public IP using **different port numbers**. This is the most common method for conserving IP addresses.

---

**How NAT Prevents Address Depletion:**  

By allowing **hundreds or thousands of private devices** to share **one or a few public IP addresses**, NAT significantly reduces the demand for public IPv4 addresses. This helps organizations connect many devices to the Internet without needing a unique public IP for each device.

---

**Example:**  
In a home network, 10 devices (laptops, smartphones, smart TVs) may have private IP addresses like 192.168.1.x. When these devices access the Internet, the NAT router uses a single public IP (e.g., 203.0.113.5) and translates the private IPs to this public IP with unique port numbers. This way, 10 devices use only **one public IP**, conserving address space.