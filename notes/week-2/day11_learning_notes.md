# 📘 Week 2 – Python Intermediate  

## 📅 Day 11 – Python OOP Basics (Classes & Objects)  

### 🔑 Key Concepts
- **OOP (Object-Oriented Programming)** organizes code into **objects**.  
- **Class** = Blueprint (like design of a car).  
- **Object** = Instance of the class (actual car).  
- **`__init__` constructor** initializes values.  
- **`self`** refers to the current object.  
- **Methods** define the behavior of an object.  

---

### 📝 Example Programs  

#### 1. Basic Class & Object
```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print(f"Name: {self.name}, Age: {self.age}")

s1 = Student("Alice", 22)
s1.display()
