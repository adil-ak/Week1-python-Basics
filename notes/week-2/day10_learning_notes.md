# 📘 Week 2 – Python Intermediate  

## 📅 Day 10 – Exception Errors & Handling  

### 🔑 Key Concepts
- **Error**: Mistake in the program that causes failure.  
- **Exception**: A runtime error that can be handled.  
- **`try-except` block** is used to catch and handle exceptions.  
- **`else`** → Executes if no exception occurs.  
- **`finally`** → Always runs, useful for cleanup (like closing files).  
- **`raise`** → Used to throw exceptions manually.  
- **Custom Exceptions** → You can create your own exception classes.  

---

### 📝 Example Programs  

#### 1. Division by Zero Handling
try:
    a = int(input("Enter numerator: "))
    b = int(input("Enter denominator: "))
    result = a / b
    print("Result:", result)
except ZeroDivisionError:
    print("❌ Cannot divide by zero!")
except ValueError:
    print("❌ Please enter valid integers.")

  # 2.File Not Found Handling
  try:
    filename = input("Enter filename: ")
    with open(filename, "r") as f:
        content = f.read()
        print("File Content:\n", content)
except FileNotFoundError:
    print("❌ File does not exist.")

 # 3.Custom Exception – Invalid Age
  class InvalidAgeError(Exception):
    pass

try:
    age = int(input("Enter your age: "))
    if age < 18:
        raise InvalidAgeError("❌ You must be 18 or older.")
    print("✅ Age accepted.")
except InvalidAgeError as e:
    print(e)
except ValueError:
    print("❌ Invalid input. Enter numbers only.")
