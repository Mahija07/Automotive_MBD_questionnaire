# 🚗 Model-Based Design (MBD) Interview Questions

---<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

## 📦 MATLAB & Auto Code Generation

1. What is auto code generation in Simulink?  
2. What is the difference between GRT and ERT targets?  
3. What is the role of TLC (Target Language Compiler) files?  
4. What are the key features of Embedded Coder?  
5. How do you configure model settings for code generation?  
6. What are storage classes in auto code generation?  
7. What is the difference between reusable function and inlined code generation?  
8. How can you reduce code size during generation?  
9. What is the significance of the model's configuration parameters for code generation?  
10. What are example applications where auto code generation is used?  

---

## 🔧 Simulink Modeling

11. What are the basic block types used in Simulink?  
12. What is a virtual vs non-virtual subsystem?  
13. What are lookup tables and when would you use them?  
14. How do you implement a feedback control loop in Simulink?  
15. What is the purpose of Bus Creator and Bus Selector?  
16. What is the function of a Merge block?  
17. What are Rate Transition blocks and when are they required?  
18. What is the difference between Enable and Trigger subsystems?  
19. How do you create a masked block?  
20. What is function-call subsystem and when is it used?  

---

## 🔁 Stateflow & Flow Logic

21. What is Stateflow and how does it differ from Simulink?  
22. What is the difference between Exclusive OR and AND states in Stateflow?  
23. What are junctions in Stateflow and how are they used?  
24. What is the role of temporal logic in Stateflow?  
25. What is the difference between event-based and time-based transitions?  
26. How do you model hierarchy and parallelism in Stateflow?  
27. What is a history junction?  
28. How can you simulate faults or error-handling logic in Stateflow?  
29. What are condition actions and transition actions?  
30. What are the execution order rules in Stateflow?  

---

## 📊 Flowcharts & Logical Modeling

31. How do you convert a flowchart into a Simulink model?  
32. What are Mealy and Moore machines? How are they modeled in Stateflow?  
33. What is the difference between transition condition and state entry action?  
34. How would you implement nested states in Stateflow?  
35. What is superstate and substate concept?  

---

## ⚙️ Model Configuration & Optimization

36. How do you configure a model for real-time simulation?  
37. What are common optimization settings for embedded code generation?  
38. What is inline parameter and when should it be used?  
39. How do you control sample times and solver settings?  
40. What is signal resolution and how is it configured?  

---

## ✅ Testing & Verification

41. What are the steps to perform MIL testing?  
42. What is signal logging and how is it enabled?  
43. How do you use Simulink Test Manager?  
44. How do you verify that the generated code behaves like the model?  
45. What are model coverage metrics and why are they important?  

---

## 🔍 Miscellaneous & Practical

46. What are common errors during code generation and how do you resolve them?  
47. How do you manage large models or componentize them?  
48. What is model referencing and its benefits?  
49. How do you ensure MISRA C compliance in the generated code?  
50. What debugging tools do you use while working with Simulink and code?  

---

## 🧱 Advanced Modeling & Architecture

51. What is the use of model variants in Simulink?  
52. How do you use Variant Subsystems and Variant Source/Sink blocks?  
53. What is configuration referencing and how is it useful?  
54. How does model referencing improve reusability?  
55. What is the difference between model reference and subsystem?  
56. How do you create reusable libraries in Simulink?  
57. How do you manage calibration parameters across models?  
58. What is data dictionary in Simulink?  
59. How is signal logging different from data logging?  
60. What is signal aliasing and how do you manage it?  

---

## 🧩 Code Integration & Data Handling

61. What is the use of external input/output in Simulink models?  
62. How do you link model parameters to external code or calibration files?  
63. How do you create A2L/MDF files for calibration and measurement?  
64. What are calibration annotations in Embedded Coder?  
65. How do you manage memory sections in code generation?  
66. What is difference between volatile and non-volatile data?  
67. How do you ensure your model supports ASIL (Automotive Safety Integrity Level)?  
68. What is the role of pragma or memory mapping in generated code?  

---

## 🔀 Stateflow Advanced

69. How do you prioritize transitions in Stateflow?  
70. How does event broadcasting work?  
71. How do you use MATLAB functions inside Stateflow?  
72. What is difference between graphical and truth table functions?  
73. How do you model a watchdog mechanism in Stateflow?  
74. What are state decomposition and parallel states?  
75. How do you control execution order of parallel states?  

---

## 🐞 Debugging, Performance & Safety

76. What are common issues you’ve debugged in model simulations?  
77. What are execution order viewer and signal monitoring tools?  
78. What is simulation profiler and when do you use it?  
79. What are some code verification strategies you follow?  
80. How do you integrate Polyspace for static code analysis?  
81. How do you test time deterministic behavior of the model?  
82. What are checks you run before delivering model/code?  

---

## 🛡️ Safety & Process Compliance

83. How do you ensure compliance to ISO 26262 in your modeling process?  
84. What are safety mechanisms modeled using Stateflow?  
85. What is the importance of requirement traceability?  
86. What are Simulink Requirements and how do you use them?  
87. What are change impact assessments in modeling?  

---

## 🌍 Simulation & Environment

88. How do you simulate physical systems in Simulink (e.g., using Simscape)?  
89. What is co-simulation and how do you perform it?  
90. What is SIL/PIL testing? How is it configured?  
91. What are host-target interface considerations?  
92. How do you set up hardware-in-the-loop (HIL) testing?  

---

## 📂 Process, Documentation & Collaboration

93. What are your steps from model creation to production code delivery?  
94. How do you version control Simulink models?  
95. What documentation tools do you use for Simulink models?  
96. How do you handle change requests in models?  
97. What is your process for model review or design peer-review?  
98. How do you manage test cases for MIL/SIL validation?  
99. What do you include in your model test harnesses?  
100. How do you ensure model readability and maintainability?  