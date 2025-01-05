# React Interview-Questions
# Full-Stack Interview Question Bank

This question bank covers **JavaScript** and **React** topics. You can later add **Python** and **Django** questions to complete your full-stack interview preparation.

---

## JavaScript Questions

### Basic JavaScript Questions

1. **What are closures?**  
2. **What is hoisting?**  
3. **What is a pure function in JavaScript?**  
4. **Difference between `let`, `const`, and `var`.**  
5. **What is event bubbling?**  
6. **What is event capturing?**  
7. **What is the event loop?**  
8. **What are some ES6 features?**  
9. **Arrow function vs. normal function.**  
10. **Synchronous vs. asynchronous functions.**  
11. **What are Promises in JavaScript?**  
12. **Console-based questions:**
    - `console.log(2 + true)`
    - `console.log(NaN == NaN)`
    - `console.log(NaN === NaN)`
    - `console.log('7' - - '3')`
    - `console.log('7' + + '3')`
    - `console.log([] == [])`
    - `console.log([] === [])`
    - `console.log(null == undefined)`

### Additional JavaScript Questions

1. **What is the difference between `==` and `===`?**  
2. **Explain the `this` keyword in JavaScript.**  
3. **What are prototypes, and how does prototypal inheritance work in JavaScript?**  
4. **What are higher-order functions in JavaScript?**  
5. **Difference between `.call()`, `.apply()`, and `.bind()`.**  
6. **Explain the concept of “Currying” in JavaScript.**  
7. **Common array methods (e.g., `map`, `filter`, `reduce`)—how do they work and when to use them?**  
8. **How do you handle errors in JavaScript?**  
9. **Difference between `document.getElementById` and `document.querySelector`.**  
10. **What is the difference between a shallow copy and a deep copy in JavaScript?**  
11. **Explain `async/await` in detail.**  
12. **What is the concept of the call stack, and how do stack overflows happen in JavaScript?**  
13. **Explain event delegation.**  
14. **Difference between microtasks (e.g., `Promise.then()`) and macrotasks (e.g., `setTimeout()`).**  

---

## React Questions

1. **What is the Virtual DOM, and how does React use it?**  
2. **Explain the lifecycle methods in class components** (e.g., `componentDidMount`, `componentDidUpdate`, `componentWillUnmount`).  
3. **What are React Hooks? Name a few commonly used ones.** (`useState`, `useEffect`, `useContext`, `useReducer`, etc.)  
4. **Explain `useEffect` in depth** (dependencies array, cleanup functions, etc.).  
5. **What are Controlled vs. Uncontrolled components in React?**  
6. **What is the Context API in React, and when would you use it?**  
7. **How does React handle rendering optimization?** (e.g., `React.memo`, `useCallback`, `useMemo`).  
8. **What are keys in React, and why are they important?**  
9. **How would you optimize a React application’s performance?** (code splitting, lazy loading, memoization, virtualization, etc.)  
10. **Difference between Class Components and Functional Components in React.**  
11. **Explain error boundaries in React** (`componentDidCatch`, `getDerivedStateFromError`).  
12. **How do you handle forms in React?** (controlled components, libraries like Formik/React Hook Form).  
13. **How does server-side rendering (SSR) work with React?** (e.g., Next.js)  
14. **What are Higher-Order Components (HOCs) in React?**  

---

## Sample Follow-Up / Scenario-Based Questions

1. **JavaScript**  
   - Given a code snippet with multiple nested callbacks, how would you refactor it to use Promises or `async/await`?  
   - How would you debug or optimize a large array manipulation task?

2. **React**  
   - You have a parent component rendering 100 children, each with complex state. How can you optimize re-renders?  
   - How would you migrate a Class Component with lifecycle logic to a Functional Component using Hooks?

3. **Integration (React + Python/Django)**  
   - Explain how you would structure a full-stack app with a React frontend and a Django backend.  
   - Where would you handle data fetching, how do you manage state, and how do you secure API endpoints?

---

