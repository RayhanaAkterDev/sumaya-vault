---
class: cse
title: 10 Describe the method of cryptography process.
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
tags:
  - board_2019
  - board_2020
  - board_2022
importance: ⭐⭐⭐
---
# Method of Cryptography Process

**Cryptography process** refers to the set of steps through which information is transformed into a secure form for transmission or storage and then converted back into its original form when needed. The main goal is to ensure **confidentiality, integrity, authentication, and non-repudiation** of data.

---

## Steps in the Cryptography Process

1. **Plaintext (Original Message)**  
    Plaintext is the original readable data that requires protection. It may include personal messages, login credentials, or financial information. If plaintext is transmitted directly, it can easily be intercepted and misused by attackers.
    
2. **Encryption**  
    Encryption is the process of applying an algorithm along with a key to transform plaintext into an unreadable form. This step hides the true meaning of the data and ensures that only authorized parties who possess the correct key can recover the information.
    
3. **Ciphertext (Encoded Message)**  
    Ciphertext is the encrypted version of the plaintext. It appears as a meaningless or random sequence of characters. Even if someone intercepts the ciphertext, it cannot be understood without the correct decryption key.
    
4. **Transmission of Ciphertext**  
    The ciphertext is transmitted over the communication medium, such as the internet or a network channel. Since it is already in encrypted form, it remains secure even if the transmission channel is insecure or exposed to attackers.
    
5. **Decryption**  
    Decryption is the reverse of encryption. At the receiver’s end, the ciphertext is transformed back into readable plaintext using a decryption algorithm and the appropriate key. In symmetric encryption the same key is used for decryption, whereas in asymmetric encryption a private key is used for this purpose.
    
6. **Plaintext Recovery (Original Message)**  
    After decryption, the receiver obtains the original plaintext message. At this stage, the data is readable again, completing the secure communication cycle.