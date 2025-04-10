# 📚 EMBEDDED C

<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

### 🧠 **What is Embedded C?**

**Embedded C** is an extension of the C programming language tailored for **embedded systems development** — systems with limited hardware (memory, CPU) and tight real-time constraints. It's used to program microcontrollers like **8051, ARM, PIC, AVR**, etc.

---

### 📅 **When is Embedded C Used?**

- When you're writing software for **microcontrollers or embedded devices**.
- During **firmware development** for products like automotive ECUs, IoT devices, washing machines, medical devices, etc.
- Anytime **performance, memory usage, and timing** are critical.

---

### 🌍 **Where is Embedded C Used?**

- Automotive ECUs (Engine Control Units, Body Control Modules)
- Consumer electronics (TVs, Washing Machines, Microwaves)
- Industrial automation
- Healthcare devices
- Aerospace control systems
- Robotics and IoT systems

---

### ❓ **Why Use Embedded C?**

- It's **close to hardware**, allowing precise control of registers, ports, timers, etc.
- **Portable** across different microcontrollers (with proper abstraction).
- Efficient for **real-time applications** where timing and performance matter.
- Supported by almost all **embedded toolchains and compilers** (e.g., Keil, IAR, MPLAB, STM32CubeIDE).

---

### ⚙️ **How Do We Use Embedded C?**

- Write your C code using microcontroller-specific **register definitions**, **memory-mapped I/O**, and **ISR functions**.
- Use **predefined headers and drivers** provided by microcontroller vendors.
- Build and compile the code using a suitable IDE or toolchain.
- Flash the binary to the target microcontroller.

Example (for an 8051):

```c
#include <reg51.h>

void main() {
  while(1) {
    P1 = 0xFF;  // Set all pins on port 1
  }
}
```

---

### 🌟 **Benefits of Embedded C**

- 🔹 Efficient execution in resource-constrained environments
- 🔹 Precise control of hardware
- 🔹 Portable with minimal changes
- 🔹 Easy to maintain and modular
- 🔹 Structured programming for better development practices
- 🔹 Strong community support and vast legacy code

---

### **Interview Questions and Answers for Embedded C**

---

### 🔧 Embedded C – Interview Questions & Answers

**1. What is Embedded C?**  
Embedded C is a set of language extensions for the C Programming Language to support embedded processors and microcontrollers.

**2. How is Embedded C different from C?**  
Embedded C includes direct access to hardware through memory-mapped I/O and register manipulation, unlike standard C.

**3. What are the key features of Embedded C?**  
Portability, efficiency, low-level access, hardware interfacing, and deterministic execution.

**4. What are microcontrollers?**  
Microcontrollers are small computing systems on a chip that control embedded devices.

**5. What is the use of `volatile` keyword?**  
It tells the compiler that a variable can change at any time, preventing optimization that could ignore changes.

**6. What is an ISR?**  
Interrupt Service Routine – a function triggered when a hardware interrupt occurs.

**7. How do you declare an ISR in Embedded C?**  
Using compiler-specific syntax. For 8051: `void isr() interrupt 1`.

**8. What is the role of registers?**  
Registers are memory locations inside the microcontroller used for data storage and control.

**9. What are the data types commonly used?**  
`int`, `char`, `unsigned`, `float`, `uint8_t`, `uint16_t`, etc.

**10. What is memory-mapped I/O?**  
Peripheral devices are assigned specific memory addresses that can be accessed like regular variables.

**11. How do you turn on an LED in Embedded C?**  
```c
P1 = 0x01; // Turns on LED connected to P1.0
```

**12. What is bit manipulation?**  
Directly modifying bits for controlling specific hardware features.

**13. Explain `sbit` keyword.**  
Used to access individual bits of a special function register.

**14. What is a watchdog timer?**  
A hardware timer that resets the system if the software becomes unresponsive.

**15. What is polling?**  
Continuously checking the status of a peripheral or flag.

**16. What is debouncing?**  
Filtering the noise when reading mechanical switch input.

**17. What is the stack used for?**  
Storing return addresses, local variables, and function parameters.

**18. What is the heap used for?**  
Dynamic memory allocation (though it's avoided in embedded systems).

**19. What are the memory sections?**  
Code, data, bss, stack, and heap.

**20. What is the difference between `const` and `#define`?**  
`const` defines typed variables, `#define` is preprocessor macro substitution.

**21. What is a real-time system?**  
A system where response time is critical, and tasks must execute within deadlines.

**22. What is a timer in embedded systems?**  
A counter used for time tracking or generating delays.

**23. How to generate delay in Embedded C?**  
Using timers or loops, e.g. `for(i=0;i<50000;i++);`.

**24. What is the difference between a microprocessor and microcontroller?**  
Microcontroller has CPU, memory, and I/O on one chip; microprocessor only has CPU.

**25. What is I2C?**  
A serial protocol for multi-device communication using 2 wires.

**26. What is SPI?**  
Serial Peripheral Interface, a fast communication protocol using 4 wires.

**27. What is UART?**  
Universal Asynchronous Receiver/Transmitter – used for serial communication.

**28. What is GPIO?**  
General-Purpose Input/Output – pins used to control or read digital signals.

**29. What is the purpose of `static` keyword?**  
Restricts variable scope to file or function.

**30. What is inline assembly in Embedded C?**  
Embedding assembly code in C for performance-critical tasks.

**31. What is `typedef`?**  
Used to define new names for data types.

**32. What is the purpose of `extern`?**  
Declares a variable defined elsewhere in another file.

**33. How do interrupts work in Embedded C?**  
Triggered by hardware, ISR is called to handle the event.

**34. What is the difference between `=`, `==`, and `===` in Embedded C?**  
`=` assigns, `==` compares; `===` doesn’t exist in C.

**35. What is firmware?**  
Software programmed into non-volatile memory of embedded systems.

**36. What are linker scripts?**  
Used to define memory layout and placement of code/data.

**37. How to optimize embedded code?**  
Avoid floating-point, reduce recursion, minimize memory, use efficient algorithms.

**38. What is the difference between `call` and `goto`?**  
`call` invokes a function with return, `goto` jumps unconditionally.

**39. What is bootloader?**  
A small program that loads main firmware into memory during startup.

**40. What is RTOS?**  
Real-Time Operating System used in complex embedded systems.

**41. What is context switching?**  
Changing the CPU from one task/process to another.

**42. What is DMA?**  
Direct Memory Access allows peripherals to transfer data without CPU.

**43. What are software debuggers?**  
Tools to trace, inspect, and control code execution (e.g., Keil, MPLAB).

**44. What are common IDEs for Embedded C?**  
Keil uVision, MPLAB X, STM32CubeIDE, Code Composer Studio.

**45. What is code profiling?**  
Analyzing code performance and identifying bottlenecks.

**46. What are volatile vs const volatile?**  
`volatile`: variable may change unexpectedly; `const volatile`: can change, but not modified in code.

**47. What is memory leak in embedded systems?**  
Failure to free unused memory — dangerous due to limited resources.

**48. What is the role of linker and compiler?**  
Compiler converts code to object file; linker combines into a final executable.

**49. What is endianess?**  
Byte order — Little Endian (LSB first) or Big Endian (MSB first).

**50. How to ensure safety in embedded development?**  
Follow MISRA C, use static analysis, test rigorously, use watchdogs.
