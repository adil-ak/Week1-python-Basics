# 📘 Day 8 – Python File Handling 

Today’s focus: **File Handling in Python** – how to create, read, write, append, and delete files.  

---

## 🔑 Key Concepts  

### 1. Opening a File  
```python
f = open("filename.txt", "mode")
```
#### 2.Reading File
```python
f = open("sample.txt", "r")
print(f.read())          # read entire file
print(f.read(10))        # read first 10 characters
print(f.readline())      # read one line
print(f.readlines())     # read all lines as list
f.close()
```
### 3.Writing to a file
```python
f = open("sample.txt", "w")
f.write("Hello, World!\n")
f.write("Python File Handling is easy.")
f.close()
```
# Append mode
```python
f = open("sample.txt", "a")
f.write("\nThis line is appended.")
f.close()
```
### 4.Using with Statement
```python
with open("sample.txt", "r") as f:
    data = f.read()
    print(data)   # no need to close file manually
```
### 5.Deleting a File
```python
import os

if os.path.exists("sample.txt"):
    os.remove("sample.txt")
    print("File deleted.")
else:
    print("File does not exist.")
```
