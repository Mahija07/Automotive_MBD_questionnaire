# 📚 SAFETY STANDARDS 

### ✅ **What are Safety Standards?**
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

Safety standards in automotive software define structured processes and guidelines to ensure the **functional safety**, **reliability**, and **compliance** of electronic systems and software in vehicles.

---

### 📅 **When do we use them?**

- During **development of safety-critical ECUs** (like brakes, airbags, ADAS)
- When targeting **compliance certifications**
- In **design, testing, validation, and verification** phases
- Especially for **ASIL-classified systems (A-D)**

---

### 🌍 **Where are they used?**

- In **OEMs and Tier-1 suppliers**
- Across the **entire V-model lifecycle**
- In **hardware and software** development for:
  - Powertrain
  - ADAS/Autonomous features
  - Lighting
  - Chassis
  - Diagnostics

---

### ❓ **Why do we use them?**

- To prevent **loss of life and damage**
- To fulfill **legal, regulatory, and customer requirements**
- To **reduce risk** through structured safety analysis (FMEA, HARA)
- To achieve **ASIL compliance (Automotive Safety Integrity Level)**

---

### ⚙️ **How do we use them?**

- Apply **ISO 26262** for functional safety
- Use tools that comply with **MISRA C**, **ASPICE**, or **ISO/PAS 21448 (SOTIF)**
- Follow structured **requirements traceability**, **code verification**, and **testing**
- Perform **FMEA**, **FTA**, **Safety Goals**, **HARA**, **Safety Cases**

---

### 🌟 **Benefits**

- ✅ Ensures **human safety**
- ✅ Boosts **product reliability and credibility**
- ✅ Meets **regulatory mandates**
- ✅ Reduces **product recalls and liability**
- ✅ Improves **customer trust** and brand value

---

### **Interview Questions and Answers on Safety Standards in Automotive**

---

**1. What is ISO 26262?**  
A functional safety standard for automotive electrical and electronic systems.

**2. Why is ISO 26262 important?**  
It ensures the vehicle functions safely under both normal and fault conditions.

**3. What is Functional Safety?**  
The absence of unreasonable risk due to hazards caused by malfunctioning behavior of E/E systems.

**4. What are the major parts of ISO 26262?**  
It includes 12 parts, from vocabulary to hardware/software development, ASIL determination, etc.

**5. What is ASIL?**  
Automotive Safety Integrity Level — defines risk levels (A to D) with D being the highest.

**6. What is HARA?**  
Hazard Analysis and Risk Assessment — used to determine ASIL and identify safety goals.

**7. What is a Safety Goal?**  
A high-level safety requirement derived from HARA to mitigate hazards.

**8. What is a Safety Case?**  
Documented evidence showing that safety goals are met and the system is safe.

**9. What is FMEA?**  
Failure Modes and Effects Analysis — identifies potential failure points in a system.

**10. What is FTA?**  
Fault Tree Analysis — top-down approach to identify causes of system failure.
 
**11. What is the V-model in ISO 26262?**  
A development process showing relationship between development and verification activities.

**12. What is the role of tool qualification in ISO 26262?**  
To ensure tools used in development don't introduce undetected errors.

**13. What is freedom from interference?**  
Separation of software components with different ASILs to prevent negative impact.

**14. What are safety mechanisms?**  
Software or hardware features that detect, prevent, or control failures.

**15. What are the software development phases in ISO 26262?**  
Initiation, specification, architectural design, implementation, testing.

**16. What is ASPICE?**  
Automotive SPICE — a process improvement model for automotive software development.

**17. Difference between ASPICE and ISO 26262?**  
ASPICE focuses on process quality; ISO 26262 focuses on functional safety.

**18. What is a safety requirement?**  
A requirement created to mitigate risks identified during safety analysis.

**19. What is SOTIF?**  
Safety of the Intended Functionality — ISO/PAS 21448 — covers risks from system limitations, not failures.

**20. What is the role of MISRA C?**  
A set of C programming guidelines to ensure safe and reliable code in automotive systems.
 
**21. What are typical safety-related ECUs?**  
Airbag, ABS, ESP, ADAS controllers, engine control, etc.

**22. What is software verification in ISO 26262?**  
Ensures software meets its requirements through testing and reviews.

**23. What is hardware-software interface (HSI)?**  
Documentation describing interaction between hardware and software.

**24. What are confidence levels in tool qualification?**  
TCL 1–3: higher confidence required for more critical tools.

**25. Can ISO 26262 be applied to motorcycles?**  
Yes, through ISO 26262 Part 12 or extensions.

**26. What is a dependent failure?**  
A failure in one component causing another to fail — must be analyzed and avoided.

**27. What is robustness testing?**  
Testing to ensure software behaves reliably under stress or faults.

**28. What is fault injection?**  
Introducing errors to validate the system's fault detection and handling.

**29. What is a safety culture?**  
A company-wide mindset and practice focused on safety at every level.

**30. What are software safety requirements?**  
Detailed requirements derived from safety goals to be implemented in code.
 
**31. What is a development interface agreement (DIA)?**  
Defines responsibilities between supplier and OEM for safety activities.

**32. What is traceability?**  
Mapping requirements to design, code, and test cases to ensure complete coverage.

**33. What is latent fault?**  
A fault present in the system but not yet detected.

**34. What is diagnostic coverage (DC)?**  
Percentage of faults that can be detected and handled properly.

**35. What is safe state?**  
A system state that is considered safe in case of failure (e.g., reduced speed, emergency stop).

**36. What is a QM level?**  
Quality Management level — non-safety-related classification in ISO 26262.

**37. What’s the difference between ASIL A and ASIL D?**  
ASIL A is low criticality; ASIL D is the most stringent safety requirement.

**38. What is software architectural design?**  
Defines the structure of software components and interactions, especially for safety partitioning.

**39. What is requirement decomposition?**  
Breaking high-level requirements into detailed, manageable sub-requirements.

**40. What are verification techniques?**  
Reviews, inspections, static analysis, dynamic testing, etc.
 
**41. What is the purpose of safety validation?**  
To ensure the final product meets safety goals under real-world conditions.

**42. What are safety-related anomalies?**  
Unexpected behaviors that could lead to unsafe operation.

**43. What is change impact analysis?**  
Evaluating the impact of changes on safety requirements and the system.

**44. What is a watch-dog timer?**  
A safety mechanism that resets the system in case of software hang.

**45. How is memory protection achieved?**  
Using MMU, MPU, or OS services to avoid unsafe memory access.

**46. How is software configuration managed?**  
Through version control, baselines, and change control to ensure traceability.

**47. What’s the role of test coverage metrics?**  
To measure how much code or requirements have been tested.

**48. Can ISO 26262 be applied to AI-based systems?**  
Only partially — SOTIF (ISO 21448) complements it for perception and learning systems.

**49. How is documentation handled in safety projects?**  
Extensive documentation is mandatory for traceability, auditing, and compliance.

**50. How do safety standards improve product quality?**  
They enforce disciplined development, robust testing, and reduce the risk of defects reaching users.