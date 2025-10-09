---
class: cse
title: 18 Mention the differences between connectionless and connection oriented network system
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2019
  - CN/Ch1/board_2021
  - CN/Ch1/board_2022
---

## Differences Between Connectionless and Connection-Oriented Network Systems

|**Feature**|**Connection-Oriented System**|**Connectionless System**|
|---|---|---|
|**Connection Setup**|A connection is established between sender and receiver before any data is transmitted.|No prior connection is needed; data is sent immediately without setup.|
|**Communication Style**|Works on a **handshake** model (e.g., TCP’s 3-way handshake) to begin communication.|Works on a **fire-and-forget** model — data is sent without verifying readiness.|
|**Reliability**|Ensures **reliable transmission** by checking for errors, acknowledgments, and packet ordering.|Does **not guarantee delivery**, order, or error correction — may lose or duplicate data.|
|**Data Path**|Data packets follow a **predefined and consistent path** throughout the session.|Each packet may take a **different route** through the network independently.|
|**Overhead & Resources**|Involves **higher overhead** due to connection setup, maintenance, and teardown processes.|Uses **less overhead**, making it more resource-efficient and suitable for fast transfers.|
|**Speed**|Generally **slower**, as it focuses on reliability and proper sequencing.|Generally **faster**, as it avoids delays from setup and acknowledgments.|
|**Error Handling**|Built-in error detection and correction mechanisms within the protocol (e.g., retransmission).|Minimal or no built-in error handling; left to the **application** if needed.|
|**Use Cases**|Ideal for tasks like file transfers, emails, and web page loading where data must be accurate.|Preferred for streaming, VoIP, online gaming, where speed is more important than accuracy.|
|**Protocol Example**|**TCP (Transmission Control Protocol)** is the most common example.|**UDP (User Datagram Protocol)** is widely used for connectionless communication.|
|**Acknowledgment System**|Uses **ACKs** (acknowledgments) to confirm successful delivery of each packet.|No acknowledgment is sent; sender assumes data reaches the destination.|