---
class: cse
title: 03 Classify different classes of IP address with its range and also specify the list of all private IP address.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-08
status: pending 🛑
tags:
  - board_2018
  - board_2021
---

# Classification of IP Addresses

### IPv4 Address Classes

|**Class**|**Range**|**Leading Bits**|**Default Subnet Mask**|**No. of Networks**|**No. of Hosts per Network**|**Usage**|
|---|---|---|---|---|---|---|
|**A**|`1.0.0.0 – 126.255.255.255`|`0`|`255.0.0.0`|128|~16 million|Very large networks|
|**B**|`128.0.0.0 – 191.255.255.255`|`10`|`255.255.0.0`|16,384|~65,000|Medium-sized networks|
|**C**|`192.0.0.0 – 223.255.255.255`|`110`|`255.255.255.0`|~2 million|254|Small networks (homes/offices)|
|**D**|`224.0.0.0 – 239.255.255.255`|`1110`|Not defined|N/A|N/A|Multicast communication|
|**E**|`240.0.0.0 – 255.255.255.255`|`1111`|Not defined|N/A|N/A|Experimental / Research|

---

### Private IP Address Ranges

|**Class**|**Private IP Range**|
|---|---|
|**A**|`10.0.0.0 – 10.255.255.255`|
|**B**|`172.16.0.0 – 172.31.255.255`|
|**C**|`192.168.0.0 – 192.168.255.255`|