---
class: cse
title: 07 Explain Interrupt Handler.
course:
  - Embedded System Programming
chapter:
  - "ch7: XML"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2022
---
# Interrupt Handler

An **Interrupt Handler** (also known as an **Interrupt Service Routine – ISR**) is a special routine executed by the CPU in response to an interrupt signal. It allows the system to respond quickly to external or internal events (like I/O operations, hardware requests, or software-generated interrupts) without losing the flow of the main program. The primary goal of an interrupt handler is to service the request efficiently and then return control back to the interrupted task.

### Working Process of an Interrupt Handler

1. **Interrupt Signal**  
    The process starts when a hardware device (like a keyboard, timer, or disk controller) or a software process generates an interrupt request. These signals are often managed by the **Programmable Interrupt Controller (PIC)**, which prioritizes multiple requests and forwards the appropriate one to the CPU.
    
2. **Suspension of Current Task**  
    Once the CPU acknowledges the interrupt, it pauses the execution of the currently running instruction sequence. The CPU must suspend this task immediately so that the interrupt can be addressed on time, especially in the case of real-time or critical events.
    
3. **Context Saving**  
    To avoid losing progress, the CPU saves the current **context** of the interrupted task onto the system stack. This includes the **Program Counter (PC)**, CPU registers, and status flags. Saving this state ensures that after the interrupt is serviced, the program can resume from the exact point where it was paused.
    
4. **Locating the Handler**  
    The CPU identifies which interrupt handler should run by consulting the **Interrupt Vector Table (IVT)**. This table contains the starting memory addresses of all handlers, and each interrupt request is associated with a unique vector pointing to the correct routine.
    
5. **Handler Execution**  
    After locating the correct address, the CPU jumps to the handler and begins executing it. The handler performs the required actions, such as reading data from an input device, acknowledging the interrupt request, handling an error condition, or updating a system variable. Handlers are designed to be efficient so that they finish quickly and do not delay other processes.
    
6. **Context Restoration**  
    Once the interrupt has been serviced, the CPU restores the previously saved context from the stack. The program counter and registers are reloaded so that the interrupted task has the same state as before the interrupt occurred.
    
7. **Resumption of Task**  
    Finally, the CPU resumes the execution of the interrupted program from the exact point it left off. To the user or running application, this switch is seamless, and it appears as if the task was never interrupted.

### Example

When a **keyboard key is pressed**, the controller sends an interrupt to the CPU. The CPU pauses the current task, saves its state, and executes the keyboard handler, which reads and stores the key code. After that, the CPU restores the saved state and resumes the interrupted program.