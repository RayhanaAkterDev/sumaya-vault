---
class: cse
title: 04 What is DNS? Why do you think DNS uses UDP instead of TCP for its query and response messages?
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2018
---
# What is DNS?

The **Domain Name System (DNS)** is a hierarchical and distributed naming service that translates human-readable domain names into machine-readable IP addresses. Since users prefer easy names like _www.google.com_ rather than long numeric addresses such as _142.250.190.14_, DNS acts as the “phonebook of the internet,” enabling seamless communication between people and computers.

---

# Why DNS Uses UDP Instead of TCP for Queries and Responses

DNS primarily uses **UDP (User Datagram Protocol)** on port 53 for query and response messages. While TCP is more reliable, UDP is chosen in most cases because it better suits the nature of DNS communication. The main reasons are:

1. **Faster Communication**  
    UDP is connectionless, meaning it does not require setting up and tearing down a connection like TCP. This makes DNS queries and responses much faster, which is important since DNS is used before almost every internet communication.
    
2. **Small Message Size**  
    Most DNS queries and responses are small (less than 512 bytes in the traditional standard, and now often under 1280 bytes with EDNS). Such small packets can easily fit within a single UDP datagram, eliminating the need for TCP’s overhead.
    
3. **Reduced Overhead**  
    TCP requires acknowledgments, sequencing, and error-checking for each packet, which adds extra overhead. For DNS, where speed is critical and occasional packet loss can simply trigger a retransmission, UDP provides a lightweight and efficient solution.
    
4. **Scalability**  
    Because DNS servers handle millions of queries per second worldwide, using UDP reduces resource usage. If TCP were used for every query, it would overload servers with connection management, slowing down the entire system.
    
5. **Fallback to TCP for Larger Responses**  
    DNS is not limited to UDP. If a response is too large to fit in a single UDP packet (for example, with DNSSEC or zone transfers), DNS automatically switches to TCP. This ensures both efficiency (with UDP) and reliability (with TCP when needed).
    
6. **Lower Latency for Real-Time Applications**  
    DNS resolution happens before almost every internet activity like web browsing, gaming, or video streaming. Using UDP reduces latency, ensuring faster access to resources.
       
7. **Stateless Nature**  
    UDP is stateless, meaning the server does not need to maintain session information for every client. This significantly reduces memory and CPU usage, allowing DNS servers to handle millions of queries efficiently.
    
8. **Sufficient Reliability Through Retransmission**  
    Even though UDP itself does not guarantee delivery, DNS clients are designed to retransmit queries if no response is received. This makes UDP reliable enough for DNS purposes without the heavy overhead of TCP.