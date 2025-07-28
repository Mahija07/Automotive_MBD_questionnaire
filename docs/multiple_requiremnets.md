# 💡 Simulink Requirements – MATLAB Implementation Ideas
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>
These requirements are ideal for Level 1 & 2 interviews and practical automotive model-based design projects. They can be implemented in MATLAB/Simulink and validated using Simulink Requirements, Traceability, and Test Manager.

---

## 🚦 1. Brake Light Control System

**Requirement:**  
- If the brake pedal is pressed, the brake lights shall turn ON.  
- If the brake pedal is not pressed, the brake lights shall turn OFF.

**Inputs:**  
- `Brake_Pedal_Status` (Boolean)

**Output:**  
- `Brake_Light` (Boolean)

**Implementation Hints:**  
- Use `If-Else` or logical operator blocks.  
- Model must respond instantly to pedal press.  
- Link requirement via Simulink Requirements.

---

## 🌡️ 2. Temperature Warning System

**Requirement:**  
- When engine temperature exceeds 95°C, turn ON the warning indicator.  
- When engine temperature falls below 90°C, turn OFF the warning indicator.

**Inputs:**  
- `Engine_Temp` (double, °C)

**Output:**  
- `Temp_Warning_Lamp` (Boolean)

**Implementation Hints:**  
- Use Hysteresis logic to avoid flickering.  
- Apply memory block for state retention.

---

## 🛑 3. Emergency Stop Logic

**Requirement:**  
- If both Brake_Pedal is pressed AND Obstacle_Detected is true, trigger Emergency_Stop.

**Inputs:**  
- `Brake_Pedal_Status` (Boolean)  
- `Obstacle_Detected` (Boolean)

**Output:**  
- `Emergency_Stop` (Boolean)

**Implementation Hints:**  
- Use AND logical block or condition action subsystem.  
- Test multiple scenarios using signal builder or test harness.

---

## ⛽ 4. Low Fuel Indicator System

**Requirement:**  
- Turn ON Low_Fuel_Lamp when Fuel_Level falls below 10%.  
- Turn OFF when Fuel_Level rises above 15%.

**Inputs:**  
- `Fuel_Level` (percentage, double)

**Output:**  
- `Low_Fuel_Lamp` (Boolean)

**Implementation Hints:**  
- Use Compare To Constant and Logic blocks.  
- Add simulation data inspector traceability.

---

## 🔄 5. Gear Shift Requirement

**Requirement:**  
- If Vehicle_Speed > 40 and Engine_RPM > 2500, Shift Up.  
- If Vehicle_Speed < 20 and Engine_RPM < 1500, Shift Down.

**Inputs:**  
- `Vehicle_Speed` (km/h)  
- `Engine_RPM` (rpm)

**Outputs:**  
- `Shift_Command` (Enum: `UP`, `DOWN`, `HOLD`)

**Implementation Hints:**  
- Use MATLAB Function block or Multiport Switch.  
- Integrate with Stateflow for gear logic.

---

## 🔧 How to Use in Simulink

- 📎 Link each requirement to the model block via **Simulink Requirements**.
- 📊 Use **Simulink Test** to create test cases for each scenario.
- ✅ Validate using **coverage metrics**, **MIL** or **SIL**.
- 🔗 Maintain bidirectional traceability with requirement documents.

---

📝 *You can extend these with AUTOSAR properties, integrate into SWCs, or simulate with CAN messages as per domain-specific projects (Maruti, Bosch, Nissan, etc.)*

