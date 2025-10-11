 1. _What is embedded system?_ Describe the characteristics of embedded system.
   
  > [!note] **Characteristics of Embedded System**
  >  An **embedded system** is a combination of hardware and software designed to perform a specific task or function within a larger system. It is dedicated, task-specific, and often real-time.
  >  1. **Single-functioned**: An embedded system is designed to do one task or a set of related tasks repeatedly. _Example: A washing machine controller only manages wash cycles._
  >  2. **Tightly constrained**: It operates under strict constraints of **size, power, memory, and performance**. _Example: A digital watch uses minimal memory and battery._
  >  3. **Real-time operation**: Many embedded systems are **real-time systems**, which means they must respond to inputs within a defined time limit. _Example: Airbag system in a car must deploy immediately on crash detection._
  >  4. **Low power consumption**: Designed for **energy efficiency**, especially in portable or battery-operated devices. _Example: Medical wearable devices._
  >  5. **Reliability and stability**: Embedded systems must run for long periods without failure. _Example: Traffic light systems work continuously without crashes._
  >  6. **Minimal or no user interface**: Often, these systems work automatically with little or no human interaction. _Example: Automatic fire alarm systems._
  >  7. **Embedded software is stored in ROM/Flash**: The program (firmware) is permanently stored in non-volatile memory like ROM or flash. _Example: Smart TV firmware._
  >  8. **Application-specific hardware**: Embedded systems often use **custom-designed processors** or microcontrollers for efficient performance. _Example: Microcontrollers in microwave ovens._

2. _Explain IoT in embedded system programming with example._
3. Explain real-time embedded system and explain essential components of embedded system.
### 1. **Real-Time Embedded System**

A **real-time embedded system** is a type of embedded system that responds to inputs or events **within a strict and defined time constraint**. These systems are commonly used in applications where timing is crucial, such as medical devices, robotics, aerospace, and automotive systems.

#### ✅ **Definition:**

> A real-time embedded system is a computing system embedded within a larger device, designed to perform specific tasks and respond to inputs within a guaranteed time frame.

**1. Operating Systems for Embedded Systems:**  

**GPOS (General‑Purpose Operating System):**  
A General‑Purpose Operating System is designed for environments where precise timing is not a primary requirement. Its focus is on providing a rich set of features, user interfaces, and multitasking capabilities rather than guaranteeing strict response times. GPOS is used in applications like personal computing, servers, and mobile devices, where performance and versatility matter more than fixed deadlines. Examples include Windows, Linux, and macOS.

**RTOS (Real‑Time Operating System):**  
A Real‑Time Operating System is designed for environments where tasks must be completed within strict, predictable, and well‑defined deadlines. Its priority is determinism and quick response to external events. RTOS is used in applications where delays can cause serious errors or failures, such as medical equipment, automotive controls, robotics, and aerospace. Examples include FreeRTOS, VxWorks, and QNX.

**Types of Real‑Time Systems:**

**1. Hard Real‑Time System:**  
A hard real‑time system operates under very strict timing constraints. All critical tasks must be completed within a precisely defined deadline. Missing the deadline, even once, is considered a system failure, which can lead to serious consequences, including equipment damage or loss of life. These systems are used in applications where timing is absolutely critical, such as pacemakers, anti‑lock braking systems (ABS), and aircraft control systems.

**2. Soft Real‑Time System:**  
A soft real‑time system operates with less stringent timing constraints compared to hard real‑time systems. In these systems, missing a deadline is undesirable but not catastrophic. The system can tolerate delays, although this may degrade the overall quality of service. Examples include video streaming, online gaming, and video conferencing, where delays affect user experience but do not cause total system failure. 

**2. Essential Components of an Embedded System**

An embedded system is made up of both hardware and software elements. Together, they form a dedicated unit that operates with precision for a specific task.

