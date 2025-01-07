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
N = 5 Arr = [62, 8, 34, 5, 332]

- **Output**:
0-4 6-7 9-33 35-61 63-331

- **Explanation**:  
Elements in the ranges `0-4`, `6-7`, `9-33`, `35-61`, and `63-331` are not present in the array.

**Key Points**  
- Sort the array to identify gaps.  
- Output ranges in a concise format (e.g., `start-end`).

---

## 4. Generator – Filter Prime Numbers

**Question**  
Write a **generator** function in Python that yields only the prime numbers from a given list of integers.

**Example**  
- **Input**: `[2, 3, 4, 16, 17, 19, 21]`  
- **Output** (yielded values): `2, 3, 17, 19`

**Key Points**  
- Demonstrate understanding of Python generators (`yield`).  
- Implement an efficient prime-checking routine.  
- Possibly discuss time complexity.

---

## 5. Minimum Number of Platforms (Train Arrival & Departure)

**Question**  
You are given two arrays representing arrival and departure times of trains at a station:
arr = [100, 130, 215, 245, 315, 330, 400]
dep = [150, 415, 240, 355, 405, 350, 450]

Find the minimum number of platforms required so that no train has to wait, given the arrival and departure times.

Key Points

A common approach is to sort both arrival and departure times.
Traverse them to determine the overlap (when a platform is still occupied).
Time complexity is typically O(n log n).

---

## 6. Explain Decorator and Generator in Python

### Open-Ended Discussion

#### Decorator
- **Definition & Syntax**: A decorator is a function that takes another function as an argument, extends its behavior without explicitly modifying it, and returns a new function. The syntax commonly uses the `@decorator_name` approach.
- **Usage**: Common in logging, authentication, caching, rate-limiting, etc.
- **How It Works**: Decorators wrap another function to add functionality before or after the wrapped function runs (or even replace it), without changing the original code of that function.

#### Generator
- **Difference from a Normal Function**: A generator uses `yield` instead of `return` to produce a sequence of values over time.
- **`yield` vs. `return`**: `yield` pauses the function, saving its state, and resumes on the next call, whereas `return` exits the function immediately.
- **Memory Benefits**: Generators produce items lazily, generating values on the fly rather than creating a complete data structure in memory.

---

## 7. Sorting Algorithms: Bubble Sort vs. Insertion Sort

### Open-Ended Discussion

- **Bubble Sort**  
  - **Process**: Repeatedly compares adjacent elements and swaps them if they are in the wrong order.
  - **Time Complexity**: O(n²) in the average and worst case.
  - **Swaps**: Often many swaps, making it less efficient on large or nearly-sorted lists.

- **Insertion Sort**  
  - **Process**: Builds the sorted array one item at a time by comparing the current item to its predecessors.
  - **Time Complexity**: O(n²) in the average and worst case, but can be more efficient if the list is partially sorted.
  - **Typical Use**: Small datasets, or when data is nearly sorted.

**Key Points**  
- Both have the same average/worst-case time complexity of O(n²).  
- Insertion Sort can be more efficient for small or nearly-sorted datasets.  
- Bubble Sort may do more swaps, especially if the list is in reverse order.

---

## 8. Knapsack Problem (0/1)

### Question
Given a set of items, each with a weight and a value, determine the **number of each item** to include in a collection so that the total weight is **≤ a given limit** and the total value is **as large as possible**.

**Key Points**  
- **Classic Dynamic Programming** problem.  
- Time complexity often cited as O(nW), where W is the capacity/weight limit.  
- Discuss possible space optimizations (rolling arrays, etc.).  
- Variation: **Unbounded Knapsack**, where you can include multiple units of the same item.

---

## 9. Best Time to Buy and Sell Stock

### Question
You are given an array of prices, where `prices[i]` is the price of a given stock on day `i`. Design an algorithm to **maximize** your profit by choosing **one day to buy** and a **different day to sell**.

**Key Points**  
- Keep track of the **minimum price** seen so far as you iterate.  
- Calculate potential profit at each step.  
- A single pass solution runs in O(n) time and O(1) space.

---

## 10. Check for Anagrams

### Question
Given two strings, determine if they are anagrams of each other (i.e., contain the same characters in the same frequencies).

**Key Points**  
- **Sorting** approach: Sort both strings and compare; O(n log n) time.  
- **Hash/Dictionary** approach: Count character frequencies in both strings and compare; O(n) time.  
- Consider edge cases (spaces, punctuation, case-sensitivity, unicode).

---

## Additional / Optional Coding Questions

1. **Longest Substring Without Repeating Characters**  
   - Typically solved with a sliding window approach.  
   - Time complexity: O(n).

2. **Merge Intervals**  
   - Given a collection of intervals, merge all overlapping intervals.  
   - Sort by start time, then check overlaps as you iterate.

3. **Top K Frequent Elements**  
   - Could use a max-heap or bucket sort approach.  
   - Time complexity depends on the data structure chosen.

4. **Longest Common Subsequence (LCS)**  
   - Classic dynamic programming problem for strings or sequences.  
   - Time complexity: O(n × m) for strings of lengths n and m.

---

## Tips & Guidance

1. **Complexity Analysis**  
   - Always discuss your algorithm’s time and space complexity.  
2. **Edge Cases**  
   - Consider minimal inputs, large inputs, empty strings/arrays, special characters, etc.  
3. **Coding Style**  
   - Emphasize readability, clear naming conventions, and adhere to Python best practices (PEP 8).  
4. **Testing**  
   - Provide sample inputs/outputs.  
   - Write quick test cases or discuss how you’d unit test your solution.

---
```
list_1=[4,4,3,2,4,2,4,1,5,6,4,2,1,4,8]

def check_duplicate(input):
  output={}
  final_output=[]

  for i, val in enumerate(input):
      if val in output.keys():
        output[val]=output[val]+1
      else:
        output[val]=1
  
  final_output = {x:j for x,j in output.items() if j != 1}
  
  return final_output
        
print(check_duplicate(list_1))


```
 Examples => Expected Output
 [7, 1]  =>  [1, 7]
 [5, 8, 6, 3, 4]  =>  [3, 8, 6, 5, 4]
 [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]  =>  [1, 8, 3, 6, 5, 4, 7, 2, 9, 0]
 [5, 3, 2, 8, 1, 4] => [1, 3, 2, 8, 5, 4]
 [5, 3, 1, 8, 0] => [1, 3, 5, 8, 0]

def sort_even_number(input):
  final_sorted_list=[]
  odd_dict_list = {i:val for i, val in enumerate(input) if i%2!=0}
  sorted_list=odd_dict_list.sorted()
  
  for i, val in input:
    if val%2 !=0:
      i

```

def custom_check(func):
    def wrapper():
      return func().upper()
    return wrapper

@custom_check
def test():
    return "hello"
    
print(test())


student_data = {
    'Rohan': {"Course": {"Math":50, "Physics":70, "Chemistry":80}},
    'Mohan': {"Course": {"Math":67, "Physics":87, "Chemistry":38}},
    'Pramod': {"Course": {"Math":63, "Physics":67, "Chemistry":95}}
}


def calculate_highest_mark(input):
    highest_marks=0
    for student, details in student_data.items():
          highest_marks = sum(details['Course'].items())

    return {
        "highest_marks": highest_marks,
    }
    


--Customers: customer_id    first_name  last_name   age country created_at
--Orders: order_id  item    amount  customer_id, is_canceled, created_at
--Shippings: shipping_id    status  customer, is_active, created_at

Find the  Total number of customer in each country

select country, count(*) from customer group_by country;


Customer.objects