# Python & Related Topics – Interview Question Bank

Below is a curated list of topics and example questions based on the items seen in the provided image, along with some additional questions to deepen your interview preparation. Feel free to add or remove questions based on the role requirements and time constraints.

---

## 1. Time Complexity

1. **Explain time complexity in the context of Python.**  
   - What is Big-O notation?  
   - How do you analyze the time complexity of a Python function or algorithm?

2. **Compare the time complexities of different collection operations.**  
   - Inserting, deleting, or accessing elements in lists, dictionaries, and sets.

3. **How do you optimize code for better time complexity?**  
   - Provide an example of an algorithm that went from O(n²) to O(n).

---

## 2. Memory Management in Python

1. **How does Python manage memory for objects?**  
   - Reference counting and garbage collection (generational GC).

2. **What is a memory leak in Python, and how can it occur?**  
   - Circular references, improper global usage, etc.

3. **Explain the difference between stack and heap memory.**  
   - Where do variables, objects, and function calls reside?

4. **How would you profile memory usage in a Python application?**  
   - Tools such as `memory_profiler`, `objgraph`, etc.

---

## 3. The Global Interpreter Lock (GIL)

1. **What is the GIL in Python, and why does it exist?**  
   - Impact on multi-threading and concurrency.

2. **How does the GIL affect CPU-bound vs. I/O-bound programs?**  
   - When is threading advantageous, or when to consider multiprocessing?

3. **Explain ways to bypass or mitigate GIL limitations.**  
   - Using `multiprocessing`, `asyncio`, or external libraries (NumPy, etc.).

---

## 4. Object-Oriented Programming (OOP) in Python

1. **Explain the basic OOP principles (Inheritance, Encapsulation, Polymorphism, Abstraction).**  
2. **Describe how you’d implement polymorphism in Python with an example.**  
3. **What is multiple inheritance, and how does the MRO (Method Resolution Order) work in Python?**  
4. **Explain the difference between class methods, instance methods, and static methods.**

---

## 5. Data Types in Python

1. **List some built-in data types in Python.**  
   - `int`, `float`, `bool`, `str`, `list`, `tuple`, `dict`, `set`, etc.

2. **Immutable vs. Mutable data types.**  
   - How do they differ, and why does it matter?

3. **What are the differences between a list and a tuple?**  
   - Performance, mutability, use cases.

4. **Explain how Python handles large integers.**

---

## 6. `__name__ == "__main__"` Idiom

1. **What does `if __name__ == "__main__":` mean in Python?**  
   - Why is it used, and where do you typically see it?

2. **Explain the difference between running a Python script vs. importing it as a module.**

---

## 7. Generators in Python

1. **What are generators, and how do they differ from regular functions?**  
   - `yield` keyword usage.

2. **Advantages of using generators.**  
   - Memory efficiency (lazy evaluation), clarity in code.

3. **Explain how to create a generator expression vs. a list comprehension.**

---

## 8. Decorators in Python

1. **What is a decorator, and how is it defined in Python?**  
2. **Explain the syntax and typical use cases for decorators.**  
   - Logging, authorization, caching, etc.

3. **What is the difference between a function decorator and a class decorator?**

---

## 9. Lazy Loading

1. **What does lazy loading mean in the context of Python (and web frameworks)?**  
   - Delaying object loading until it’s needed.

2. **Explain scenarios where lazy loading is beneficial.**  
   - Large data sets, ORM relationships in Django, performance considerations.

---

## 10. Django vs. Flask

1. **Compare Django and Flask in terms of structure, scalability, and community support.**  
2. **When would you choose Django over Flask, and vice versa?**  
3. **Name some features or built-in functionalities Django provides out of the box.**

---

## 11. List Methods in Python

1. **What are common list methods in Python, and how do they work?**  
   - `append`, `extend`, `insert`, `pop`, `remove`, `sort`, `reverse`, `index`, etc.

2. **Explain the difference between `append` and `extend`.**  
3. **How would you slice a list, and why might that be useful?**

---

