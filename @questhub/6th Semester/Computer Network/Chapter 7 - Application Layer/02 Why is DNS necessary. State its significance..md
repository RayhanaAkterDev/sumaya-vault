---
class: cse
title: 02 Why is DNS necessary? State its significance.
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - CN/Ch7
---
# Why is DNS Necessary? State its Significance

The **Domain Name System (DNS)** is necessary because it acts as the backbone of the internet’s addressing system. Computers use IP addresses to locate each other, but humans cannot practically memorize or use those numeric values. DNS solves this by converting domain names into IP addresses and offering additional services like scalability, security, and reliability. Its significance is that without DNS, the internet would be complex, inefficient, and inaccessible for general users.

---

## Significance of DNS

1. **Simplifies Internet Usage**  
    DNS makes the internet accessible by allowing users to type domain names instead of long numeric IP addresses. Without DNS, every user would need to remember numbers like _142.250.190.14_ to visit Google, which is not practical. By handling the translation in the background, DNS ensures smooth user experience.
    
2. **Ensures Global Accessibility**  
    DNS provides a uniform system of addressing across the globe. A domain name like _[www.amazon.com](http://www.amazon.com)_ resolves to the same resource worldwide, regardless of where the user is located. This global standardization ensures consistency and universal access to online services.
    
3. **Supports Scalability of the Internet**  
    The internet is expanding rapidly with billions of websites and connected devices. DNS is designed as a distributed, hierarchical system that can handle this growth without central overload. Its structure of root servers, TLD servers, and authoritative servers ensures that queries are managed efficiently.
    
4. **Provides Reliability and Availability**  
    DNS operates with multiple redundant servers across the world. Even if one server fails, queries are redirected to others. This ensures that users can access websites and services without interruption, making DNS a highly reliable system.
    
5. **Facilitates Load Balancing**  
    DNS can map a single domain name to multiple IP addresses, distributing traffic among different servers. For instance, a global website like YouTube directs users to servers closest to their location. This not only balances load but also improves speed, reduces latency, and prevents system crashes during peak demand.
    
6. **Enables Proper Email Delivery**  
    DNS supports email communication through Mail Exchange (MX) records. These records tell mail servers where to deliver emails for a specific domain. Without DNS, sending an email to someone at _@example.com_ would not be possible, as the mail system would not know the correct destination server.
    
7. **Enhances Security**  
    DNS Security Extensions (DNSSEC) add cryptographic protection to prevent attacks like DNS spoofing or cache poisoning, where malicious actors try to redirect users to fake sites. By verifying the authenticity of DNS responses, DNS ensures safe and trustworthy communication over the internet.
    
8. **Supports Multiple Internet Services**  
    Beyond website browsing, DNS underpins many other services such as cloud computing, online gaming, VoIP calls, and file transfers. These applications depend on DNS to locate the correct servers, making it a crucial part of modern internet infrastructure.