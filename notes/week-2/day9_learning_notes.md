# 📘 Week 2 – Python Intermediate  

## 📅 Day 9 – Python Exceptions & Error Handling  

### 🔑 Key Concepts
- **Errors** stop program execution.  
- **Exceptions** can be handled using `try-except`.  
- Common exceptions: `ZeroDivisionError`, `ValueError`, `FileNotFoundError`.  
- `else` runs if no exception occurs.  
- `finally` always runs (cleanup).  
- You can **raise exceptions** manually.  
- You can create **custom exceptions** for validation.  

---

### 📝 Example Programs  

#### 1. Division by Zero Handling
```python
try:
    a = int(input("Enter numerator: "))
    b = int(input("Enter denominator: "))
    result = a / b
    print("Result:", result)
except ZeroDivisionError:
    print("❌ Cannot divide by zero!")
except ValueError:
    print("❌ Please enter valid integers.")
