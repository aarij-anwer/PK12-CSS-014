# **Module 6: Computing Pedagogy and Code Tracing**

## **Overview**
This module explores **Computing Pedagogy** concepts and techniques, including the **notional machine, top-down refinement, worked examples, scaffolding, and vocabulary-based learning**. It also covers **Computational Thinking principles such as abstraction and modularity**, as well as **manual code tracing techniques** to reinforce students' understanding of program execution.

---

## **Learning Outcomes**
By the end of this module, educators will:
- Understand and apply key **Computing Pedagogy** techniques in the classroom.
- Become proficient in **code tracing activities** for student learning.
- Explore **Computational Thinking concepts**, including procedural and data abstractions.
- Learn how **modularity and abstraction** impact programming efficiency.

---

## **6.1 Approaches to CS Pedagogy**

### **Notional Machine**
- A **notional machine** is a **mental model** of how a computer executes code.
- It helps students **visualize** concepts like memory allocation, control flow, and function execution.
- Teaching with a notional machine enables students to **predict program behavior** before writing or running code.
- Example: In Python, when calling a function, a new **execution frame** is created, affecting variable scope and memory allocation.

### **Top-Down Refinement**
- A **problem-solving approach** that starts with a **high-level problem definition** and breaks it into smaller, manageable parts.
- Encourages students to **generalize solutions** rather than hard-coding specific cases.
- Example: Instead of writing a function that only calculates the area of a square, students should generalize it to handle any rectangle.

```python
# Specific function (not generalized)
def square_area(side):
    return side * side

# Generalized function
def rectangle_area(length, width):
    return length * width
```

### **Worked Examples**
- **Step-by-step solutions** provided before students attempt problems on their own.
- Reduces **cognitive load** by offering structured learning.
- Encourages students to **analyze and modify** existing solutions before writing their own.
- Example: Showing students a function that **sorts a list** before asking them to implement a search algorithm.

### **Apprenticeship Role of the CS Teacher**
- Teachers act as **mentors**, guiding students through **real-world problem-solving**.
- Live coding sessions allow educators to **model thought processes**, showcasing debugging and iterative problem-solving.
- Encourages students to **ask questions and collaborate** rather than just following instructions.

### **Vocabulary – Reading and Explaining Code**
- Emphasizes the importance of **code comprehension** before writing new code.
- Strategies include:
  - **Code walkthroughs** where students explain a program line-by-line.
  - **Predicting output** before running a program.
  - **Identifying errors** before execution.
- Example Activity: Present students with a Python snippet and ask, “What will this print?”

```python
x = "hello"
y = x.upper()
print(x, y)
```

(Expected Output: `hello HELLO` – demonstrates string immutability)

### **Block-Based and Text-Based Languages**
- **Block-based languages (Scratch, Blockly)** are great for beginners, reducing syntax-related errors.
- **Text-based languages (Python, Java)** require more precision but offer greater flexibility and scalability.
- Transitioning from block-based to text-based coding should be **scaffolded** using small, incremental changes.

### **Scaffolding in CS**
- **Scaffolding** is the practice of **providing structured support** that is gradually removed as students become more proficient.
- Examples of scaffolding techniques:
  - Providing **starter code** rather than making students start from scratch.
  - Using **guided coding activities** before moving to open-ended assignments.
  - Encouraging **pair programming** to allow students to learn from peers.

---

## **6.2 Computational Thinking - Abstraction and Modularity**

### **Procedural Abstractions**
- **Functions and methods** allow for **code reuse and modularity**.
- Example:
  - **Without abstraction:** Writing the same logic multiple times.
  - **With abstraction:** Encapsulating logic in a function for reuse.

```python
# Without procedural abstraction
def convert_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9

def convert_to_kelvin(fahrenheit):
    return convert_to_celsius(fahrenheit) + 273.15
```

- Encouraging students to write **highly cohesive functions** with **minimal coupling** improves code maintainability.
- Novice programmers often write **long, monolithic functions**—guiding them toward **modular design** is essential.

### **Data Abstractions**
- **Variables, lists, dictionaries, and sets** provide different levels of abstraction.
- Example:
  - **Lists** are ordered and indexable but slow for lookups.
  - **Dictionaries (hashmaps)** allow for **faster lookups** but do not maintain order.

```python
# Using a list
students = ["Alice", "Bob", "Charlie"]
print("Alice" in students)  # O(n) lookup time

# Using a dictionary (hashmap)
students_dict = {"Alice": True, "Bob": True, "Charlie": True}
print("Alice" in students_dict)  # O(1) lookup time
```

- **In Grade 12**, students should be encouraged to explore **efficiency trade-offs** between different data structures.

### **Modularity in CS Education**
- The **ICD2O Grade 10 curriculum** explicitly includes **modular programming principles**.
- In **Grades 11 and 12**, students should be encouraged to:
  - Optimize **method cohesion** (each method does one thing).
  - Reduce **method coupling** (methods should not rely heavily on each other).
  - Consider the **efficiency of data structures** in program design.

---

## **6.3 Code Tracing**

### **Why is Code Tracing Important?**
- Reinforces **understanding of execution flow**.
- Helps identify **logical errors** before running code.
- Strengthens **mental modeling of program behavior**.

### **Steps for Manual Code Tracing**
1. **Identify variables** in the code.
2. **Create a table** with columns for variables and output.
3. **Step through the code**, updating variable values and noting output.
4. **Predict the final output** before running the program.

### **Example Code Tracing Activity**
```python
x = 3
y = 1
for i in range(1, 4):
    if (x * i) > 5:
        y = y + x
        x = x - 1
print(y)
print(y - x)
```

| Step | x | y | i | Output |
|------|---|---|---|--------|
| 1    | 3 | 1 | - | -      |
| 2    | 3 | 1 | 1 | -      |
| 3    | 3 | 1 | 2 | -      |
| 4    | 2 | 4 | 2 | -      |
| 5    | 2 | 4 | 3 | -      |
| 6    | 1 | 6 | 3 | -      |
| 7    | 1 | 6 | - | 6      |
| 8    | 1 | 6 | - | 5      |

---

## **Conclusion**
This module emphasizes **pedagogical techniques** to enhance CS instruction, particularly through **notional machines, abstraction, modularity, and code tracing**. Educators should integrate **scaffolding, worked examples, and manual tracing exercises** to deepen student comprehension and problem-solving skills.
