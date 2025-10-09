---
class: cse
title: 01 What is the purpose of Domain Name System (DNS)?
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2019
---
### Purpose of Domain Name System (DNS)

The **Domain Name System (DNS)** is a hierarchical and distributed naming system that translates human-readable domain names into machine-readable IP addresses. Since humans prefer easy-to-remember names like _www.google.com_ instead of complex numeric IP addresses (e.g., _142.250.190.14_), DNS plays a vital role in making internet communication simple and efficient.

---
## Main Purposes of DNS

1. **Name-to-IP Address Translation**  
    DNS translates domain names into IP addresses so that devices can locate and communicate with each other on the network. For example, when a user types _www.google.com_, DNS resolves it to an IP like _142.250.190.14_.
    
2. **Simplifying User Experience**  
    DNS allows people to use readable names instead of long numeric IP addresses. This makes the internet easier to use, since remembering _facebook.com_ is far simpler than memorizing _157.240.22.35_.
    
3. **Distributed and Hierarchical System**  
    DNS operates as a global, distributed database arranged in a hierarchy of root servers, top-level domain servers, and authoritative servers. This structure ensures reliability, scalability, and efficient resolution even with billions of daily queries.
    
4. **Load Balancing and Reliability**  
    DNS can map one domain to multiple IP addresses and redirect users to the closest or least busy server. This balances traffic, prevents overload, and keeps services available even during heavy usage.
    
5. **Email Routing through MX Records**  
    DNS uses Mail Exchange (MX) records to direct emails to the correct mail servers. Without DNS, an email sent to _@example.com_ would not know where to be delivered.
    
6. **Domain Aliasing with CNAME Records**  
    DNS supports aliases, meaning one domain can point to another domain name. This helps organizations manage multiple services easily. For example, _blog.company.com_ may be linked to _company.wordpress.com_.
    
7. **Security through DNSSEC**  
    DNS can be extended with DNS Security Extensions (DNSSEC) to protect against threats like spoofing and cache poisoning. It ensures that the response received is authentic and has not been tampered with.
    
8. **Support for Other Internet Services**  
    DNS is not limited to web browsing. It also supports services like VoIP, cloud applications, FTP, and online gaming by resolving service-specific addresses to the correct servers.