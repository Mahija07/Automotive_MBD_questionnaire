# 📚 GOOGLE TEST 

### ✅ **What is Google Test?**

**Google Test (GTest)** is a powerful **C++ unit testing framework** developed by Google.  
It lets developers write **automated test cases** to check the correctness of their C++ code — class functions, modules, and behaviors.
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

---

### 📅 **When do we use Google Test?**

We use GTest:
- During **unit testing** phase (early in the development cycle)
- When writing **test-driven development (TDD)**
- While integrating Continuous Integration (CI) pipelines (e.g., Jenkins, GitHub Actions)
- When validating logic-heavy or safety-critical code, e.g., in **automotive ECUs**
- For writing regression tests to ensure future code changes don’t break existing functionality

---

### 🌍 **Where do we use Google Test?**

It is used:
- In **C++ projects** across multiple domains (automotive, embedded, robotics, etc.)
- As part of **software validation toolchains**
- In **unit testing environments** like:
  - Visual Studio
  - Eclipse with CDT
  - CMake-based builds
  - GitLab CI, GitHub Actions, Jenkins
- In **automotive software units/modules** like diagnostics, lighting, driver assistance, etc.

---

### ❓ **Why do we use Google Test?**

Because:
- It helps catch **bugs early** in development
- Ensures **modular and reliable code**
- Makes refactoring safer with **test coverage**
- Encourages **cleaner design** by requiring testability
- It’s **free, open-source, and well-maintained**
- Supports **mocking** via Google Mock (gMock)

---

### 🌟 **Benefits of Google Test:**

- ✅ Easy to write and read test cases using macros like `EXPECT_EQ`, `ASSERT_TRUE`
- ✅ Provides detailed failure reports and logging
- ✅ Allows **parameterized tests** and **test fixtures**
- ✅ Integrates smoothly with **CI/CD pipelines**
- ✅ Supports **mocking** to simulate hardware or dependencies
- ✅ Cross-platform and highly customizable
- ✅ Makes your software **robust, testable, and production-ready**


### Coverage Types in GTest:

1. **Statement Coverage (Line Coverage)**
2. **Branch Coverage (Decision Coverage)**
3. **Path Coverage**
4. **Condition Coverage**
5. **Modified Condition/Decision Coverage (MC/DC)**

Each type of coverage ensures different aspects of the code are thoroughly tested.

---

### 1️⃣ **Statement Coverage (Line Coverage)**

**What It Means**:  
This coverage type ensures that **every line of code** in the program is executed at least once during the tests.

**How to Achieve It**:
- Create tests that trigger every line of your function/method.
- Each line of your function should be executed by at least one test case.

**Example**:

```cpp
bool checkEngineStatus(int engineTemperature, bool engineRunning) {
    if (engineRunning) {
        if (engineTemperature > 90) {
            return true;
        }
    }
    return false;
}
```

To cover this:

1. **Test 1**: `engineTemperature = 100, engineRunning = true` → hits line 3 and 4.
2. **Test 2**: `engineTemperature = 80, engineRunning = true` → hits line 3 but not line 4.

By running tests that cover both the `if` conditions, you achieve **Statement Coverage**.

**Tools**:  
- Use **gcov**, **lcov**, or **Bullseye** to measure line coverage.
  
---

### 2️⃣ **Branch Coverage (Decision Coverage)**

**What It Means**:  
This type ensures that **each decision point** (i.e., `if` or `switch` statements) takes on **both possible outcomes**—true and false.

**How to Achieve It**:
- Ensure that every **decision point** (condition inside an `if`, `while`, `switch`, etc.) evaluates to both **true** and **false**.

**Example**:

```cpp
bool isSpeedSafe(int speed) {
    if (speed > 120) {
        return false;  // dangerous
    } else {
        return true;   // safe
    }
}
```

To cover **branch coverage**:
- **Test 1**: `speed = 130` → goes through the `if` block, evaluates to **false**.
- **Test 2**: `speed = 110` → goes through the `else` block, evaluates to **true**.

**Tools**:  
- **gcov** or **lcov** will report branch coverage to show that both branches are tested.

---

### 3️⃣ **Path Coverage**

**What It Means**:  
This type ensures that **all possible paths** through the code are exercised. This can become complex with multiple decision points (since it requires testing combinations of branches).

**How to Achieve It**:
- Identify all possible **paths** through the code, including combinations of decision branches.
- Create test cases to cover **each unique combination of decisions** (paths).

**Example**:

```cpp
bool shouldTurnOnLights(int timeOfDay, bool vehicleMoving) {
    if (timeOfDay > 18) {
        if (vehicleMoving) {
            return true;
        } else {
            return false;
        }
    }
    return false;
}
```

