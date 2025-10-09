---
class: cse
title: 02 What is the difference between single & multi-pass compiler?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2021
  - board_2022
---
### Difference Between Single-Pass and Multi-Pass Compiler

| Feature                   | Single-Pass Compiler                                                                  | Multi-Pass Compiler                                                                                |
| ------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Definition**            | Processes the entire source code in a single pass, scanning each statement only once. | Processes the source code in multiple passes, scanning the code several times for different tasks. |
| **Processing Time**       | Faster since the code is read only once.                                              | Slower because the code is scanned multiple times.                                                 |
| **Memory Requirement**    | Requires less memory as it stores minimal intermediate information.                   | Requires more memory to store intermediate representations between passes.                         |
| **Error Detection**       | Detects fewer errors; some errors may not be found until later stages.                | Can detect more errors at different stages since each pass focuses on specific tasks.              |
| **Code Optimization**     | Limited optimization opportunities due to single pass.                                | Better optimization possible because multiple passes allow more thorough analysis.                 |
| **Complexity**            | Simpler to implement.                                                                 | More complex to implement due to multiple passes and data handling between passes.                 |
| **Use Case**              | Suitable for simple or small programming languages.                                   | Suitable for complex or large programming languages.                                               |
| **Symbol Table Handling** | Often limited; symbols may need to be reprocessed for forward references.             | Efficient; symbols and other intermediate data can be fully resolved across passes.                |
| **Error Recovery**        | Difficult; once an error is detected, the compiler may not continue smoothly.         | Easier; errors in one pass can be fixed or reported without affecting other passes.                |