| **Component**                   | **Explanation**                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Hardware**                 | The hardware includes the microcontroller or microprocessor, supporting circuitry, and external interfaces required for the device to operate. It forms the foundation of any embedded system.                                                                                                                                                                                                                                                                               |
| **2. Software**                 | The software (or firmware) consists of the program or instructions that control the hardware. It is stored in ROM or Flash memory and governs how the system operates.                                                                                                                                                                                                                                                                                                       |
| **3. Processor**                | The processor is the brain of the embedded system. It can be a microcontroller (integration of CPU, RAM, ROM, and peripherals) or a microprocessor (CPU only), responsible for executing instructions.                                                                                                                                                                                                                                                                       |
| **4. Memory**                   | Memory provides storage space for program instructions and data. RAM is used for temporary data storage during execution, while ROM or Flash is used for permanent storage of firmware and application code.                                                                                                                                                                                                                                                                 |
| **5. Input and Output Devices** | These are the interfaces through which an embedded system interacts with the external world. <br><br>**Input devices** (such as sensors, switches, and buttons) collect data or signals from the environment. <br><br>**Output devices** (such as LEDs, displays, motors, and buzzers) present information, alerts, or carry out the required action based on the system’s processing. Together, they enable communication between the embedded system and its surroundings. |
| **8. Power Supply**             | The power supply provides stable and regulated voltage required for the embedded system. It ensures that all hardware components operate reliably.                                                                                                                                                                                                                                                                                                                           |
| **9. Timer/Counters**           | Timers and counters are used for precise timekeeping, delays, or generating periodic events within the embedded system. They are crucial for real‑time and time‑sensitive applications.                                                                                                                                                                                                                                                                                      |

4. Design and write the code for a thief detection system using Arduino uno PIR sensor and buzzer.
## **Question:**

**Design and write the code for a thief detection system using Arduino Uno, PIR sensor, and buzzer.**

## ✅ 1. **Objective:**

To design a basic theft detection system that uses a **PIR motion sensor** to detect movement and activates a **buzzer** as an alarm signal when motion is detected. A **reset button** is optionally included to turn off the buzzer manually.

## ✅ 2. **Required Components:**

- **Arduino Uno** – 1 piece    
- **PIR Motion Sensor (HC-SR501)** – 1 piece    
- **Buzzer (Active)** – 1 piece    
- **Push-button (optional for reset)** – 1 piece    
- **Connecting wires**    
- **Breadboard** (optional, for neat prototyping)    

## ✅ 3. **Circuit Description:**

**Circuit Description:**  
- **PIR Sensor**:    
    - The sensor’s **output pin (OUT)** is connected to Arduino digital pin 7 to send a HIGH signal when motion is detected.
- **Buzzer**:    
    - Connected to **Arduino digital pin 8** to sound an alarm when the sensor triggers.        
- **Reset Button** _(optional)_:    
    - Connected to **Arduino digital pin 6** to stop the alarm manually when pressed.        
- **Power Supply**:    
    - All components powered by the **Arduino’s 5V output** for a stable supply.        
- **Common Ground**:    
    - The PIR sensor, buzzer, and reset button share a **common ground (GND)** with the Arduino for a complete circuit.

## ✅ 4. **Circuit Connections:**

### 🔌 **PIR Sensor (HC-SR501):**

- `VCC` → Arduino `5V`    
- `GND` → Arduino `GND`    
- `OUT` → Arduino **Digital Pin 7**    

### 🔔 **Buzzer:**

- `+ve terminal` → Arduino **Digital Pin 8**    
- `-ve terminal` → Arduino `GND`    

> ⚠️ For high-power buzzers, use a transistor circuit instead of directly connecting to the Arduino.

### 🔘 **Reset Button (Optional):**

- One side → **GND**    
- Other side → Arduino **Digital Pin 6**    

> 🔸 No external resistor is required, as Arduino’s internal **pull-up resistor** will be used.

## ✅ 5. **Arduino Code:**

```cpp

```

## ✅ 6. **Working Principle:**

- The **PIR sensor** continuously monitors for changes in infrared radiation, which indicates motion.    
- When motion is detected, it sends a **HIGH signal** to the Arduino.    
- The Arduino then **activates the buzzer** to sound an alert.    
- If a reset button is included, pressing it **turns off the buzzer**, allowing manual acknowledgment of the alert.    

## ✅ 7. **Conclusion:**

This is a **simple yet effective theft detection system** using **Arduino Uno**, making use of basic components like a **PIR sensor and buzzer**. It's suitable for use in **homes, offices, or small shops**. The addition of a **reset button** makes it more user-friendly, allowing manual control after motion is detected.



---


