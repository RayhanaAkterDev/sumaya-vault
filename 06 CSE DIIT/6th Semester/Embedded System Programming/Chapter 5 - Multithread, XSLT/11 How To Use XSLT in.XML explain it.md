---
class: cse
title: 11 How To Use XSLT in.XML? Explain it
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - ESP/Ch5
---
## How to Use XSLT in XML

**XSLT (Extensible Stylesheet Language Transformations)** is used to transform XML data into other formats such as HTML, plain text, or another XML structure. To use XSLT with an XML file, you need to **link the XML file to an XSLT stylesheet**, which contains rules and templates defining how the XML data should be transformed. The browser or an XSLT processor then reads both files and applies the transformations to produce the output.

### Steps to Use XSLT in XML

1. **Create an XML Document** – Prepare an XML file containing the structured data you want to display or transform.
    
2. **Create an XSLT Stylesheet** – Write an XSLT file with templates, matching patterns, and instructions for transforming XML elements into the desired output format (like HTML).
    
3. **Link the XSLT to the XML** – Include a reference to the XSLT file in the XML document using the `<?xml-stylesheet?>` processing instruction:

```xml
<?xml-stylesheet type="text/xsl" href="style.xsl"?>
```

4. **Apply the Transformation** – Open the XML file in a web browser or use an XSLT processor. The processor reads the XML data, applies the rules from the XSLT stylesheet, and generates the output.
    
5. **View the Result** – The output can be displayed in a browser as HTML, exported as plain text, or written into another XML file depending on the instructions in the XSLT.

---

### Example

Suppose you have an XML file `books.xml` with a list of books:

```xml
<?xml version="1.0"?>
<?xml-stylesheet type="text/xsl" href="books.xsl"?>
<books>
  <book>
    <title>Programming Basics</title>
    <author>Sumaya</author>
  </book>
  <book>
    <title>Embedded Systems</title>
    <author>Rahman</author>
  </book>
</books>
```

The XSLT file `books.xsl` contains templates to transform this XML into an HTML table. When opened in a browser, the XML data is displayed as a formatted table without modifying the original XML file.