
# Cpp_Experiment_10_Call_by_Value_And_Reference

## Aim
To study and implement different ways of calling functions in C++:
- Call by Value  
- Call by Reference (using pointers)  
- Pass by Reference (using C++ references)  

---

## Objectives
- Understand how data is transferred between functions.  
- Differentiate between call by value, call by reference, and pass by reference.  
- Observe how changes inside a function affect (or do not affect) actual variables.  
- Develop clarity about memory management during function calls.  

---

## Theory
In C++, functions help in modular programming by breaking large code into smaller reusable blocks. However, the way data is passed to these functions impacts the behavior of variables.

### 🔹 Call by Value
- A **copy** of the actual parameter is passed.  
- Changes affect only the copy, not the original variable.  
- Separate memory is allocated for actual and formal parameters.  
- Example: Swapping two numbers won’t change the original values.  

### 🔹 Call by Reference (using Pointers)
- The **address (memory location)** of the variable is passed.  
- Formal parameters act as pointers to actual parameters.  
- Any modification directly updates the original variable.  
- Useful when functions need to update the caller’s data.  

### 🔹 Pass by Reference (using C++ References)
- A reference variable acts like an **alias** of another variable.  
- No copy is made; operations directly affect the original variable.  
- Syntax is simpler and safer compared to pointers.  
- Widely used in C++ for efficiency and readability.  

---

## 📊 Comparison Table

| Method            | What is Passed?  | Changes Affect Original? | Memory Used | Safety & Simplicity  |
|-------------------|------------------|---------------------------|-------------|-----------------------|
| Call by Value     | Copy of variable | No                        | More        | Very safe             |
| Call by Reference | Address          | Yes                       | Less        | Needs pointer care    |
| Pass by Reference | Reference        | Yes                       | Less        | Simple & efficient    |

---

## Program Description

We implemented **three different programs** to highlight the behavior of parameter passing.

### 1️⃣ Call by Value
- Function receives copies of actual values.  
- Inside the function, values are swapped but original variables remain unchanged.  
- Demonstrates that only local copies are affected.  

### 2️⃣ Call by Reference (using Pointers)
- Function receives addresses of variables.  
- Pointers access the original variables and perform swapping.  
- After execution, original values are permanently changed.  

### 3️⃣ Pass by Reference (using References)
- Function uses reference variables (aliases of originals).  
- Any modification is directly applied to the actual variables.  
- Cleaner syntax compared to pointers, no explicit dereferencing needed.  

---

## Overall Observation
- **Call by Value →** No effect on actual variables.  
- **Call by Reference →** Original values modified using pointers.  
- **Pass by Reference →** Original values modified using reference variables (simpler syntax).  

---

## Concepts Used
- Functions in C++  
- Function parameters and return types  
- Pointers and memory addressing  
- Reference variables in C++  
- Distinction between formal vs. actual parameters  

---

## Conclusion
This experiment clarified the differences between the three parameter passing methods:  

- **Call by Value:** Safe but doesn’t modify original variables.  
- **Call by Reference:** Directly modifies original data but requires careful pointer handling.  
- **Pass by Reference:** Achieves the same effect as pointers but with simpler, safer syntax.  

> ✅ The method of parameter passing directly determines whether modifications inside a function are reflected in the caller’s variables.
