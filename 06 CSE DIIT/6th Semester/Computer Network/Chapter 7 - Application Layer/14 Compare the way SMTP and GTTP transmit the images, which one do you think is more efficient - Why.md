---
class: cse
title: 14 Compare the way SMTP and GTTP transmit the images, which one do you think is more efficient? Why?
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
# Comparison of SMTP and HTTP for Transmitting Images

|Feature|SMTP (Email Transmission)|HTTP (Web Transmission)|
|---|---|---|
|**Transmission Method**|Images are sent as part of an email using **MIME encoding** (usually Base64), converting binary data to text.|Images are sent in **binary form** directly from server to client.|
|**Data Size**|Image size increases by ~33% due to Base64 encoding.|No size increase; original binary size is transmitted.|
|**Speed**|Slower due to **store-and-forward** through multiple mail servers.|Faster due to direct client-server connection.|
|**Overhead**|High overhead from MIME headers, encoding, and multiple hops.|Minimal overhead; mainly HTTP request and response headers.|
|**Efficiency for Large Files**|Less efficient, slower transfer, more bandwidth required.|More efficient; allows **progressive download** and faster rendering.|
|**Use Case**|Sending images as part of emails or attachments.|Real-time retrieval of images on websites or web applications.|
