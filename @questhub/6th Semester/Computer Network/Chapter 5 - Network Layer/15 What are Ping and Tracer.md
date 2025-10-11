---
class: cse
title: 15 What are Ping and Tracer?
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2022
---
### Ping and Tracer – Detailed Definitions

Ping is a network utility used to **check the availability and responsiveness of a host** on an IP network. It works by sending **ICMP (Internet Control Message Protocol) Echo Request packets** to the target device and waits for **ICMP Echo Reply packets** in return. Ping provides information about **network connectivity, round-trip time (latency), and packet loss**, which helps in diagnosing network problems. It is widely used by network administrators to verify whether a particular device (like a server, router, or computer) is reachable over the network and to measure the **speed and reliability** of the connection. For example, using `ping google.com` allows one to check if Google’s server is reachable and how fast the network responds.
  
Tracer, or Traceroute, is a network diagnostic tool that **traces the exact path** that data packets take from the source to a destination across an IP network. It works by sending packets with gradually increasing **Time-To-Live (TTL) values**, causing each intermediate router to respond with a **Time Exceeded message**. This allows the source device to identify every router or gateway the packets pass through, along with the **time delay at each hop**. Traceroute is especially useful for locating **network bottlenecks, delays, or failures** along the path. For instance, `traceroute google.com` (on Linux/macOS) or `tracert google.com` (on Windows) shows the full route and response times to reach Google’s server, helping diagnose routing issues or slow network links.