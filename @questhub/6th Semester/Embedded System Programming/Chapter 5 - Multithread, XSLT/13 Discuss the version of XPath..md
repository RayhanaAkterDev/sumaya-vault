---
class: cse
title:
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - ESP/Ch5
---
## Versions of XPath

**XPath** has evolved over time, with different versions providing enhanced features and capabilities for navigating and querying XML documents.

1. **XPath 1.0** – Released in 1999, XPath 1.0 is the first version and the most widely supported. It provides basic features for navigating XML nodes, selecting elements and attributes, applying filters, and simple functions for strings, numbers, and boolean values. Most XSLT 1.0 processors and XML parsers support XPath 1.0.
    
2. **XPath 2.0** – Introduced in 2007, XPath 2.0 added significant improvements, including support for sequences, richer data types (like date, time, and duration), enhanced functions, and more powerful conditional expressions. It allows more complex queries and is used with XSLT 2.0 processors.
    
3. **XPath 3.0 and 3.1** – XPath 3.0 and 3.1, released later, further extend the language by supporting **higher-order functions, maps, arrays, and advanced expressions** for more flexible XML processing. These versions are used in modern XSLT 3.0 processors and provide improved capabilities for working with large and complex XML documents.

---

**Example:**

Suppose an XML document contains employee data. Using XPath 1.0, you can select all employee names:

```xpath
/employees/employee/name
```

Using XPath 2.0 or 3.0, you could select employees with a salary greater than 5000 and order them by department using more advanced expressions.