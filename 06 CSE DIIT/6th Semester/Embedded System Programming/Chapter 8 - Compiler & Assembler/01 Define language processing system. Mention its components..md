---
class: cse
title: 01 Define language processing system? Mention its components.
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2020
---
### Language Processing System

A **Language Processing System (LPS)** is a system designed to process, understand, and manipulate human or programming languages. In computing, it usually refers to systems that analyze and translate programming languages (like compilers and interpreters), while in natural language processing, it deals with human languages. The main goal is to convert source language input into a meaningful output, either as machine-executable code or as interpreted information.

### Components of a Language Processing System

1. **Lexical Analyzer (Scanner):** It reads the source code and breaks it into tokens, which are meaningful units like keywords, identifiers, operators, and constants. It also removes unnecessary spaces and comments. The lexical analyzer detects errors such as invalid symbols and simplifies the processing for the next phase.
    
2. **Syntax Analyzer (Parser):** It examines the arrangement of tokens according to the rules of the language grammar. The parser constructs a parse tree or syntax tree representing the program’s structure and identifies syntax errors when token sequences do not conform to the grammar.
    
3. **Semantic Analyzer:** This component ensures the program’s statements are meaningful. It performs tasks like type checking, scope resolution, and verifying operations are semantically correct. Semantic errors, such as assigning a string to an integer variable, are detected here.
    
4. **Intermediate Code Generator:** It converts the syntax tree into an intermediate representation, which is independent of the target machine. This representation makes further optimization easier and provides a bridge between high-level code and machine code.
    
5. **Code Optimizer:** It improves the intermediate code to make it more efficient. Optimization may reduce execution time, minimize memory usage, or remove redundant instructions without changing the program’s output.
    
6. **Code Generator:** It translates the optimized intermediate code into target machine code. It handles memory allocation, register assignment, and selects appropriate machine instructions, producing an executable program.
    
7. **Symbol Table:** A data structure that stores information about identifiers, including names, types, scope, and memory locations. It is accessed throughout the compilation process to maintain consistency and support semantic analysis.
    
8. **Error Handler:** Responsible for detecting, reporting, and recovering from errors during different phases of processing. It provides meaningful messages to help the programmer identify and correct issues.