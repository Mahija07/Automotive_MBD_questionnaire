---

title: Code-Based Development (CBD)
----

# 💻 Code-Based Development (CBD)

This section includes:

- Embedded C and C++ fundamentals
- MISRA C rules
- Manual code development for automotive applications
- Best practices for maintainable and scalable code

---

## Sample Q&A

**Q1. What are some key MISRA C rules to follow in automotive software?**

**A:** Avoid dynamic memory allocation, ensure explicit type casting, and prevent use of unrestricted pointers.

**Q2. How can C++ be used in embedded systems?**

**A:** Through classes for encapsulation, templates for reusability, and namespaces for modular code.

**Q3. What is volatile keyword in embedded C?**

**A:** It tells the compiler not to optimize a variable that can change unexpectedly (like hardware registers).

**Q4. How do you manage memory in embedded C?**

**A:** Use static allocation, stack variables, and avoid heap where possible.

**Q5. What are macros and how are they used in embedded systems?**

**A:** Macros are preprocessor definitions used for constants and conditional compilation.

**Q6. What are the challenges of using pointers in embedded systems?**

**A:** Dangling pointers, null dereferencing, and memory corruption.

**Q7. How do you organize code in a multi-module embedded project?**

**A:** Using header files, abstraction layers, and separation of concerns.

**Q8. What is the use of bit manipulation in embedded code?**

**A:** Efficient control of hardware registers and flags.

**Q9. How do you implement ISR (Interrupt Service Routines)?**

**A:** By registering hardware interrupt handlers and keeping them short and efficient.

**Q10. What tools help maintain code quality in automotive development?**

**A:** MISRA checkers, SonarQube, Polyspace, static/dynamic analyzers.
