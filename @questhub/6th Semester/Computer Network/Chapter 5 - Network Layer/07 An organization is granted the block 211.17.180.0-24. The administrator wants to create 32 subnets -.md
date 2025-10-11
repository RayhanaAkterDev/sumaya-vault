---
class: cse
title: 07 An organization is granted the block 211.17.180.0/24. The administrator wants to create 32 subnets -
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-08
status: pending 🛑
tags:
  - board_2019
---

An organization is granted the block 211.17.180.0/24. The administrator wants to create 32 subnets - 

- Find the subnet mask.
- Find the number of addresses in each subnet.
- Find the first and last addresses in subnet 1.
- Find the first and last addresses in subnet 32.

---

Given:

- Network: `211.17.180.0/24`    
- Required subnets: 32    

### 1. Find the subnet mask

**Number of bits needed for 32 subnets:**  

![[Pasted image 20250909071641.png]]

Add these bits to the original network prefix (/24).
`24+5=29`

✅ **Subnet mask:** `/29` or in decimal `255.255.255.248`

---

### 2. Number of addresses in each subnet
Number of addresses = ![[Pasted image 20250909072032.png]]

Usable addresses: `8 − 2 = 6`

---

### 3. Find the first and last addresses of subnet 1

- First address in subnet 1 is `211.17.180.0`
- Last address in subnet 1 is `211.17.180.7`
  - ---
- First usable address: `211.17.180.1`    
- Last usable address: `211.17.180.6`

---

### 4. Find the first and last addresses of subnet 32

**Step 1:** Calculate the starting address of subnet 32:

![[Pasted image 20250909073425.png]]

- First address in subnet 32 is `211.17.180.248`
- Last address in subnet 32 is `211.17.180.255`
  - ---
- First usable address: `211.17.180.249`    
- Last usable address: `211.17.180.254`

---