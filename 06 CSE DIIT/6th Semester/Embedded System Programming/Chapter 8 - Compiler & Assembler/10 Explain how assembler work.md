---
class: cse
title: 10 Explain how assembler work
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
## How an Assembler Works

An **assembler** is a program that converts assembly language into machine code that a CPU can execute. The process involves several systematic steps to ensure accurate translation, memory management, and error detection.

1. **Reading the Source Program:**  
    The assembler reads the assembly language program line by line, identifying **mnemonics, operands, labels, and assembler directives**. This ensures that all instructions and symbols are recognized correctly.
    
2. **Lexical Analysis:**  
    Each instruction is broken down into **tokens**—the basic units such as operation codes (mnemonics), registers, constants, and labels. This helps the assembler understand the structure of each instruction.
    
3. **Translation of Instructions:**  
    Mnemonics are translated into **binary machine code** using a lookup table that maps assembly instructions to their corresponding opcodes. For example, `MOV A, 5` might be translated into `10110000 00000101`.
    
4. **Symbol Table Creation:**  
    The assembler maintains a **symbol table** containing all labels, variables, and constants along with their memory addresses. This is essential for resolving **forward and backward references** within the program.
    
5. **Address Assignment:**  
    Memory locations are assigned to every instruction and data element, ensuring that the CPU can correctly locate and execute each instruction in sequence.
    
6. **Handling Directives:**  
    Assembler directives, also called pseudo-instructions, are interpreted to control the assembly process. Examples include reserving memory (`RESB`), defining constants (`DB`), or including files. These directives guide assembly but do not produce machine code themselves.
    
7. **Error Detection:**  
    The assembler checks for **syntax errors, invalid instructions, undefined labels, and memory allocation issues**, reporting them to the programmer for correction before generating machine code.
    
8. **Generating Output:**  
    Finally, the assembler produces the **object code** or **machine code** that can be loaded into memory and executed by the CPU. Many assemblers also create a **listing file**, showing both the assembly instructions and the corresponding machine code for verification and debugging.
    

**Example:**  
For the instruction `MOV A, 5`, the assembler translates it into machine code, assigns it a memory location, updates the symbol table, and includes it in the listing file, making it ready for execution.