---
title: Polyspace & SonarQube
---

# 🧪 Polyspace & SonarQube

This section focuses on static analysis tools used in the automotive domain for quality assurance and safety compliance.

---

## Sample Q&A

**Q1. What is Polyspace used for?**  
**A:** Polyspace is a static analysis tool that detects runtime errors, code defects, and MISRA violations in embedded C/C++ code.

**Q2. How does Polyspace detect runtime errors without executing code?**  
**A:** It performs formal methods analysis based on abstract interpretation to mathematically prove the absence of certain runtime errors.

**Q3. What are some key error categories Polyspace highlights?**  
**A:** Division by zero, out-of-bounds array access, null pointer dereferencing, and uninitialized variables.

**Q4. What does a green code annotation mean in Polyspace?**  
**A:** It indicates the absence of runtime errors (code is proven safe).

**Q5. What are red annotations in Polyspace?**  
**A:** Red highlights indicate definite runtime errors that must be fixed.

**Q6. How is SonarQube different from Polyspace?**  
**A:** SonarQube is more focused on code quality, maintainability, and code smells, whereas Polyspace targets safety and runtime issues.

**Q7. What types of metrics does SonarQube provide?**  
**A:** Code smells, cyclomatic complexity, duplication, code coverage, bugs, and vulnerabilities.

**Q8. Can SonarQube be integrated with Jenkins or GitHub?**  
**A:** Yes, it integrates easily with CI/CD pipelines and version control systems.

**Q9. How do you handle MISRA compliance in Polyspace?**  
**A:** Use rule checkers and configure the analysis for specific versions of MISRA standards.

**Q10. What is the benefit of using both tools?**  
**A:** Polyspace ensures safety and standards compliance; SonarQube ensures maintainability and quality.