Paths:
- Path 1: `timeOfDay > 18` and `vehicleMoving = true`
- Path 2: `timeOfDay > 18` and `vehicleMoving = false`
- Path 3: `timeOfDay <= 18`

To cover **path coverage**:
- **Test 1**: `timeOfDay = 19, vehicleMoving = true` → Path 1.
- **Test 2**: `timeOfDay = 19, vehicleMoving = false` → Path 2.
- **Test 3**: `timeOfDay = 15, vehicleMoving = false` → Path 3.

**Tools**:  
- **gcov** or **lcov** will help track which paths are covered.

---

### 4️⃣ **Condition Coverage**

**What It Means**:  
This ensures that each **atomic condition** (in an `if` expression) is evaluated to both **true and false** at least once, regardless of the overall decision result.

**How to Achieve It**:
- Ensure that each **condition** in a compound decision (`&&`, `||`) is tested for both **true and false**.

**Example**:

```cpp
bool isEmergencyStopNeeded(int speed, bool brakePressed) {
    if (speed > 120 && brakePressed) {
        return true;
    }
    return false;
}
```

**Test Requirements**:
- Condition 1 (`speed > 120`) → tested for both **true** and **false**
- Condition 2 (`brakePressed`) → tested for both **true** and **false**

**Test Cases**:
- **Test 1**: `speed = 130, brakePressed = true` → tests condition 1 and 2 as **true**.
- **Test 2**: `speed = 80, brakePressed = true` → tests condition 1 as **false**, condition 2 as **true**.
- **Test 3**: `speed = 130, brakePressed = false` → tests condition 1 as **true**, condition 2 as **false**.

**Tools**:  
- **gcov**, **lcov** will also track condition coverage.

---

### 5️⃣ **Modified Condition/Decision Coverage (MC/DC)**

**What It Means**:  
MC/DC is a stricter form of coverage than **Condition** and **Branch Coverage**. It ensures that:
- Each condition **evaluates to both true and false**.
- Each condition's **independent effect** on the overall decision is validated (i.e., altering one condition changes the outcome).

**How to Achieve It**:
- Design tests to toggle one condition at a time while keeping others constant to show that each condition independently affects the decision.

**Example**:

```cpp
bool shouldDisableAutopilot(int speed, bool driverAlert) {
    if (speed > 120 && driverAlert) {
        return true;
    }
    return false;
}
```

Here, we need to show that:
- `speed > 120` alone changes the result.
- `driverAlert` alone changes the result.

**Test Cases**:
- **Test 1**: `speed = 130, driverAlert = true` → both true → decision **true**
- **Test 2**: `speed = 130, driverAlert = false` → changes **driverAlert** → decision **false**
- **Test 3**: `speed = 80, driverAlert = true` → changes **speed** → decision **false**

**Tools**:  
- **gcov** and **lcov** can help generate MC/DC reports when testing individual conditions.

---

### How to Achieve GTest Coverage:

To use **Google Test** effectively for these types of coverage, you can integrate **code coverage tools** into your build system:

1. **Install Coverage Tools**:
   - **gcov** (GNU tool for coverage analysis)
   - **lcov** (GUI frontend for gcov)
   - **Bullseye**, **VectorCAST**, or similar tools

2. **Compile with Coverage Flags**:
   - When building the test binary, use the following GCC flags to enable coverage:
     ```bash
     g++ -fprofile-arcs -ftest-coverage -o my_test_binary my_test.cpp
     ```

3. **Run Tests**:
   - Execute your GTest tests as usual. The coverage tools will record which parts of the code are exercised.

4. **Generate Coverage Reports**:
   - Use **lcov** or **gcov** to generate coverage reports:
     ```bash
     lcov --capture --directory . --output-file coverage.info
     genhtml coverage.info --output-directory out
     ```

5. **Visualize**:
   - View the HTML reports that show line coverage, branch coverage, and other metrics.

---

### **Google Test (GTest) Interview Questions and Answers**

---

**1. What is Google Test?**  
Google Test is a unit testing framework for C++ developed by Google to test individual units of code.

**2. Why is GTest used in automotive software testing?**  
It validates logic modules like diagnostics, lighting control, etc., ensuring reliability and compliance with safety standards.

**3. What is a test fixture in GTest?**  
A test fixture is a class containing setup/teardown routines for multiple test cases that share common objects or configurations.

**4. How do you write a simple test in GTest?**  
```cpp
TEST(SampleTest, AdditionCheck) {
  EXPECT_EQ(2 + 2, 4);
}
```

**5. What is the difference between `EXPECT_` and `ASSERT_`?**  
`EXPECT_` continues after failure; `ASSERT_` stops the test at the failure point.

**6. Can GTest be used in embedded systems?**  
Yes, especially for logic that runs on-host before integration on-target.

