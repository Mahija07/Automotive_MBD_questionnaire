# 📚 M SCRIPTING 

### 💡 **What is M-Scripting (MATLAB Scripting)?**
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

M-scripting refers to writing code in **MATLAB using `.m` files**, which include scripts and functions. It allows for:
- Data processing
- Algorithm development
- Simulation automation
- Plotting & visualization
- Model control (e.g., running Simulink models via script)

---

### 📍 **Where is it used?**

- Controlling **Simulink** model simulations
- Automating **test cases** (MIL/SIL)
- Post-processing results (e.g., signal logs, plots)
- Writing reusable utility functions
- Performing **batch regression tests**
- Creating **configuration scripts** for automotive domains

---

### 📅 **When do we use it?**

- During **model development**
- For **automated testing pipelines**
- To **generate and document results**
- When building toolchains for **code generation, verification**

---

### ❓ **Why use M-scripts?**

- **Automation:** Run tasks, load data, execute models without GUI
- **Customization:** Build test frameworks and utilities
- **Reusability:** Define functions for common engineering operations
- **Efficiency:** Avoid repetitive manual actions

---

### ⚙️ **How do we use it?**

- Create `.m` files with code and logic
- Use control structures (`if`, `for`, `while`)
- Interface with Simulink models using `set_param`, `sim`, `get_param`
- Perform data handling using tables, matrices, cell arrays, structs
- Integrate with toolboxes or use for test automation

---

### 🌟 **Benefits**

✅ Simplifies repetitive tasks  
✅ Helps in building test frameworks  
✅ Makes simulation runs reproducible  
✅ Enables clean and structured development  
✅ Easy to integrate with CI/CD and test tools like Jenkins or JIRA  
✅ Great for logging, visualization, post-analysis  

---

### 🧩 **Basic MATLAB Scripting Commands & Their Use**

| **Command** | **Use** |
|-------------|---------|
| `clc` | Clears the Command Window |
| `clear` | Removes variables from workspace |
| `close all` | Closes all open figure windows |
| `disp(x)` | Displays value of `x` |
| `fprintf()` | Prints formatted data to screen or file |
| `load('file.mat')` | Loads variables from a `.mat` file |
| `save('file.mat')` | Saves variables to a `.mat` file |
| `plot(x, y)` | Plots x vs y |
| `title('text')` | Adds title to plot |
| `xlabel('x')`, `ylabel('y')` | Labels x and y axes |
| `legend()` | Adds legend to plot |
| `hold on` | Allows multiple plots on same axes |
| `axis([xmin xmax ymin ymax])` | Sets axis limits |
| `if`, `else`, `elseif`, `end` | Conditional statements |
| `for i = 1:N` | Looping from 1 to N |
| `while condition` | Loop while condition is true |
| `break` | Exit loop early |
| `continue` | Skip current iteration |
| `function out = name(in)` | Function definition |
| `sim('modelName')` | Runs a Simulink model |
| `set_param()` | Set block/model parameter |
| `get_param()` | Get block/model parameter |
| `exist('var', 'var')` | Check if variable exists |
| `isnan(x)` | Check if value is NaN |
| `size(x)` | Returns dimensions of array `x` |
| `length(x)` | Returns largest dimension of `x` |
| `zeros(n,m)`, `ones(n,m)` | Create n-by-m array of 0s or 1s |
| `rand(n)` | Generate n-by-n random matrix |
| `linspace(a,b,n)` | Generate `n` points between `a` and `b` |
| `mean(x)` | Compute mean of x |
| `std(x)` | Compute standard deviation |
| `max(x)`, `min(x)` | Find max/min values |
| `sum(x)`, `prod(x)` | Sum/product of array elements |
| `input('msg')` | Get input from user |
| `pause(n)` | Pause execution for n seconds |
| `try...catch` | Error handling block |
| `gca`, `gcf` | Current axes, current figure handles |
| `eval('code')` | Execute string as MATLAB code |
| `cd`, `pwd`, `ls` | Directory navigation |
| `who`, `whos` | List variables in workspace |


### **MATLAB M-Scripting Interview Q&A **

---

**1. What is an M-script in MATLAB?**  
A script written in a `.m` file that contains a sequence of MATLAB commands.

**2. How is an M-script different from a function?**  
Scripts don’t take inputs or return outputs; functions do.

