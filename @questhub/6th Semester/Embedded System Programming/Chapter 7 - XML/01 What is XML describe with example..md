---
class: cse
title: 01 What is XML? Describe with example.
course:
  - Embedded System Programming
chapter:
  - "ch7: XML"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2022
  - board_2021
---
### XML (Extensible Markup Language)

XML (Extensible Markup Language) is a markup language used to store, transport, and structure data in a readable format for both humans and machines. Unlike HTML, which defines how data is displayed, XML focuses on describing what the data is. XML allows users to create custom tags to represent data meaningfully. It is platform-independent and widely used for data exchange between different systems, such as web services, APIs, and configuration files.

**Key Features of XML:**

- **Extensible:** Users can define their own tags according to the data requirements.    
- **Structured:** Data is organized in a hierarchical tree-like structure with elements and sub-elements.    
- **Self-Descriptive:** Each piece of data is enclosed within descriptive tags.    
- **Platform-Independent:** Can be used across different software and hardware platforms.

---

#### Example of XML

```xml
<?xml version="1.0" encoding="UTF-8"?>
<library>
    <book>
        <title>Introduction to Programming</title>
        <author>John Smith</author>
        <year>2023</year>
        <price>29.99</price>
    </book>
    <book>
        <title>Data Structures</title>
        <author>Jane Doe</author>
        <year>2022</year>
        <price>39.99</price>
    </book>
</library>
```

**Explanation of Example:**

- `<library>` is the root element containing all book records.    
- `<book>` represents an individual book entry.    
- Nested tags like `<title>`, `<author>`, `<year>`, and `<price>` describe specific information about each book.    
- This structure allows easy data exchange, searching, and parsing by programs.