# Coding & Algorithmic Interview Questions

Below is a curated set of coding challenges and topics suitable for a candidate with **6.5+ years of experience**. Each question has a brief description of what is expected. You can mix and match these based on the candidate's expertise and the time available for the interview.

---

## 1. Validate Brackets

**Question**  
Given a string containing only the characters `'('`, `')'`, `'{'`, `'}'`, `'['`, and `]'`, determine if the input string is valid.

**Requirements for validity**  
1. Open brackets must be closed by the same type of brackets.  
2. Open brackets must be closed in the correct order.

**Sample Test Cases**  
- Input: `()[]{}`
  - Output: `True`
- Input: `(]`
  - Output: `False`

**Key Points**  
- Typically solved using a stack.  
- Return a boolean indicating whether the string is valid.

---

## 2. SQL – Average Salary by Department

**Question**  
Consider a database table named **employees** with columns:  
- `employee_id`  
- `employee_name`  
- `department_id`  
- `salary`

There is another table named **departments** with columns:  
- `department_id`  
- `department_name`

Write a SQL query to find the **average salary for each department**. Include the **department name** in the result set.

**Key Points**  
- Use `JOIN` to connect the `employees` table with `departments`.  
- Aggregate function `AVG()`.  
- `GROUP BY` department.

**Example Output**  
- Columns returned might be: `department_name`, `average_salary`

---

## 3. Missing Elements in a Range

**Question**  
Given an array `Arr[]` of `N` positive integers, find the **missing elements** (if any) in the range `0` to `max(Arr)`.

**Example**  
- **Input**:

