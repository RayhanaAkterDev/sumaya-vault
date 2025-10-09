---
class: cse
title: 11 What is Machine Dependent Loader?
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch9
---
### Machine Dependent Loader

A **machine dependent loader** is a program that loads an object file into main memory for execution, where its design and operation depend on the specific architecture of the target machine. It works closely with the machine’s instruction formats, addressing modes, and memory organization to perform relocation, linking, and address resolution. Since it directly understands and uses hardware-specific details, it is fast and efficient, but it lacks portability and cannot be used on a different architecture without major modifications. 

For example, a loader designed for Intel x86 processors can correctly load and execute x86 instructions but would not work on an ARM-based system due to differences in instruction sets and addressing schemes.