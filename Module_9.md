# **Module 9: Object-Oriented Programming in Grade 12 Computer Science**

## **Overview**
This module focuses on **Object-Oriented Programming (OOP)** in the Grade 12 Computer Science course. It explores the differences between **procedural and object-oriented paradigms**, the **key principles of OOP**, and provides guidance on designing and implementing an **OO program**. The module also discusses the transition from **Grade 11 procedural programming to Grade 12 modular and object-oriented development**.

---

## **Learning Outcomes**
By completing this module, educators will:
- Understand the **differences between procedural and object-oriented (OO) programming**.
- Learn the **key OOP principles**, including **inheritance, encapsulation, abstraction, and polymorphism**.
- Develop an **OO software design and implementation approach**.
- Explore **best practices for modular programming** and **collaborative software development** in Grade 12.

---

## **9.1 Grade 12 Computer Studies Course Overview**

### **Transition from Procedural to Object-Oriented Programming**
- The **Grade 11 Computer Science course (ICS3U)** primarily focuses on **procedural programming**.
- In **Grade 12 (ICS4U)**, students transition to **Object-Oriented Analysis, Design, and Programming**.
- Educators can choose to **continue using the same programming language** from Grade 11 (e.g., Python, Java) or transition to a **pure OO language** such as **Ruby**.
- Modern versions of **Python and Java** include **functional programming features**, making them **hybrid languages** with **procedural, OO, and functional elements**.

### **Role-Playing Approach for Teaching OOP**
- **Collaborative exploration** of OOP concepts is key.
- A **role-playing method** can be effective in identifying **classes (nouns)** and **methods (verbs)** through real-world modeling.
- Example: In a **student management system**, students might define:
  - **Classes:** `Student`, `Teacher`, `Course`
  - **Methods:** `enroll()`, `gradeAssignment()`, `addCourse()`
- This interactive approach helps **students understand interactions between objects** before coding.

### **Collaboration in Software Development**
- The **Grade 12 curriculum emphasizes collaborative software development**.
- Encouraging **modular design** and **team-based coding projects** prepares students for real-world **software engineering practices**.

---

## **9.2 Object-Oriented Paradigm**

### **Key Concepts of Object-Oriented Programming**

| **Concept** | **Definition** | **Example** |
|------------|--------------|------------|
| **Encapsulation** | Restricting direct access to object data and controlling access through methods. | Private attributes with getter/setter methods. |
| **Inheritance** | Creating a new class that **inherits** attributes and methods from another class. | `class Car(Vehicle):` (Car extends Vehicle) |
| **Polymorphism** | Allowing different classes to use the **same interface** but with different implementations. | Overriding methods in a subclass. |
| **Abstraction** | Hiding complex implementation details and exposing only relevant features. | Abstract base classes in Python or Java interfaces. |


### **Procedural vs. Object-Oriented Programming**
- **Procedural Programming:**
  - Code is organized into **functions**.
  - Focus is on **step-by-step execution**.
  - Example (Python):
    ```python
    def calculate_area(length, width):
        return length * width
    print(calculate_area(5, 10))
    ```
- **Object-Oriented Programming:**
  - Code is organized into **classes and objects**.
  - Focus is on **data and behavior (methods)**.
  - Example (Python):
    ```python
    class Rectangle:
        def __init__(self, length, width):
            self.length = length
            self.width = width
        def area(self):
            return self.length * self.width
    rect = Rectangle(5, 10)
    print(rect.area())
    ```

### **Object-Oriented Analysis, Design, and Implementation**
- **Object-Oriented Analysis (OOA):** Identifying **key classes and relationships** in the problem domain.
- **Object-Oriented Design (OOD):** Structuring classes and defining **interactions between objects**.
- **Object-Oriented Implementation (OOP):** Writing code to **bring the design to life**.

### **Grade 12 Curriculum Expectations Related to OOP**
The **ICS4U curriculum** includes the following key OOP-related expectations:
- **Modular Programming:**
  - **A2.1:** Create a **modular program divided into multiple files**.
  - **A2.2:** Use **reusable code** and adhere to modular design principles.
- **Code Maintenance:**
  - **A4:** Use **proper coding standards** for maintainable software.
- **Applying OOP Concepts:**
  - **C1.1:** Break down a problem into **classes**.
  - **C1.2:** Apply **data encapsulation** principles.
  - **C1.3:** Use **functional decomposition** in designing subprograms.
  - **C1.4:** Apply **code reusability** principles.

### **Choosing a Programming Language for OOP**
- **Pure OOP Languages:** Ruby, Smalltalk.
- **Hybrid OOP/Procedural Languages:** Python, Java, C++.
- **Declarative Programming Languages:** SQL (focuses on queries, not algorithm implementation).

Instructors should help students **evaluate the strengths of different paradigms** and **choose the right tool for the task**.

---

## **Implementation Strategies for Teaching OOP**

### **1. Hands-On Coding Assignments**
- Students should build **real-world OO projects**, such as:
  - **Banking System** (accounts, transactions, customers).
  - **Inventory Management** (products, categories, suppliers).
  - **School Management System** (students, teachers, courses).

### **2. Class Diagrams & UML Modeling**
- Using **Unified Modeling Language (UML)** helps students **visualize relationships between classes** before coding.
- Example: **Class Diagram for a Library System**
  ```
  +------------------+
  |     Book        |
  +------------------+
  | title           |
  | author         |
  | ISBN          |
  +------------------+
  | borrow()       |
  | return()       |
  +------------------+
  ```

### **3. Collaborative Software Development**
- Use **GitHub for version control** to simulate **real-world team collaboration**.
- Implement **pair programming** and **code reviews** to improve student learning.

---

## **Conclusion**
This module introduces students to **Object-Oriented Programming (OOP)** as they transition from procedural programming. The focus is on understanding **core OOP principles (encapsulation, inheritance, polymorphism, abstraction)** and applying them through **modular software design and collaborative development**. 

By integrating **role-playing exercises, UML modeling, and real-world coding projects**, educators can effectively teach **object-oriented concepts** and **prepare students for industry-standard programming practices**.
