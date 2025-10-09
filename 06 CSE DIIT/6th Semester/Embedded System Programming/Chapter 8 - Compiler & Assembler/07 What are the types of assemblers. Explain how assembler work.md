---
class: cse
title: 07 What are the types of assemblers? Explain how assembler work?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Types of Assemblers and How an Assembler Works

An **assembler** is a program that converts assembly language into machine code. Based on design and functionality, assemblers are categorized into different types. They also follow a systematic process to translate symbolic instructions into executable machine code.

---

### **Types of Assemblers**

1. **Single-Pass Assembler:**  
    This type of assembler scans the source program **only once** to translate instructions into machine code. It is fast and simple but cannot easily handle **forward references** (labels used before being defined). Suitable for small programs with minimal complexity.
    
2. **Multi-Pass Assembler:**  
    A multi-pass assembler scans the source program **multiple times**. The first pass generally builds the **symbol table** and resolves addresses, while the subsequent passes generate the machine code. It can handle **forward references**, large programs, and allows **code optimization** but is slower and more memory-intensive.
    
3. **Cross Assembler:**  
    A cross assembler runs on **one type of computer** but produces machine code for a **different type of processor**. This is useful for developing programs for embedded systems or microcontrollers.
    
4. **Macro Assembler:**  
    This assembler supports **macros**, which are sequences of instructions that can be reused multiple times. Macros reduce repetitive coding and simplify program structure.
    

---

### **How an Assembler Works**

1. **Reading the Source Program:**  
    The assembler begins by reading the assembly language program line by line, identifying **mnemonics, operands, labels, and directives**. This step ensures that all instructions and symbols are recognized correctly.
    
2. **Translation of Instructions:**  
    Each mnemonic instruction is translated into **binary machine code** that the CPU can execute. The assembler uses an internal table that maps assembly mnemonics to their corresponding opcodes.
    
3. **Symbol Table Creation:**  
    The assembler maintains a **symbol table** containing all labels, variables, and constants with their memory addresses. This is crucial for handling references, especially forward references where a label is used before being defined.
    
4. **Address Assignment:**  
    Memory locations are assigned to every instruction and data element according to the program’s structure. This ensures that the CPU can correctly locate and execute instructions in sequence.
    
5. **Processing Directives:**  
    Assembler directives, also called pseudo-instructions, are interpreted to manage the assembly process. Examples include reserving memory space (`RESB`), defining constants (`DB`), or including additional files. These directives guide the assembler but do not generate machine code themselves.
    
6. **Error Detection:**  
    During assembly, the assembler checks for **syntax errors, invalid instructions, undefined labels, and memory allocation issues**, reporting them to the programmer for correction.
    
7. **Generating Output:**  
    After translation, the assembler produces **object code or machine code**, which can be loaded and executed by the CPU. Many assemblers also produce a **listing file** that shows both the assembly instructions and their corresponding machine code, helping in debugging and verification.
    

**Example:** For an instruction like `MOV A, 5`, the assembler translates it into binary machine code, assigns it a memory address, updates the symbol table, and includes it in the listing file, making the program ready for execution.