1. _What is system programming?_ Describe the components of system programming.
> [!note] **Components of System Programming**
> System programming focuses on developing software that manages and controls computer hardware, enabling the execution of application programs. The following are the main components involved in system programming:
> 1. **Assembler**: An assembler is a system program that translates assembly language instructions into machine code. It performs tasks such as symbol resolution, instruction translation, and memory location assignment, enabling the processor to understand and execute the instructions.
> 2. **Loader**: A loader is responsible for loading the executable code into main memory for execution. It allocates memory space, resolves symbolic references, and prepares the program so that it can run properly on the system.
> 3. **Linker**: The linker combines multiple object files generated by compilers into a single executable file. It connects external function calls with their definitions and resolves address references, enabling smooth execution across different program modules.
> 4. **Compiler**: A compiler translates high-level programming language code into low-level machine or assembly code. It performs several stages such as lexical analysis, syntax analysis, semantic checking, optimization, and final code generation to produce efficient executable programs.
> 5. **Macro Processor**: A macro processor handles macros, which are pre-defined sequences of code. It replaces macro calls with actual code blocks before the program is compiled or assembled, thus reducing code repetition and increasing productivity.
> 6. **Debugger**: A debugger is used to detect and fix errors in a program. It allows the programmer to execute code step by step, set breakpoints, and inspect variable values at different stages of execution, which helps in identifying logical or runtime issues.
> 7. **Interpreter**: An interpreter directly executes high-level source code line by line without translating it into machine code in advance. This approach makes it easier to debug and test programs, although it may execute slower compared to compiled programs.
> 8. **System Libraries**: System libraries are collections of pre-written functions and routines that provide commonly used functionalities to system and application programs. They help reduce development time and ensure code reusability by offering standard solutions for frequent operations.
> 9. **Operating System (OS)**: The operating system is a core system software that acts as an interface between hardware and user programs. It manages hardware resources such as memory, CPU, I/O devices, and provides essential services like file management, multitasking, and process control.


2. Difference between system software and application software.

| **System Software**                                                                                                            | **Application Software**                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| System software manages and controls the hardware components of a computer and provides a platform for running other software. | Application software is designed to perform specific tasks for users, such as word processing, gaming, or web browsing. |
| It acts as an interface between the hardware and application software.                                                         | It directly serves the needs and tasks of the end user.                                                                 |
| It usually runs in the background and starts automatically when the computer boots.                                            | It runs only when the user launches it and terminates after use.                                                        |
| It is essential for the basic operation and functioning of the computer system.                                                | It is not essential for the computer to operate but adds functionality for the user.                                    |
| Users do not typically interact directly with system software; interaction is indirect or through other software.              | Users interact directly with application software via graphical user interfaces or commands.                            |
| Written mostly in low-level or system programming languages such as C or assembly.                                             | Written in high-level languages like Java, Python, or C#.                                                               |
| Examples include operating systems, device drivers, assemblers, compilers, and utility programs.                               | Examples include MS Office, Adobe Photoshop, web browsers, games, and media players.                                    |
| System software manages system resources like CPU scheduling, memory management, and file systems.                             | Application software focuses on solving user-specific problems and processing data for particular applications.         |
| Updates to system software often affect the entire computer’s performance and compatibility.                                   | Updates to application software typically add features or fix bugs related to specific user tasks.                      |
| System software provides a stable environment for applications to run securely and efficiently.                                | Application software depends on the system software environment to function                                             |


3.  What is Machine system? Illustrate how components of machine structure interact.

 > [!note] **What is a Machine System?**  
> A machine system is a structured physical system composed of mechanical, electrical, or electronic components that work together to perform a specific function. It is designed to receive input, apply force, control movement, and produce output using energy from sources such as electricity, heat, or natural forces.
> In the context of computing, a machine system typically includes a central processing unit (CPU), memory, input/output (I/O) devices, and storage units. These components interact to process data, execute instructions, and generate desired outcomes. Modern machine systems may also incorporate computers, sensors, and controllers, which are used to monitor and enhance system performance.

> [!note] **Illustration of Machine Structure Component Interaction**
> In a typical machine structure like the Von Neumann architecture, instruction execution happens through the organized interaction of key hardware components. Each part has a specific job and works with others in a set order to fetch, decode, execute instructions, and handle input/output. The main components and how they interact are explained below.

