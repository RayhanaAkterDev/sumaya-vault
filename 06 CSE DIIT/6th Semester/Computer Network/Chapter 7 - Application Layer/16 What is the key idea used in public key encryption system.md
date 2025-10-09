---
class: cse
title: 16 What is the key idea used in public key encryption system?
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
# Key Idea of Public Key Encryption System

The key idea of a **public key encryption system** (also called asymmetric encryption) is the use of **two mathematically related keys**: a **public key** for encryption and a **private key** for decryption. The public key can be freely shared, allowing anyone to encrypt a message, but only the holder of the private key can decrypt it. This eliminates the need to securely share a secret key, which is required in symmetric (secret key) encryption.

---

## How It Works

1. Each user generates a **key pair**: one public and one private key.    
2. The sender uses the recipient’s **public key** to encrypt the message.    
3. The recipient uses their **private key** to decrypt the ciphertext and recover the original message.    
4. Even if someone intercepts the encrypted message, it cannot be decrypted without the private key.

---

**Example:**

- Alice wants to send a confidential message to Bob. She encrypts it using **Bob’s public key**.
- Only **Bob’s private key** can decrypt the message, ensuring that no one else, even if they know the public key, can read it.