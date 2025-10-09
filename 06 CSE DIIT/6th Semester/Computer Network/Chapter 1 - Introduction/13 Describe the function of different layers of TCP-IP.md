---
class: cse
title: 13 Describe the function of different layers of TCP/IP
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2022
  - CN/Ch1/board_2020
---

## ❖ **Functions of Different Layers of the TCP/IP Model**

The **TCP/IP model** consists of **four layers**, each having a specific role in enabling communication over the internet. These layers work together to ensure that data is successfully sent and received between devices.

---

### 1. **Application Layer**

The **Application Layer** is the **topmost layer** of the TCP/IP model. It provides direct services to the **end-users or application software**. This layer handles protocols that support user activities such as file transfers, web browsing, remote access, and email. Common protocols include:

- **HTTP** (for web pages),
    
- **FTP** (for file transfers),
    
- **SMTP** (for email),
    
- **DNS** (for domain name resolution), and
    
- **TELNET** (for remote login).  
    It ensures that the application on the sender’s side can effectively communicate with the application on the receiver’s side.
    

---

### 2. **Transport Layer**

The **Transport Layer** ensures **end-to-end communication and reliable data transfer** between two devices. It manages data segmentation, flow control, and error correction. Two main protocols operate at this layer:

- **TCP (Transmission Control Protocol)**: Provides reliable, connection-oriented communication.
    
- **UDP (User Datagram Protocol)**: Provides faster, connectionless communication without reliability.  
    This layer also ensures correct data sequencing and retransmits lost or damaged segments.
    

---

### 3. **Internet Layer**

The **Internet Layer** is responsible for **routing the data packets** from the source to the destination across multiple networks. It handles **logical addressing** using IP addresses and determines the best possible route for data delivery. The main protocol used here is:

- **IP (Internet Protocol)** – responsible for addressing and routing.  
    Other supporting protocols include:
    
- **ICMP (Internet Control Message Protocol)** – used for error messages and diagnostics,
    
- **ARP (Address Resolution Protocol)** – maps IP addresses to MAC addresses.
    

---

### 4. **Network Access Layer (or Link Layer)**

The **Network Access Layer** handles all functions related to the **physical transmission** of data over the network. It defines how bits are **physically sent** through the network medium (e.g., cables, Wi-Fi). It includes two main components:

- **Data Link Layer** – manages framing, physical addressing (MAC), and error detection.
    
- **Physical Layer** – handles actual bit-level transmission over the hardware.  
    This layer ensures that the data is correctly formatted for the specific network technology being used (e.g., Ethernet, Wi-Fi).


---


> See the exam paper answer - page 160

The **TCP/IP model** (Transmission Control Protocol/Internet Protocol) is a foundational framework for how data is transmitted across the internet. It consists of **four layers**, each with a specific function that contributes to successful data communication between devices.

---

### 1. **Application Layer**

**Definition:**  
The Application Layer is the topmost layer of the TCP/IP model. It provides a direct interface between user applications and the network. This layer is responsible for delivering services such as web browsing, file transfers, and email by using various application-level protocols.

**Key Functions:**

- Provides services like HTTP, FTP, SMTP, DNS, and DHCP.    
- Facilitates communication between software applications and lower network layers.    
- Handles data formatting, user authentication, and session control.    
- Manages data encryption and compression where needed.    

---

### 2. **Transport Layer**

**Definition:**  
The Transport Layer ensures reliable or best-effort communication between devices. It establishes end-to-end connections, manages data delivery, and ensures that data is delivered accurately and in the correct sequence.

**Key Functions:**

- Uses TCP for reliable communication and UDP for faster, connectionless communication.    
- Breaks large messages into smaller segments and reassembles them at the destination.    
- Performs error detection, correction, and retransmission (TCP).    
- Uses port numbers to identify sending and receiving applications.    
- Controls data flow to prevent congestion or packet loss.    

---

### 3. **Internet Layer**

**Definition:**  
The Internet Layer is responsible for logical addressing and routing of data packets across multiple networks. It ensures that each packet reaches its correct destination, even if it has to pass through several intermediate routers.

**Key Functions:**

- Assigns IP addresses and ensures proper identification of devices.    
- Determines the best path for data transmission using routing protocols.    
- Handles packet fragmentation and reassembly for compatibility across networks.    
- Uses protocols such as IP, ICMP (for error reporting), and ARP (for address resolution).    
- Enables internetworking by connecting multiple networks together.    

---

### 4. **Network Access Layer (Link Layer)**

**Definition:**  
The Network Access Layer is the lowest layer in the TCP/IP model. It manages the physical transmission of data over the network medium. This includes both the hardware (like cables and network interface cards) and the software protocols that control access to the medium.

**Key Functions:**

- Encapsulates data into frames for transmission.    
- Uses MAC addresses to identify devices on the local network.    
- Handles access control to shared communication channels.    
- Performs error detection using techniques like checksums.    
- Supports transmission technologies such as Ethernet and Wi-Fi.
