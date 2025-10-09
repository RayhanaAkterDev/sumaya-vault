---
class: cse
title: 05 Write down the features of machine dependent assembler.
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2021
---
### Features of a Machine-Dependent Assembler

A **machine-dependent assembler** is designed to work specifically for a particular type of computer or processor. Its features reflect this close relationship with the hardware and its instruction set.

1. **Hardware Specific:** It generates machine code that can only be executed on a specific processor or family of processors. Instructions and memory addressing are tailored to the target machine’s architecture.
    
2. **Instruction Set Dependent:** The assembler supports only the mnemonics and instructions defined by the processor’s instruction set. It cannot understand or translate instructions meant for a different machine.
    
3. **Memory Organization Awareness:** It knows the memory structure, word length, and addressing modes of the target machine, ensuring correct placement of instructions and data in memory.
    
4. **Optimized for the Target Machine:** It can produce code that takes advantage of the specific features of the processor, such as special registers, instruction formats, or hardware capabilities, for faster and more efficient execution.
    
5. **Limited Portability:** Programs assembled by a machine-dependent assembler are not portable. The same assembly code may not run on a different processor without modification.
    
6. **Direct Handling of Hardware Features:** It can manage input/output operations, interrupts, and other hardware-specific functions, which are unique to the target machine.
    
7. **Error Reporting Specific to Machine:** It detects errors based on the constraints of the target machine, such as invalid instructions, addressing errors, or memory overflow according to the hardware limits.

**Example:** An assembler designed for an Intel 8086 microprocessor will generate 16-bit machine code instructions suitable only for that processor. The same code cannot run directly on an ARM processor without modification.