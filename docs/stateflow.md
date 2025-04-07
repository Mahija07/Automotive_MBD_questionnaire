---

title: Stateflow
----

# 🔁 Stateflow

Covers:

- State hierarchy
- Events and transitions
- Truth tables and temporal logic

---

**Q1. How is a state transition triggered in Stateflow?**

**A:** By an event or a condition being satisfied, depending on the transition guard.

**Q2. What is a junction in Stateflow?**

**A:** A graphical element to combine multiple transitions or simplify paths.

**Q3. What is a temporal condition?**

**A:** A condition based on time, like `after(5,sec)`.

**Q4. What are truth tables used for?**

**A:** To express complex conditional logic in a tabular form.

**Q5. What is the difference between entry and during actions?**

**A:** Entry actions execute once upon entering a state, during actions execute every time step while the state is active.

**Q6. What are local and output data in Stateflow?**

**A:** Local is internal data, output is passed to the Simulink model.

**Q7. What is a parallel state?**

**A:** A state that runs concurrently with other parallel states.

**Q8. How do you integrate Simulink and Stateflow?**

**A:** Via input/output signals and function calls between the two.

**Q9. What is history junction?**

**A:** It remembers the last active substate when a superstate is re-entered.

**Q10. How do you debug a Stateflow chart?**

**A:** Use chart animation, logging, and debug breakpoints.