- **Program Counter (PC) / Location Counter (LC):** Holds the address of the next instruction to execute. It begins the cycle by placing this address into the **Memory Address Register (MAR)** and automatically increments to point to the subsequent instruction.
    
- **Memory Address Register (MAR):** Receives the address from the PC and forwards it to the memory system. This is how the system knows which memory location to access next—either to fetch an instruction or perform a data operation.
    
- **Memory Controller:** Interacts with the MAR to retrieve the instruction from the specified address in memory. It handles the memory access operation and sends the fetched data into the **Memory Buffer Register (MBR)**.
    
- **Memory Buffer Register (MBR):** Temporarily holds the fetched instruction (or data) coming from memory. Once the instruction is fetched, the MBR transfers it to the **Instruction Register (IR)** so it can be decoded.
    
- **Instruction Register (IR):** Stores the current instruction. This register makes the instruction available to the decoder while isolating it from other memory traffic during execution.
    
- **Instruction Decoder / Interpreter:** Reads the instruction from the IR, identifies what action is required (e.g., arithmetic, data transfer), and signals the involved components—like registers, the ALU, memory, or I/O devices—to perform their roles.
    
- **Working Registers:** Provide temporary storage during execution. When the decoder signals that operands are needed, they are loaded into these registers so operations (like addition or comparison) can be performed efficiently.
    
- **General Registers:** Hold constants, variables, or addresses that can be directly accessed during instruction execution. They are often used as the source or destination of data involved in the operation, depending on what the instruction requires.
    
- **System Buses (Data, Address, Control):** Act as the communication highways that allow all components to exchange information. The **Address Bus** carries memory addresses, the **Data Bus** carries instructions and values, and the **Control Bus** manages timing and signals like read/write commands.
    
- **Input/Output (I/O) Channels:** Handle external data exchange. If the instruction involves reading input (e.g., from a keyboard or sensor), the I/O channel sends that data to memory or registers. If the instruction outputs data, the I/O channel sends results from memory or registers to external devices like a display or printer.
    

Each component executes its role in sync with the others during every instruction cycle, forming a continuous loop of coordinated data flow and control that enables the system to function.


4. What is SDI & MDI? Explain MDI.

> [!note] SID
> **Single Document Interface (SDI)** is a type of graphical user interface where each document or file is opened in a **separate application window**. In SDI, every document window functions as an independent instance of the application, each with its own menu bar, toolbar, and controls. The operating system handles each window separately on the taskbar.
> This structure makes it easier for users to **work on one document at a time** and to **switch between applications** using the taskbar or Alt+Tab. However, managing multiple open documents may result in **taskbar clutter**, especially when many windows are open.
> **Examples of SDI applications** include:
> - Microsoft Notepad
> - Paint
> - Older versions of Microsoft Word

> [!note] MDI
> **Multiple Document Interface (MDI)** is a graphical user interface design where **multiple documents are opened within a single parent window**. The main (parent) window acts as a container that holds multiple child windows, each displaying a separate document. The child windows share the parent’s menu bar, toolbar, and status bar.
> MDI applications are useful when users need to **work with several documents at the same time**, such as comparing files, copying content between documents, or viewing related data side-by-side. The user can arrange child windows by cascading or tiling them within the parent window.
> This model helps to reduce taskbar clutter, but it can be limiting in multi-monitor environments or when users want to view documents in separate screens.
> **Examples of MDI applications** include:
> - Microsoft Visual Studio
> - Adobe Photoshop
> - Microsoft Excel (older versions)


> [!note] **Explanation of MDI**
> #### **Parent-Child Structure**
>  MDI follows a parent-child architecture where the main window acts as the **parent**, and multiple documents or views open as **child windows** within it. These child windows are confined within the boundaries of the main window and cannot exist outside it.
>  
> #### **Single Menu Bar**
> In MDI applications, there is only **one menu bar and toolbar** shared across all child windows. The options on the menu bar dynamically change based on which child window is active, maintaining a consistent interface and reducing redundancy.
> 
> #### **Efficient Management** 
> MDI provides built-in features like **window tiling, cascading, maximizing/minimizing**, and switching between documents. Users can work with multiple files or views more efficiently without needing to switch between separate application windows.
> 
> #### **Examples of MDI Applications**
> Popular software that uses MDI includes **Microsoft Visual Studio**, **Adobe Photoshop**, and older versions of **Microsoft Excel**. These applications allow users to open, edit, and compare multiple files or projects within one interface.


