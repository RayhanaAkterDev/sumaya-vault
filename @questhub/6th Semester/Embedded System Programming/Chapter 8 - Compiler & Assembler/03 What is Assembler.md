---
class: cse
title: 03 What is Assembler?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2020
  - board_2021
  - board_2022
---
# Assembler

An **assembler** is a software tool that converts a program written in **assembly language**, which uses human-readable mnemonics like `MOV` or `ADD`, into **machine code** that a computer can execute directly. It translates symbolic instructions into binary instructions understandable by the CPU and generates a **symbol table** for labels and variables. Assemblers may also produce listing files that show both the assembly code and corresponding machine code, which helps in debugging. There are **single-pass** and **multi-pass** assemblers, depending on whether they translate the code in one or multiple passes. Overall, an assembler serves as a crucial link between human-readable programs and the low-level instructions a computer can execute, making it essential for low-level programming and system development.