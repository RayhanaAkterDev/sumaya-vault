---
class: cse
title: 13 Write the electronic mail message format.
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
# Electronic Mail (Email) Message Format

An **electronic mail message** is structured in a standard format to ensure proper delivery, readability, and interpretation by email systems. It generally consists of **two main sections**: the **header** and the **body**.

---

## 1. Header

The header contains information needed for routing, identification, and processing of the email. Common fields include:

1. **From:** The sender’s email address.    
2. **To:** The recipient’s email address.    
3. **Cc (Carbon Copy):** Email addresses of secondary recipients who will receive a copy.
4. **Bcc (Blind Carbon Copy):** Email addresses of recipients hidden from others.    
5. **Date:** The date and time when the email was sent.    
6. **Subject:** A brief summary of the email content.    
7. **Message-ID:** A unique identifier assigned to the email.    
8. **Reply-To:** Address where replies should be sent (optional).  

---

## 2. Body

The body contains the actual message intended for the recipient. It may include:

1. **Text content:** The main written message.    
2. **Attachments:** Files, images, or documents sent along with the email.    
3. **Formatting:** Optional formatting like fonts, colors, or HTML content.

---

## 3. Example of Email Message

```vbnet
From: alice@example.com
To: bob@example.com
Cc: charlie@example.com
Bcc: manager@example.com
Date: 11 Sep 2025, 10:30 AM
Subject: Meeting Schedule
Message-ID: <12345@example.com>
Reply-To: alice@example.com

Dear Bob,

Please find attached the schedule for tomorrow's project meeting. Let me know if you have any conflicts.

Regards,
Alice
```