> [!note] Advantages of MDI
> - Easy to manage **multiple files** within a single application window
> - Reduces **taskbar clutter** as only one window appears in the taskbar
> - **Shared resources** like toolbars, menus, and status bars save space and provide uniformity
> - Improves **workflow efficiency** when dealing with multiple related documents

> [!note] Disadvantages of MDI
> - Less suitable for **multi-monitor environments** as all child windows are confined to one parent window
> - If the **parent window crashes**, all child documents are affected and may be lost
> - Can be **confusing for beginners** if too many child windows are opened at once
> - Not as **flexible** as SDI in managing unrelated tasks or documents

> In a Multiple Document Interface (MDI), the parent window acts as a central workspace where multiple child documents can be opened and viewed simultaneously. Each child window remains within the bounds of the main application window, making it easier to organize and manage multiple files without switching between multiple application instances.

> This design allows users to **compare documents side-by-side**, **copy and paste content between them**, and **perform tasks across multiple files** more efficiently. The interface usually provides options to **tile** or **cascade** child windows, giving users control over how they view and arrange their documents.

> Furthermore, since all documents are contained within a single window, **taskbar clutter is minimized**, and switching between documents becomes more streamlined using the application’s internal controls (like window menu or tab view). This structure is particularly helpful in applications that involve multitasking or working with interrelated documents.

> However, MDI also has some limitations. For example, users cannot drag and display individual documents on separate screens in a multi-monitor setup, as all documents are confined within the parent window.

> Overall, MDI is a powerful interface model for document-heavy applications, providing an efficient and organized workspace under one unified environment.

---


1. What is activeX? Explain activeX control and activeX components.
### ✅ What is ActiveX?

**ActiveX** is a **software framework developed by Microsoft** that enables applications to share information and functionality through web browsers and desktop environments, regardless of the programming language in which they're written. It allows for the embedding of multimedia content, interactive objects, and software updates directly into web pages or applications.

Originally introduced in **1996**, ActiveX was primarily used with **Microsoft products** like Internet Explorer, Word, and Excel. ActiveX controls function similarly to web browser plug-ins and are especially useful for enhancing a browser’s capabilities—such as playing videos, displaying interactive content, or running specific business applications—without requiring separate software.

However, most ActiveX controls work only on **Windows platforms** and are generally limited to **Internet Explorer**, making them less compatible with modern cross-platform web standards.

---

### ✅ ActiveX Control

![[WhatsApp Image 2025-06-21 at 21.02.59_a4cd1f0e.jpg]]

**Example**: A video player embedded in a website, a date-picker in an Excel sheet, or a calculator component within a program.

---

### ✅ ActiveX Components

ActiveX Components are the **building blocks** of the ActiveX technology. They are **reusable software objects** developed using **COM (Component Object Model)** architecture. These components can be integrated into various programming environments (such as Visual Basic, C++, and .NET) and used across different applications.

ActiveX Components are designed to be **language-independent** and **binary compatible**, making it easy for developers to embed rich functionalities into their applications. These components can be:

1. **ActiveX Controls**:  
    Interactive, visual elements like buttons, sliders, calendars, or media players that can be embedded in applications or webpages.
    
2. **Automation Objects**:  
    Non-visual components that expose services or methods for automating tasks, such as a spell checker, calculator engine, or database access component.
    
3. **ActiveX DLLs and EXEs**:  
    Binary files that contain compiled classes, methods, or services.    
    - **ActiveX DLLs** are in-process servers, providing functionalities within the host application’s process.        
    - **ActiveX EXEs** are out-of-process servers, providing services that run in their own process and can be used by multiple clients.



4. Explain DMA controller with suitable diagram.

A **DMA (Direct Memory Access) Controller** is a hardware component that enables high-speed data transfer directly between **main memory** and **I/O devices**, without the continuous involvement of the **CPU**. It is especially useful in systems where large blocks of data need to be moved frequently, such as in disk access, audio/video streaming, and communication devices.

### Benefits