**3. How do you create an M-script?**  
Create a new `.m` file and save it with your code.

**4. What command is used to run an M-script?**  
Just type the file name (without `.m`) in the command window.

**5. What is the command to run a Simulink model from a script?**  
`sim('modelName')`

**6. How do you automate test cases using scripts?**  
By looping through test inputs and calling Simulink models with `sim()`.

**7. What function is used to set parameters in a Simulink model?**  
`set_param()`

**8. What is `get_param()` used for?**  
To retrieve model, block, or signal parameters.

**9. How do you store simulation output in a script?**  
By capturing the output of `sim()` like:  
```matlab
out = sim('modelName');
```

**10. What function is used to create plots?**  
`plot(x, y)`

**11. How can you use conditions in scripts?**  
Using `if`, `elseif`, and `else`.

**12. How do you loop in MATLAB?**  
Using `for` and `while` loops.

**13. How do you suppress output in MATLAB?**  
Add a semicolon `;` at the end of the statement.

**14. What is the use of `disp()`?**  
To display text or variable values.

**15. How can you create a function inside an M-script?**  
Add a `function` block at the end of the script (in recent MATLAB versions).

**16. How do you handle errors in scripts?**  
Use `try` and `catch` blocks.

**17. What is the use of `exist()`?**  
To check if a variable or file exists.

**18. How do you load `.mat` files in scripts?**  
Using `load('filename.mat')`.

**19. What does `clear` do?**  
Clears variables from the workspace.

**20. What does `clc` do?**  
Clears the command window.

**21. How to save simulation outputs from scripts?**  
Use `save('filename.mat', 'variableName')`

**22. How do you write data to a text file?**  
Using `fopen`, `fprintf`, and `fclose`.

**23. What is the `fprintf` function for?**  
Formatted data printing to the screen or file.

**24. How do you generate test input signals in a script?**  
Use functions like `sin`, `linspace`, `rand`, or custom arrays.

**25. What are common uses of M-scripts in automotive?**  
MIL testing, batch simulations, test automation, plotting results.

**26. What does `pause` do?**  
Temporarily stops script execution.

**27. How do you call a function from a script?**  
Just type the function name and pass inputs.

**28. How do you debug an M-script?**  
Use breakpoints and the `dbstop`, `dbstep`, `dbclear` commands.

**29. How do you use global variables in scripts?**  
Use the `global` keyword.

**30. What is the difference between `length()` and `size()`?**  
`length()` returns the largest dimension, `size()` returns both.

**31. How do you vectorize operations in MATLAB?**  
Use array/matrix operations instead of loops.

**32. How do you check for NaN in a script?**  
Use `isnan()`.

**33. How do you define a cell array?**  
`C = {1, 'text', [1 2 3]};`

**34. What is the benefit of scripting for testing?**  
Automates tests, repeatability, saves time, traceability.

**35. How do you execute a script from another script?**  
Just call the filename without `.m`.

**36. How do you generate plots for multiple datasets?**  
Use `hold on` and multiple `plot()` calls.

**37. How do you add titles and labels to plots?**  
Use `title()`, `xlabel()`, `ylabel()`.

**38. What does `gca` and `gcf` stand for?**  
Current axes and current figure handles.

**39. How do you loop through signal names in a list?**  
Use a `for` loop with cell arrays.

**40. How do you compare expected vs actual values?**  
Use `assert()` or difference-based checks with tolerance.

**41. What’s the role of `simOut.logsout`?**  
Access logged signals from Simulink.

**42. How do you log signals in a script?**  
Enable logging in Simulink, access via `simOut`.

**43. Can you run a script from a button in Simulink?**  
Yes, using a callback that triggers `evalin('base', 'scriptName')`.

**44. What is `eval()` used for?**  
Executes a string as a MATLAB command.

**45. What is the use of `input()` in scripts?**  
Takes user input during script execution.

**46. What is `switch-case` used for?**  
Alternative to `if-else` for handling multiple conditions.

**47. What does `who` and `whos` show?**  
Lists all variables and their details.

**48. How do you define an inline anonymous function?**  
```matlab
f = @(x) x^2;
```

**49. What is `cellfun` or `arrayfun` used for?**  
Apply a function to each cell/array element.

**50. Why is M-scripting important in automotive MBD?**  
Helps automate modeling, testing, simulation, data processing, and reporting — making engineering efficient and traceable.