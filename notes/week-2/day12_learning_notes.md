# 📘 Week 2 – Python Intermediate  

## 📅 Day 12 – OOP Advanced (Inheritance, Polymorphism, Encapsulation)  

### 🔑 Key Concepts
- **Inheritance**: One class (child) can use properties/methods of another class (parent).  
- **Polymorphism**: Same method name behaves differently depending on the object.  
- **Encapsulation**: Restricting direct access to variables/methods (protecting data).  

---

### 📝 Example Programs  

#### 1. Single Inheritance
```python
class Animal:
    def speak(self):
        print("Animal speaks")

class Dog(Animal):
    def speak(self):
        print("🐶 Dog barks")

d = Dog()
d.speak()
class Animal:
    def move(self):
        print("Animals can move")

class Dog(Animal):
    def bark(self):
        print("Dog barks")

class Puppy(Dog):
    def weep(self):
        print("Puppy cries")

p = Puppy()
p.move()
p.bark()
p.weep()

```

#### 2. Encapsulation


class Account:
    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance   # private variable

    def deposit(self, amount):
        self.__balance += amount

    def get_balance(self):
        return self.__balance

acc = Account("Alice", 1000)
acc.deposit(500)
print(acc.get_balance())  # ✅ Accessible through method
print(acc.__balance)    # ❌ Will throw error


