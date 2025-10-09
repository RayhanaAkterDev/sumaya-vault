---
class: cse
title: 05 What is DOM? Describe it.
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2022
---
# DOM (Document Object Model)

The **Document Object Model (DOM)** is a **programming interface** for HTML and XML documents. It represents the document as a structured tree of objects, allowing programs and scripts to dynamically access, modify, or manipulate the content, structure, and style of web pages. Essentially, the DOM acts as a bridge between web documents and programming languages like JavaScript, enabling interactive and dynamic web applications.

---

## Description of DOM

1. **Tree Structure Representation** – The DOM represents the document as a hierarchical tree of nodes. Each element, attribute, and piece of text in the HTML or XML document is represented as a node in this tree. This structure makes it easy to navigate, search, and modify elements programmatically.
    
2. **Types of Nodes** – DOM nodes can be of various types: element nodes (e.g., `<div>`, `<p>`), attribute nodes (e.g., `id`, `class`), text nodes (content inside elements), and others such as comment nodes or document nodes.
    
3. **Dynamic Interaction** – Using the DOM, scripts can dynamically change the content, structure, and styling of web pages. For example, JavaScript can add, delete, or modify elements in response to user actions without reloading the page.
    
4. **Cross-Language Support** – The DOM is platform- and language-independent. While commonly accessed via JavaScript in web browsers, other programming languages like Python or Java can also manipulate XML documents through the DOM API.
    
5. **Event Handling** – The DOM provides mechanisms to handle events such as clicks, mouse movements, or keypresses. Scripts can attach event listeners to nodes, making web pages interactive and responsive to user actions.

---

### Example

Suppose an HTML page has a paragraph:

```html
<p id="demo">Hello World!</p>
```

Using the DOM in JavaScript, you can change its content dynamically:

```js
document.getElementById("demo").innerHTML = "Hello Sumaya!";
```

Here, the paragraph node is accessed via the DOM, and its text is updated without reloading the page.