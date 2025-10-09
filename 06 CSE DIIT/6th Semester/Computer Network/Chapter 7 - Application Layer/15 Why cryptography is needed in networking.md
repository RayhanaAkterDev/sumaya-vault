---
class: cse
title: 15 Why cryptography is needed in networking?
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
# Why Cryptography is Needed in Networking

Cryptography is essential in networking because it provides the tools and techniques to secure data transmitted across networks. As data travels over public or shared networks, it is vulnerable to interception, tampering, and unauthorized access. Cryptography ensures that information remains **confidential, authentic, and unaltered**, protecting both users and systems from malicious activities.

---

## Reasons for Needing Cryptography in Networking

1. **Confidentiality**  
    Cryptography ensures that sensitive information, such as passwords, credit card numbers, or personal messages, remains unreadable to unauthorized users. Without encryption, attackers can easily intercept and misuse data.
    
2. **Data Integrity**  
    Cryptography allows detection of any modifications to data during transmission. Techniques like message authentication codes (MAC) or digital signatures ensure that the data received is exactly what was sent.
    
3. **Authentication**  
    It verifies the identities of the communicating parties. Public key cryptography, digital certificates, and signatures help confirm that the sender is genuine and prevent impersonation attacks.
    
4. **Non-Repudiation**  
    Cryptography prevents senders from denying their actions. For example, digital signatures in emails or transactions ensure that the sender cannot later claim they did not send the message.
    
5. **Secure Key Exchange**  
    Cryptography enables safe exchange of secret keys over unsecured networks. Public key methods allow two parties to establish a shared secret key without exposing it to attackers.
    
6. **Protection Against Attacks**  
    Cryptography helps defend against eavesdropping, man-in-the-middle attacks, replay attacks, and other network threats, maintaining trust in network communication.
    
7. **Confidentiality of Routing Information**  
    Cryptography protects sensitive routing data in networks, preventing attackers from learning network topology or intercepting path information.
    
8. **Support for Virtual Private Networks (VPNs)**  
    Cryptography enables VPNs, allowing secure communication over public networks by encrypting all transmitted data and maintaining privacy.