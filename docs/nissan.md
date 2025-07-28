# 🚗 Nissan Interview Experience
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>
**Role:** Embedded System Engineer – Powertrain Domain  
**Mode:** Hybrid (Initial rounds online, final at plant)  
**Location:** Chennai + Onsite interaction with Japan counterparts  
**Rounds:** 3 Technical + 1 Managerial + 1 HR

---

## 🧪 Technical Round 1: ECU + Requirement Analysis + System Knowledge

**Topics Touched:**
- ECU fundamentals
- Engine-Side system knowledge
- Requirement decomposition
- System to Software handoff
- ARXML usage

**Sample Questions:**

1. **How do you differentiate system-level requirements and software-level requirements?**  
   *(They emphasized ISO 26262 boundary clarity.)*

2. **What are the basic functional blocks in an engine control ECU?**  
   *(Expect references to injection control, crankshaft timing, etc.)*

3. **Have you created SWCs from ARXML and ECU extracts? Explain the process.**

4. **How do you analyze customer-level engine performance requirements and convert them into implementable software logic?**

5. **What is the significance of requirement traceability during change requests in ECUs?**

6. **What tools have you used for requirement writing and version control?**  
   *(Expected answers: Polarion, DOORS, or similar.)*

---

## 🔬 Technical Round 2: Model Development + Virtual vs Non-Virtual Blocks + Testing

**Topics Touched:**
- Simulink modeling with OEM standard libraries
- Virtual/Non-virtual block usage
- SWC Integration + AUTOSAR
- SIL testing and GTest integration

**Sample Questions:**

1. **Can you explain the difference between virtual and non-virtual subsystems in Simulink?**  
   *(Follow-up: When to use which in production-grade ECUs?)*

2. **How is your model development guided by the ARXML and ECU extract files?**

3. **Walk us through the model-to-code generation process using TargetLink or Embedded Coder.**

4. **What type of ports have you configured while designing SWCs? What’s the importance of sender-receiver vs client-server interfaces?**

5. **How do you validate SWC functionality in GTest? Can you describe how you setup SIL-based test scenarios?**

6. **Have you worked on CAN signal testing or integrating DBCs in your simulation environment?**

---

## 🏭 Technical Round 3: Manufacturing Awareness + System Maturity + International Collaboration

**Topics Touched:**
- Plant interaction and calibration flow
- Communication with Japan teams
- Plant-based integration of ECU software
- Manufacturing defect feedback loop

**Sample Questions:**

1. **What changes are necessary in an ECU when moving from prototype testing to manufacturing calibration?**

2. **How do you collaborate with Japan teams when local plant requirements conflict with global architecture?**

3. **Explain how real-vehicle data logs help in refining engine control models.**

4. **What exposure do you have to mass production defect reporting and feedback loop from manufacturing to engineering?**

5. **How do you ensure synchronization between multiple departments (testing, calibration, manufacturing, requirement) across geographies?**

---

## 👨‍💼 Managerial Round

- Asked about previous project deliveries, deadlines, change management
- Japanese work ethic and precision-based discussions
- Enthusiasm about working in cross-cultural teams
- Communication expectations in Japan-headquartered environments

---

## 📝 Final Notes

- Interview structure emphasized **Japanese precision** and **methodical documentation**.
- Strong **modeling and validation** background using ARXML-based flow and ECU-specific implementations was crucial.
- GTest knowledge for **unit + SIL testing** was a big plus.
- Manufacturing and plant calibration exposure added strong weightage.
- Virtual vs Non-virtual subsystem clarity was expected even at junior levels.