- **Faster data transfer** without CPU intervention    
- **Efficient CPU utilization**, allowing multitasking    
- **Reduced CPU overhead** and improved system throughput

---

In traditional data transfer, the CPU actively reads data from an I/O device and writes it to memory (or vice versa), which consumes significant CPU time and slows overall system performance.

The DMA controller eliminates this bottleneck by independently managing data transfers. The CPU initiates the process by configuring the DMA controller with:

- The **starting memory address** for data transfer,    
- The **number of data words/bytes** to transfer,    
- The **direction** of transfer (memory to device or device to memory).    

Once configured, the DMA controller **takes control of the system buses** (address, data, and control lines) and transfers data **directly between memory and the I/O device**, freeing the CPU to perform other tasks.

After completing the transfer, the DMA controller **raises an interrupt signal** to inform the CPU that the operation is finished.

---

![[Pasted image 20250621204937.png]]

![[Pasted image 20250621210206.png]]

The figure illustrates the DMA controller connected to the system bus, memory, CPU, and an I/O device. The CPU initializes the DMA controller by providing the transfer parameters. The DMA controller then takes over the system bus to transfer data directly between memory and the I/O device. Upon completion, the DMA controller sends an interrupt to the CPU, signaling the end of the transfer.


5. Difference between microprocessor and microcontroller.

|Point|**Microprocessor**|**Microcontroller**|
|---|---|---|
|**Definition**|A microprocessor is a general-purpose central processing unit (CPU) on a single chip.|A microcontroller is an integrated chip that contains a CPU, RAM, ROM, I/O ports, and other peripherals.|
|**Components**|Requires external components like RAM, ROM, and I/O for operation.|Includes RAM, ROM, I/O, and sometimes timers, ADC/DAC built on the same chip.|
|**Applications**|Used in personal computers, workstations, and servers for complex processing.|Used in embedded systems like washing machines, sensors, automotive, robotics, etc.|
|**Cost**|Expensive due to the requirement of external components.|Cost-effective as it has built-in components.|
|**Power Consumption**|Higher due to external component connections.|Lower, ideal for low-power applications.|
|**Clock Speed**|Typically higher clock speeds (GHz range).|Lower clock speeds (MHz range), optimized for control tasks.|
|**Design Focus**|Focused on processing raw data and running complex programs.|Focused on controlling external devices and sensors.|
|**Example**|Intel 8085, Pentium, AMD Ryzen.|Atmel ATmega328, PIC16F877|

4. Design and write the code for any logic gate (AND, OR, or NOT ) using Arduino uno and LED.

### ✅ Objective

To design and implement an **AND gate** using an Arduino Uno and an LED. The LED will only turn ON when both input switches are ON, mimicking the behavior of an AND gate.

---

### ✅ Circuit Description (Written Explanation)

The circuit uses **two input switches** connected to the Arduino as digital inputs, and an **LED** connected to one of the Arduino’s digital pins. The Arduino reads the state of both switches. If both switches are ON, the Arduino turns ON the LED. Otherwise, the LED remains OFF.

---

### ✅ Pin Connections (in words)

- Switch A is connected to **digital pin 2** of the Arduino.    
- Switch B is connected to **digital pin 3** of the Arduino.    
- An LED, with a **220 Ω resistor** in series, is connected to **digital pin 13** of the Arduino.    

---

### ✅ Logic Explanation

The program reads both inputs (switch A and switch B). According to the AND gate truth table:

- If **both switch A and switch B are ON**, the LED turns ON.    
- In all other cases, the LED remains OFF.  
    This demonstrates the working of an AND gate.    

---

### ✅ Arduino Code

```cpp
// AND Gate Demo using Arduino Uno

const int switchA = 2;
const int switchB = 3;
const int ledPin = 13;

void setup() {
  pinMode(switchA, INPUT);
  pinMode(switchB, INPUT);
  pinMode(ledPin, OUTPUT);
}

void loop() {
  int stateA = digitalRead(switchA);
  int stateB = digitalRead(switchB);

  // AND Gate Logic
  if (stateA == HIGH && stateB == HIGH) {
    digitalWrite(ledPin, HIGH); // LED ON
  } else {
    digitalWrite(ledPin, LOW);  // LED OFF
  }
}
```