---
class: cse
title: 17 What is the difference between unicast, multicast and broadcast address
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_NA
---

|**Aspect**|**Unicast Address**|**Multicast Address**|**Broadcast Address**|
|---|---|---|---|
|**Purpose**|Identifies a single unique device|Identifies a group of devices interested in receiving data|Targets all devices on a local network segment|
|**Communication**|One-to-one|One-to-many|One-to-all|
|**Delivery**|Packet sent to one specific recipient only|Packet sent to all members of a multicast group|Packet sent to every device in the broadcast domain|
|**IP Range (IPv4)**|Any valid individual IP address|224.0.0.0 to 239.255.255.255|Network address with all host bits set (e.g., 192.168.1.255 for subnet 192.168.1.0/24)|
|**Example**|192.168.1.10|224.0.0.1 (all routers on subnet)|192.168.1.255|

---

|**Feature**|**Unicast**|**Multicast**|**Broadcast**|
|---|---|---|---|
|**Communication Type**|One-to-One|One-to-Many (to a specific group)|One-to-All (within a network/subnet)|
|**Target**|Single specific host|Multiple selected hosts in a group|All hosts on the local network|
|**IP Address Range**|Any valid host IP (e.g., `192.168.1.10`)|`224.0.0.0` to `239.255.255.255` (Class D)|Last address in the subnet (e.g., `192.168.1.255`)|
|**Used In**|Personal communication, file transfers|Live streaming, IPTV, video conferencing|ARP, DHCP Discover, general announcements|
|**Efficiency**|Most efficient for single recipient|Efficient for group communication|Least efficient; can cause network overload|
|**Router Behavior**|Forwarded normally|Forwarded only if routers support multicast|Not forwarded beyond local network (default)|
|**Example Protocols**|HTTP, FTP, SSH|IGMP, RTP, PIM|ARP, DHCP, NetBIOS|