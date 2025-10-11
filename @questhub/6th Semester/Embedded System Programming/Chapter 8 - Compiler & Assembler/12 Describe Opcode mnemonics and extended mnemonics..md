---
class: cse
title: 12 Describe Opcode mnemonics and extended mnemonics.
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Opcode Mnemonics

An **opcode mnemonic** is a symbolic, human-readable representation of a **machine-level operation** that the CPU can perform. Each mnemonic corresponds to a specific opcode (operation code) in machine language, making it easier for programmers to write and understand instructions without dealing with raw binary code. For example, in assembly language, `MOV` is a mnemonic for the machine instruction that moves data from one location to another, and `ADD` represents addition. Opcode mnemonics are **hardware-specific**, meaning they depend on the instruction set of the processor. They form the core of assembly language instructions, specifying the operation to be performed on the operands.

---

### Extended Mnemonics

**Extended mnemonics** are additional symbolic instructions provided by some assemblers to simplify programming and improve readability. They go beyond basic opcode mnemonics and can represent **complex operations, pseudo-instructions, or directives** that the assembler converts into one or more machine-level instructions. Extended mnemonics often help with tasks like memory reservation, initializing constants, or controlling the assembly process. For example, `MVI A, 05H` (move immediate value) or `DS 10` (define storage) are considered extended mnemonics because they represent higher-level operations rather than a single machine instruction.

---

**Example:**

- **Opcode Mnemonic:** `ADD B` → Tells the CPU to add the contents of register `B` to the accumulator.    
- **Extended Mnemonic:** `DB 0AH` → Tells the assembler to allocate a byte of memory with the value `0AH` (10 in decimal).