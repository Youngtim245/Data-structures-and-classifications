# Data-structures-
# Data Structures and Their Classifications

This repository provides an overview of **Data Structures**, their **Classifications**, **Examples in C and Python**, and **Real-world Applications**.

---

## 1. What is a Data Structure?

A **Data Structure** is a way of organizing, managing, and storing data efficiently so it can be used effectively.  
They are fundamental to designing efficient algorithms and solving computational problems.

---

### 2. Classification of Data Structures

### **A. Primitive Data Structures**
These are the basic building blocks provided by programming languages.

| Type | Description | Example (C) | Example (Python) |
|------|--------------|--------------|------------------|
| Integer | Numeric type | `int x = 10;` | `x = 10` |
| Float | Decimal numbers | `float y = 10.5;` | `y = 10.5` |
| Character | Single symbol | `char c = 'A';` | `c = 'A'` |
| Boolean | Logical values | `_Bool flag = 1;` | `flag = True` |

**Applications:** Used in arithmetic operations, condition checks, and logical computations.

---

### **B. Non-Primitive Data Structures**

These are derived from primitive types. They are divided into two categories:

#### **1. Linear Data Structures**
Elements are arranged sequentially.

| Type | Description | Example Code | Common Applications |
|------|--------------|--------------|---------------------|
| **Array** | Collection of elements of same type | **C:**<br>`int arr[5] = {1,2,3,4,5};`<br>**Python:**<br>`arr = [1,2,3,4,5]` | Used in sorting algorithms, matrices, image processing |
| **Linked List** | Nodes linked via pointers | **C:**<br>```c\nstruct Node {int data; struct Node* next;};```<br>**Python:**<br>```python\nclass Node:\n    def __init__(self, data):\n        self.data = data\n        self.next = None``` | Dynamic memory use, implementing stacks/queues |
| **Stack** | LIFO (Last In First Out) | **C:**<br>`push(), pop()` using arrays or linked lists<br>**Python:**<br>`stack.append(x); stack.pop()` | Expression evaluation, undo features |
| **Queue** | FIFO (First In First Out) | **C:**<br>`enqueue(), dequeue()`<br>**Python:**<br>`from collections import deque` | Scheduling, printer queues, CPU tasks |

---

#### **2. Non-Linear Data Structures**
Elements are connected in a hierarchical or network manner.

| Type | Description | Example Code | Common Applications |
|------|--------------|--------------|---------------------|
| **Tree** | Hierarchical structure | **C:**<br>```c\nstruct Node {int data; struct Node *left, *right;};```<br>**Python:**<br>```python\nclass Node:\n    def __init__(self, data):\n        self.data = data\n        self.left = self.right = None``` | File systems, search algorithms (BST) |
| **Graph** | Set of vertices connected by edges | **Python:**<br>```python\ngraph = {'A': ['B','C'], 'B': ['A','D'], 'C':['A'], 'D':['B']}``` | Social networks, routing algorithms, maps |

---

### **C. Abstract Data Types (ADTs)**

An ADT defines operations on data without specifying implementation details.

| ADT | Implementation Example | Applications |
|-----|--------------------------|--------------|
| Stack | Implemented using arrays or linked lists | Function call stack, undo feature |
| Queue | Implemented using arrays, linked lists, or circular queues | CPU scheduling |
| List | ArrayList or LinkedList | Database records, dynamic collections |
| Map / Dictionary | Hash tables | Fast lookup tables, symbol tables |

---

## 3. Example Implementations

### **Array in Python**
```python
arr = [10, 20, 30, 40]
for x in arr:
    print(x)