## 12. `try-except` (Exception Handling)

1. **How do you handle exceptions in Python using `try-except` blocks?**  
2. **Explain `try-except-else-finally`.**  
3. **How can you create custom exceptions in Python, and when is it appropriate?**

---

## 13. File Handling

1. **How do you open and close files in Python safely?**  
   - Using the `with open(...) as f:` context manager.

2. **Reading vs. writing files.**  
   - `read()`, `readline()`, `readlines()`, `write()`, `writelines()`, etc.

3. **Binary files vs. text files.**  
   - Common use cases for each.

---

## 14. String Methods in Python

1. **Common string methods: `split`, `join`, `replace`, `strip`, etc.**  
2. **How do Python strings handle immutability?**  
3. **String formatting options:**  
   - f-strings, `.format()`, `%` formatting.

---

## 15. Date and Time in Python

1. **How to work with dates and times in Python using the `datetime` module.**  
2. **Converting between different time zones.**  
   - Libraries: `pytz`, `zoneinfo`.

3. **Parsing and formatting dates.**  
   - `strftime`, `strptime`.

---

## 16. Database Fundamentals

### ACID Properties

1. **What are ACID properties in the context of database transactions?**  
   - Atomicity, Consistency, Isolation, Durability.

2. **Explain how Python’s ORM frameworks (e.g., Django ORM) handle transactions.**

### Joins

1. **What are different types of JOINs (INNER, LEFT, RIGHT, FULL) in SQL?**  
   - When would you use each?

2. **How do you perform joins using the Django ORM (if applicable)?**

### SQL vs. NoSQL

1. **What are the differences between relational (SQL) and non-relational (NoSQL) databases?**  
2. **Which scenarios are best suited for NoSQL?**  
   - Horizontal scaling, unstructured data, etc.

3. **What are some popular NoSQL databases (MongoDB, Redis, Cassandra)?**

### Sharding

1. **What is sharding, and why is it used?**  
2. **Discuss the challenges or trade-offs with sharding in large-scale applications.**

### 1:1, 1:M, M:M Relationships

1. **Explain how these relationship types work in relational databases.**  
2. **How does Django define relationships using models (OneToOneField, ForeignKey, ManyToManyField)?**

---

## 17. Design Patterns

1. **What are design patterns, and why are they important?**  
2. **Name a few common design patterns you’ve used in Python.**  
   - Singleton, Factory, Observer, etc.

3. **How might the Factory pattern or Singleton pattern be implemented in Python?**

---

## 18. Security/Cybersecurity (SOAR, SIEM)

> **(These topics may be role-dependent, but can be useful for security-focused positions.)**

1. **What is SOAR (Security Orchestration, Automation, and Response)?**  
   - How does it integrate with existing security systems?

2. **What is SIEM (Security Information and Event Management)?**  
   - How might you incorporate logging/monitoring in a Python application?

3. **Basic security best practices in Python or web frameworks.**  
   - Input validation, sanitizing data, securing secrets, etc.

---

## 19. Coding Exercises & LeetCode-Style Questions

1. **Explain how you typically solve problems on LeetCode or other platforms.**  
   - Outline your problem-solving approach, data structures, and algorithms.

2. **Common problem patterns:**  
   - Two pointers, sliding window, BFS/DFS, dynamic programming, etc.

3. **Walkthrough example:**  
   - Given a problem to find the longest substring without repeating characters, how would you solve it?

---

## Tips & Follow-up

- **Scenario-based questions:**  
  - “How would you scale a Python application with high read/write demands?”  
  - “How do you handle large file uploads in Django or Flask?”

- **Real-world application:**  
  - Always ask, “Where have you used this?” or “How would you apply this pattern or library in a real scenario?”

- **Deep dive:**  
  - For each topic, be prepared to go one or two levels deeper (e.g., code examples, performance considerations, design trade-offs).

---

**Use this list as a starting point, and adjust the depth of questions according to the candidate’s experience level and the specific requirements of the role. Good luck with your interviews!**