**7. What is the role of `main()` in GTest?**  
It's required to initialize and run all test cases:
```cpp
int main(int argc, char **argv) {
  ::testing::InitGoogleTest(&argc, argv);
  return RUN_ALL_TESTS();
}
```

**8. How do you group tests logically?**  
By using test fixtures or naming conventions in `TEST_F()` or `TEST_P()`.

**9. What’s `TEST_F()` used for?**  
It defines a test using a shared fixture class (i.e., common test setup/teardown logic).

**10. What is `TEST_P()` used for?**  
It’s used for parameterized tests to run the same logic with multiple input values.

**11. What is Google Mock?**  
A companion library for GTest to create mock objects and test interactions.

**12. How do you mock a method?**  
By creating a class using `MOCK_METHOD()` macros.

**13. Can you integrate GTest with CI tools like Jenkins or GitHub Actions?**  
Yes, via command-line runners and test result parsers (e.g., XML).

**14. How do you skip a test temporarily?**  
Prefix the test name with `DISABLED_`.

**15. What is the benefit of using GTest in Test-Driven Development (TDD)?**  
It enforces writing testable, modular, and bug-free code from the start.

**16. Can you generate reports from GTest?**  
Yes, using `--gtest_output=xml:<file.xml>`.

**17. How do you pass command-line arguments to tests?**  
Use `InitGoogleTest()` to parse them.

**18. What’s the purpose of `SetUp()` and `TearDown()`?**  
They define actions before and after each test in a fixture.

**19. Can GTest be used for integration testing?**  
It’s mostly for unit testing but can be extended for lightweight integration.

**20. What’s the default test result format?**  
Console-based output with pass/fail logs.

**21. How do you run only a specific test case?**  
Use `--gtest_filter=TestSuiteName.TestName`.

**22. How do you test exception handling in GTest?**  
Using `EXPECT_THROW()`, `EXPECT_NO_THROW()`, etc.

**23. What is `ASSERT_THROW()` used for?**  
To assert that a statement throws an expected exception and aborts if not.

**24. Can you use GTest with CMake?**  
Yes, it integrates seamlessly with `FetchContent` or `add_subdirectory()`.

**25. Can you write custom matchers?**  
Yes, using `MATCHER()` or by extending matcher classes.

**26. What is `EXPECT_NEAR()` used for?**  
To compare floating point values with tolerance.

**27. How do you test time-sensitive functions?**  
By mocking time or using time thresholds with `EXPECT_*` statements.

**28. What is `SUCCEED()` macro?**  
Used to mark a test as passed explicitly, helpful in complex logic.

**29. Can you create reusable assertions?**  
Yes, by wrapping checks in helper functions/macros.

**30. What is the lifecycle of a test fixture?**  
`SetUp()` → test body → `TearDown()`.

**31. How do you test private members?**  
By declaring tests as `friend class` or exposing them via interfaces.

**32. How do you avoid code duplication in test setup?**  
By using fixtures and helper methods.

**33. How do you parameterize tests?**  
Using `INSTANTIATE_TEST_SUITE_P()` and `TEST_P()`.

**34. Can GTest tests be run in parallel?**  
Yes, but care must be taken with shared resources.

**35. How is GTest useful in code coverage analysis?**  
It helps generate coverage reports when combined with tools like gcov or lcov.

**36. Is Google Test platform-dependent?**  
No, it’s cross-platform (Windows, Linux, macOS).

**37. Can GTest test multithreaded code?**  
Yes, though synchronization must be handled manually.

**38. How do you suppress output in GTest?**  
By redirecting stdout/stderr or using `--gtest_brief=1`.

**39. What is `OnTestStart()` hook used for?**  
To execute custom logic when a test begins (via event listeners).

**40. Can you nest test cases in GTest?**  
No, but you can organize using naming conventions and suites.

**41. What is `--gtest_repeat`?**  
A flag to repeat tests multiple times for stress testing.

**42. What is `--gtest_shuffle`?**  
It runs tests in random order to catch inter-test dependencies.

**43. What is a flaky test?**  
A test that fails intermittently. GTest helps isolate these.

**44. How do you mock global functions?**  
Use wrapper classes/interfaces and inject them for mocking.

**45. How do you test code that depends on hardware?**  
By mocking hardware interfaces and using simulation environments.

**46. Can you write tests for legacy code using GTest?**  
Yes, by isolating functionality or wrapping legacy APIs.

**47. What is `EXPECT_STRCASEEQ()`?**  
It checks if two C strings are equal, case-insensitive.

**48. How do you integrate GTest with Qt or ROS?**  
Using appropriate test runners and CMake integration.

**49. What is a death test?**  
A test that checks if code crashes or exits abnormally (e.g., `EXPECT_DEATH()`).

**50. How does GTest improve software quality?**  
By catching bugs early, enabling refactoring, and ensuring reliability.