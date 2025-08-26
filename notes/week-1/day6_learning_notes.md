## 📅 Day 6 - Strings

### What are Strings?

-   Strings are sequences of characters enclosed in **single (`'`),
    double (`"`)**, or **triple quotes (`'''` or `"""`)**.

-   Examples:

    ``` python
    text1 = 'Hello'
    text2 = "World"
    text3 = '''This is 
    a multiline string'''
    ```

### String Indexing

-   Strings are indexed, starting at **0**.

-   Negative indexing starts from the end.

    ``` python
    word = "Python"
    print(word[0])   # P
    print(word[-1])  # n
    ```

### String Slicing

-   Extract parts of a string using `[start:end:step]`.

    ``` python
    word = "Programming"
    print(word[0:6])    # Progra
    print(word[3:])     # gramming
    print(word[:5])     # Progr
    print(word[::2])    # Pormig
    ```

### String Operations

-   Concatenation (`+`), Repetition (`*`), Membership (`in` / `not in`).

    ``` python
    a = "Hello"
    b = "World"
    print(a + " " + b)   # Hello World
    print(a * 3)         # HelloHelloHello
    print("H" in a)      # True
    ```
