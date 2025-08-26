## 📅 Day 7 - String Modifications

### Changing Case

``` python
text = "python programming"
print(text.upper())   # PYTHON PROGRAMMING
print(text.lower())   # python programming
print(text.title())   # Python Programming
print(text.capitalize()) # Python programming
```

### Removing Whitespace

``` python
text = "   Hello World   "
print(text.strip())   # "Hello World"
print(text.lstrip())  # "Hello World   "
print(text.rstrip())  # "   Hello World"
```

### Replacing & Splitting

``` python
text = "I like Java"
print(text.replace("Java", "Python"))  # I like Python

words = "apple,banana,cherry"
print(words.split(","))  # ['apple', 'banana', 'cherry']
```

### Joining Strings

``` python
fruits = ['apple', 'banana', 'cherry']
print(" - ".join(fruits))  # apple - banana - cherry
```

### Finding & Checking

``` python
text = "Python is fun"
print(text.find("fun"))    # 10
print(text.startswith("Py"))  # True
print(text.endswith("fun"))   # True

print("123".isdigit())   # True
print("abc".isalpha())   # True
print("Hello".islower()) # False
```
