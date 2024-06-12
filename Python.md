# Introduction to Python

Python is a high-level programming language for general-purpose programming. It is an open-source, interpreted, object-oriented programming language. Python was created by a Dutch programmer, Guido van Rossum. The name of the Python programming language was derived from a British sketch comedy series, Monty Python's Flying Circus. The first version was released on February 20, 1991.

# Why Python

Python is a programming language that is very close to human language and because of that, it is easy to learn and use. Python is used by various industries and companies (including Google). It has been used to develop web applications, desktop applications, system administration, and machine learning libraries. Python is highly embraced in the data science and machine learning community.

# Comments

Comments are very important to make the code more readable and to leave remarks in our code. Python does not run comment parts of our code. Any text starting with a hash (#) in Python is a comment.
```python
# This is a single line comment
```
Triple quotes can be used for multiline comments if they are not assigned to a variable.
```python
"""
This is
a multi-line comment
"""
```

# Basic Input/Output Functions

In Python, the `print()` function is used to output text or values to the console (or output page). This function can take multiple arguments and can handle different data types, converting them to strings as needed.
```python
print("Hello Python")
print("Hello!")
a = 10
b = "Raghul"
print(a)
print(b)
print(a + 10)
print('%d %s' % (a, b))
print('a = {} \nb = {}'.format(a, b))
print(f'a = {a} \nb = {b}')
fruits = ["apple", "banana", "cherry"]
print(fruits)
print("apple", "banana", "cherry", sep=", ")
print("Hello", end=" ")
print("World")
```

To read input from the user in Python, you use the `input()` function. This function prompts the user to enter some data and then returns the data as a string.
```python
user_input = input("Enter something: ")
print("You entered:", user_input)

age = input("Enter your age: ")
age = int(age)
height = input("Enter your height in meters: ")
height = float(height)
print("Your age is:", age)
print("Your height is:", height)

age = int(input("Enter your age: "))
height = float(input("Enter your height in meters: "))
print("Your age is:", age)
print("Your height is:", height)
```

# Indentation

Python uses whitespace such as spaces and tabs to define program blocks whereas other languages like C, C++, and Java use curly braces `{}` to indicate blocks of code for class, functions, loops, and block of selection command. The number of whitespaces (spaces and tabs) in the indentation is not fixed, but all statements within the block must be indented with the same amount of space.
```python
if 5 > 2:
    print("Hello")
k2 = 12
print(12)
```

# Variable Name

Variables store data in computer memory. A variable refers to a memory address in which data is stored.

## Python Variable Name Rules

- A variable name must start with a letter or the underscore character.
- A variable name cannot start with a number.
- A variable name can only contain alphanumeric characters and underscores (A-z, 0-9, and _ ).
- Variable names are case-sensitive (e.g., firstname, Firstname, FirstName, and FIRSTNAME are different variables).

```python
x = 10
y = "Hello"
print(x, y)

x = "Hello"
print(x, y)
```

# Data Types

All data values in Python are objects and each object or value has a type. Python has built-in or fundamental data types such as Number, String, Boolean, tuples, lists, sets, and dictionaries.

```python
x, y, z = "Orange", 12, 3.14
del x, y, z

a = 10
b = -42
c = 0
d = 0b1010
e = 0b1111
f = 0o12
g = 0O77
h = 0xA
i = 0Xa
j = 10.5
k = -0.001
l = 1.5e2
m = 2.5E-3
print(a, b, c, d, e, f, g, h, i, j, k, l, m)
print(a, type(a))
print(b, type(b))
print(c, type(c))
print(d, type(d))
print(e, type(e))
print(f, type(f))
print(g, type(g))
print(h, type(h))
print(i, type(i))
print(j, type(j))
print(k, type(k))
print(l, type(l))
print(m, type(m))
```

# Casting

```python
x = str(3)
y = int(3)
z = float(3)
print(x, y, z)
```

# Get the data type

```python
a = 13
b = "Raja"
c = 3.14
d = 'A'
print(type(a))
print(type(b))
print(type(c))
print(type(d))
```

# Case-Sensitive

```python
a = 4
A = "Raja"
print(a)
print(A)
```

# Single or Double Quotes

```python
a = 'Raja'
b = "Rani"
print(a)
print(b)
```

# Assign Multiple Values

```python
x, y, z = "Orange", 12, 3.14
print(x, y, z)
```

# Assign One value to Multiple Variables

```python
x = y = z = "Raja"
print(x, y, z)
```

# Operator

In computer programming languages, operators are special symbols that represent computations, conditional matching, etc. The value of an operator used is called operands. Operators are categorized as Arithmetic, Relational, Logical, Assignment, etc. Values and variables when used with operators are known as operands.

# Arithmetic Operator

An arithmetic operator is a mathematical operator that takes two operands and performs a calculation on them. They are used for simple arithmetic. Most computer languages contain a set of such operators that can be used within equations to perform different types of sequential calculations.

```python
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
print(a // b)
print(a ** b)
```

# Relational Operator/Comparison Operators

A relational operator is also called a comparative operator which checks the relationship between two operands. If the relation is true, it returns True; otherwise, it returns False.

```python
a = 10
b = 10
print(a > b)
print(a >= b)
print(a < b)
print(a <= b)
print(a == b)
print(a != b)

a = 100
b = [10, 20, 30, 40]
print(10 is 10)
print(10 is not 10)
print(a is b)
print(a is not b)
print(a in b)
print(a not in b)
```

# Logical Operators

Logical operators are used to perform logical operations on the given relational expressions. There are three logical operators: and, or, and not.

```python
a = 10
b = 10
print("Logical AND")
print((a < b), "+", (a > b), "=", (a < b) and (a > b))
print((a <= b), "+", (a > b), "=", (a <= b) and (a > b))
print((a < b), "+", (a >= b), "=", (a < b) and (a >= b))
print((a <= b), "+", (a >= b), "=", (a <= b) and (a >= b))

print("\n\nLogical OR")
print((a < b), "+", (a > b), "=", (a < b) or (a > b))
print((a <= b), "+", (a > b), "=", (a <= b) or (a > b))
print((a < b), "+", (a >= b), "=", (a < b) or (a >= b))
print((a <= b), "+", (a >= b), "=", (a <= b) or (a >= b))

print("\n\nLogical Not")
print(a < b, "=", not (a < b))
print(a <= b, "=", not (a <= b))
```

# Assignment Operator

In Python, = is a simple assignment operator to assign values to variables.

```python
a = 10
b = 3
a += b
print(a)
a -= b
print(a)
a *= b
print(a)
a /= b
print(a)
a **= b
print(a)
a //= b
print(a)
a %= b
print(a)
```

# Conditional operator

The ternary operator is also known as a conditional operator that evaluates something based on a condition being true or false. It simply allows testing a condition in a single line, replacing the multiline if-else, making the code compact.

```python
a, b = 100, 20
min = a if a < b else b
print(min)
```

# String

## Single line String

```python
a =

 "Raja"
b = 'Rani'
print(a, b)
```

## Multiline String

```python
a = """Raja
Rani"""
print(a)

a = '''Raja
Rani'''
print(a)
```

## String Length

```python
a = "Raja"
print(len(a))
```

## Check String

```python
a = "Raja"
print("a" in a)
print("R" not in a)
```

## Concatenate Strings

```python
a = "Raja"
b = "Rani"
c = a + b
print(c)

a = "Raja"
b = "Rani"
c = a + " " + b
print(c)
```

## Format String

We cannot combine string and number directly. But we can combine them using `format()`.

```python
age = 23
txt = "My name is Raja, and I am {}"
print(txt.format(age))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {0} pieces of item {1} for {2} dollars."
print(myorder.format(quantity, itemno, price))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {2} pieces of item {1} for {0} dollars."
print(myorder.format(quantity, itemno, price))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {q} pieces of item {i} for {p} dollars."
print(myorder.format(q=quantity, i=itemno, p=price))
```

# String Methods

- capitalize()
- casefold()
- center()
- count()
- encode()
- endswith()
- expandtabs()
- find()
- format()
- format_map()
- index()
- isalnum()
- isalpha()
- isascii()
- isdecimal()
- isdigit()
- isidentifier()
- islower()
- isnumeric()
- isprintable()
- isspace()
- istitle()
- isupper()
- join()
- ljust()
- lower()
- lstrip()
- maketrans()
- partition()
- removeprefix()
- removesuffix()
- replace()
- rfind()
- rindex()
- rjust()
- rpartition()
- rsplit()
- rstrip()
- split()
- splitlines()
- startswith()
- strip()
- swapcase()
- title()
- translate()
- upper()
- zfill()

```python
a = "raja"
print(a.capitalize())
print(a.upper())
print(a.lower())
print(a.strip())
print(a.split())
print(a.split("a"))
print(a.split("a", 1))
print(a.count("a"))
print(a.replace("a", "o"))
print(a.find("a"))
print(a.index("a"))
print(a.startswith("r"))
print(a.endswith("a"))
print(a.isalnum())
print(a.isalpha())
print(a.isdigit())
print(a.islower())
print(a.isupper())
print(a.istitle())
print(a.isspace())
print(a.center(10, "*"))
print(a.zfill(10))
print(a.swapcase())
print(a.title())
print(a.ljust(10, "*"))
print(a.rjust(10, "*"))
print(a.removeprefix("r"))
print(a.removesuffix("a"))
print(a.translate({97: 100}))
```

# Slicing

```python
a = "Hello, World!"
print(a[1:5])
print(a[:5])
print(a[2:])
print(a[-5:-2])
print(a[::-1])
print(a[::2])
print(a[1:5:2])
print(a[::])
print(a[:])
```

# Data Structure

A data structure is a storage that is used to store and organize data. It is a way of arranging data on a computer so that it can be accessed and updated efficiently. Python has primitive (or basic) data structures such as float, integer, string, and boolean, and non-primitive (or advanced) data structures like list, tuple, dictionary, and set.

## List

Lists are ordered collections of items that are changeable and allow duplicate elements. List items are indexed, the first item has index [0], the second item has index [1], and so on.

```python
fruits = ["apple", "banana", "cherry"]
print(fruits)
print(fruits[0])
print(fruits[1])
print(fruits[2])
print(fruits[-1])
print(fruits[-2])
print(fruits[-3])
print(fruits[0:2])
print(fruits[:2])
print(fruits[1:])
print(fruits[::2])
print(fruits[::-1])
```

### List Methods

```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits)
fruits.insert(1, "grape")
print(fruits)
fruits.remove("banana")
print(fruits)
fruits.pop()
print(fruits)
fruits.pop(1)
print(fruits)
fruits.clear()
print(fruits)
fruits = ["apple", "banana", "cherry"]
del fruits[0]
print(fruits)
del fruits
fruits = ["apple", "banana", "cherry"]
print(fruits.index("banana"))
print(fruits.count("banana"))
fruits.reverse()
print(fruits)
fruits.sort()
print(fruits)
fruits.sort(reverse=True)
print(fruits)
```

## Tuple

Tuples are ordered collections of items that are unchangeable and allow duplicate elements. Tuple items are indexed, the first item has index [0], the second item has index [1], and so on.

```python
fruits = ("apple", "banana", "cherry")
print(fruits)
print(fruits[0])
print(fruits[1])
print(fruits[2])
print(fruits[-1])
print(fruits[-2])
print(fruits[-3])
print(fruits[0:2])
print(fruits[:2])
print(fruits[1:])
print(fruits[::2])
print(fruits[::-1])
```

### Tuple Methods

```python
fruits = ("apple", "banana", "cherry")
print(fruits.index("banana"))
print(fruits.count("banana"))
```

## Set

Sets are unordered collections of items that do not allow duplicate elements.

```python
fruits = {"apple", "banana", "cherry"}
print(fruits)
fruits.add("orange")
print(fruits)
fruits.update(["grape", "mango"])
print(fruits)
fruits.remove("banana")
print(fruits)
fruits.discard("banana")
print(fruits)
fruits.pop()
print(fruits)
fruits.clear()
print(fruits)
del fruits
fruits = {"apple", "banana", "cherry"}
print("banana" in fruits)
print("grape" not in fruits)
```

### Set Methods

```python
fruits = {"apple", "banana", "cherry"}
fruits.add("orange")
print(fruits)
fruits.update(["grape", "mango"])
print(fruits)
fruits.remove("banana")
print(fruits)
fruits.discard("banana")
print(fruits)
fruits.pop()
print(fruits)
fruits.clear()
print(fruits)
fruits = {"apple", "banana", "cherry"}
fruits2 = {"orange", "grape", "mango"}
print(fruits.union(fruits2))
print(fruits.intersection(fruits2))
print(fruits.difference(fruits2))
print(fruits.symmetric_difference(fruits2))
fruits.update(fruits2)
print(fruits)
```

## Dictionary

Dictionaries are unordered collections of items that are changeable and indexed. They are written with curly braces, and they have keys and values.

```python
person = {
    "name": "Raja",
    "age": 23,
    "city": "Chennai"
}
print(person)
print(person["name"])
print(person["age"])
print(person["city"])
print(person.get("name"))
print(person.get("age"))
print(person.get("city"))
person["age"] = 24
print(person)
person["country"] = "India"
print(person)
person.pop("age")
print(person)
person.popitem()
print(person)
person.clear()
print(person)
del person
person = {
    "name": "Raja",
    "age": 23,
    "city": "Chennai"
}
for key in person:
    print(key)
for value in person.values():
    print(value)
for key, value in person.items():
    print(key, value)
```

### Dictionary Methods

```python
person = {
    "name": "Raja",
    "age": 23,
    "city": "Chennai"
}
person.update({"country": "India"})
print(person)
print(person.keys())
print(person.values())
print(person.items())
print(person.copy())
person = dict(name="Raja", age=23, city="Chennai")
print(person)
```

### Nested Dictionary

```python
myfamily = {
    "child1": {
        "name": "Emil",
        "year": 2004
    },
    "child2": {
        "name": "Tobias",
        "year": 2007
    },
    "child3": {
        "name": "Linus",
        "year": 2011


    }
}
print(myfamily)
```

# Function

A function is a block of code that only runs when it is called. You can pass data, known as parameters, into a function. A function can return data as a result.

## Creating a Function

```python
def my_function():
    print("Hello from a function")

my_function()
```

## Parameters

Information can be passed into functions as parameters. Parameters are specified after the function name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma.

```python
def my_function(fname):
    print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")
```

## Default Parameter Value

The following example shows how to use a default parameter value. If we call the function without a parameter, it uses the default value.

```python
def my_function(country="Norway"):
    print("I am from " + country)

my_function("Sweden")
my_function("India")
my_function()
my_function("Brazil")
```

## Return Values

To let a function return a value, use the `return` statement.

```python
def my_function(x):
    return 5 * x

print(my_function(3))
print(my_function(5))
print(my_function(9))
```

## Keyword Arguments

You can also send arguments with the key=value syntax. This way the order of the arguments does not matter.

```python
def my_function(child3, child2, child1):
    print("The youngest child is " + child3)

my_function(child1="Emil", child2="Tobias", child3="Linus")
```

## Arbitrary Arguments

If you do not know how many arguments that will be passed into your function, add a `*` before the parameter name in the function definition.

```python
def my_function(*kids):
    print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus")
```

## Arbitrary Keyword Arguments

If you do not know how many keyword arguments that will be passed into your function, add two asterisk: `**` before the parameter name in the function definition.

```python
def my_function(**kid):
    print("His last name is " + kid["lname"])

my_function(fname="Tobias", lname="Refsnes")
```

# Lambda Function

A lambda function is a small anonymous function. A lambda function can take any number of arguments, but can only have one expression.

```python
x = lambda a: a + 10
print(x(5))

x = lambda a, b: a * b
print(x(5, 6))

x = lambda a, b, c: a + b + c
print(x(5, 6, 2))
```

# Module

A module is a file containing Python definitions and statements. A module can define functions, classes, and variables. A module can also include runnable code. Grouping related code into a module makes the code easier to understand and use.

## Creating a Module

To create a module, save the code you want in a file with the file extension `.py`.

```python
def greeting(name):
    print("Hello, " + name)
```

## Using a Module

Now we can use the module we just created, by using the `import` statement.

```python
import mymodule

mymodule.greeting("Jonathan")
```

## Variables in Module

The module can contain functions, as already described, but also variables of all types (arrays, dictionaries, objects etc).

```python
person1 = {
    "name": "John",
    "age": 36,
    "country": "Norway"
}
```

```python
import mymodule

a = mymodule.person1["age"]
print(a)
```

## Renaming a Module

You can create an alias when you import a module, by using the `as` keyword.

```python
import mymodule as mx

a = mx.person1["age"]
print(a)
```

## Built-in Modules

There are several built-in modules in Python, which you can import whenever you like.

```python
import platform

x = platform.system()
print(x)
```

## Using the `dir()` Function

There is a built-in function to list all the function names (or variable names) in a module. The `dir()` function.

```python
import platform

x = dir(platform)
print(x)
```

## Import From Module

You can choose to import only parts from a module, by using the `from` keyword.

```python
from mymodule import person1

print(person1["age"])
```

# Class

Python is an object-oriented programming language. Almost everything in Python is an object, with its properties and methods. A class is like an object constructor, or a "blueprint" for creating objects.

## Create a Class

To create a class, use the keyword `class`.

```python
class MyClass:
    x = 5

p1 = MyClass()
print(p1.x)
```

## The `__init__()` Function

The `__init__()` function is called automatically every time the class is being used to create a new object.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)
```

## Object Methods

Objects can also contain methods. Methods in objects are functions that belong to the object.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def myfunc(self):
        print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc()
```

## The `self` Parameter

The `self` parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def myfunc(self):
        print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc()
```

## Modify Object Properties

You can modify properties on objects like this.

```python
p1.age = 40
print(p1.age)
```

## Delete Object Properties

You can delete properties on objects by using the `del` keyword.

```python
del p1.age
```

## Delete Objects

You can delete objects by using the `del` keyword.

```python
del p1
```

## The `pass` Statement

```python
class Person:
    pass
```

# File Handling

File handling is an important part of any web application. Python has several functions for creating, reading, updating, and deleting files.

## File Handling Methods

- `open()`
- `read()`
- `readline()`
- `readlines()`
- `write()`
- `writelines()`
- `close()`

## Open a File

The key function for working with files in Python is the `open()` function. The `open()` function takes two parameters; filename, and mode.

There are four different methods (modes) for opening a file:

- `"r"` - Read - Default value. Opens a file for reading, error if the file does not exist.
- `"a"` - Append - Opens a file for appending, creates the file if it does not exist.
- `"w"` - Write - Opens a file for writing, creates the file if it does not exist.
- `"x"` - Create - Creates the specified file, returns an error if the file exists.

In addition, you can specify if the file should be handled as binary or text mode.

- `"t"` - Text - Default value. Text mode.
- `"b"` - Binary - Binary mode (e.g. images).

```python
f = open("demofile.txt")
print(f.read())
```

## Write to a File

```python
f = open("demofile.txt", "w")
f.write("Now the file has more content!")
f.close()

f = open("demofile.txt", "r")
print(f.read())
```

## Append to a File

```python
f = open("demofile.txt", "a")
f.write("Now the file has more content!")
f.close()

f = open("demofile.txt", "r")
print(f.read())
```

## Read a File

```python
f = open("demofile.txt", "r")
print(f.read())
```

### Read Only Parts of the File

```python
f = open("demofile.txt", "r")
print(f.read(5))
```

### Read Lines

```python
f = open("demofile.txt", "r")
print(f.readline())
print(f.readline())
```

### Loop Through the File Line by Line

```python
f = open("demofile.txt", "r")
for x in f:
    print(x)
```

## Delete a File

To delete a file, you must import the `os` module, and run its `os.remove()` function.

```python
import os
os.remove("demofile.txt")
```

## Check if File Exists

To avoid getting an error, you might want to check if the file exists before you try to delete it.

```python
import os
if os.path.exists("demofile.txt"):
    os.remove("demofile.txt")
else:
    print("The file does not exist")


```

## Delete Folder

To delete an entire folder, use the `os.rmdir()` method.

```python
import os
os.rmdir("myfolder")
```

# Exception Handling

Python has many built-in exceptions that are raised when your program encounters an error (something in the program goes wrong). When these exceptions occur, the Python interpreter stops the current process and passes it to the calling process until it is handled. If not handled, the program will crash.

## Exception Handling Methods

- `try`
- `except`
- `finally`
- `raise`

## Handle an Exception

```python
try:
    print(x)
except:
    print("An exception occurred")
```

## Many Exceptions

```python
try:
    print(x)
except NameError:
    print("Variable x is not defined")
except:
    print("Something else went wrong")
```

## Else

You can use the `else` keyword to define a block of code to be executed if no errors were raised.

```python
try:
    print("Hello")
except:
    print("Something went wrong")
else:
    print("Nothing went wrong")
```

## Finally

The `finally` block, if specified, will be executed regardless if the try block raises an error or not.

```python
try:
    print(x)
except:
    print("Something went wrong")
finally:
    print("The try-except block is finished")
```

## Raise an Exception

As a Python developer, you can choose to throw an exception if a condition occurs. To throw (or raise) an exception, use the `raise` keyword.

```python
x = -1

if x < 0:
    raise Exception("Sorry, no numbers below zero")
```

# Regular Expressions

A RegEx, or Regular Expression, is a sequence of characters that forms a search pattern. RegEx can be used to check if a string contains the specified search pattern.

Python has a built-in package called `re`, which can be used to work with Regular Expressions.

## Import the `re` Module

```python
import re

txt = "The rain in Spain"
x = re.search("^The.*Spain$", txt)
print(x)
```

### The `findall()` Function

The `findall()` function returns a list containing all matches.

```python
import re

txt = "The rain in Spain"
x = re.findall("ai", txt)
print(x)
```

### The `search()` Function

The `search()` function searches the string for a match, and returns a `Match` object if there is a match.

```python
import re

txt = "The rain in Spain"
x = re.search("\s", txt)
print("The first white-space character is located in position:", x.start())
```

### The `split()` Function

The `split()` function returns a list where the string has been split at each match.

```python
import re

txt = "The rain in Spain"
x = re.split("\s", txt)
print(x)
```

### The `sub()` Function

The `sub()` function replaces the matches with the text of your choice.

```python
import re

txt = "The rain in Spain"
x = re.sub("\s", "9", txt)
print(x)
```

## Metacharacters

Metacharacters are characters with a special meaning.

- `[]` - A set of characters
- `\` - Signals a special sequence (can also be used to escape special characters)
- `.` - Any character (except newline character)
- `^` - Starts with
- `$` - Ends with
- `*` - Zero or more occurrences
- `+` - One or more occurrences
- `?` - Zero or one occurrences
- `{}` - Exactly the specified number of occurrences
- `|` - Either or
- `()` - Capture and group

## Special Sequences

A special sequence is a `\` followed by one of the characters in the list below, and has a special meaning:

- `\A` - Returns a match if the specified characters are at the beginning of the string
- `\b` - Returns a match where the specified characters are at the beginning or at the end of a word
- `\B` - Returns a match where the specified characters are present, but NOT at the beginning (or at the end) of a word
- `\d` - Returns a match where the string contains digits (numbers from 0-9)
- `\D` - Returns a match where the string DOES NOT contain digits
- `\s` - Returns a match where the string contains a white space character
- `\S` - Returns a match where the string DOES NOT contain a white space character
- `\w` - Returns a match where the string contains any word characters (characters from a to Z, digits from 0-9, and the underscore _ character)
- `\W` - Returns a match where the string DOES NOT contain any word characters
- `\Z` - Returns a match if the specified characters are at the end of the string

```python
import re

txt = "The rain in Spain"
x = re.findall("\AThe", txt)
print(x)
```

# JSON

JSON is a syntax for storing and exchanging data. JSON is text, written with JavaScript object notation.

## JSON in Python

Python has a built-in package called `json`, which can be used to work with JSON data.

```python
import json

# some JSON
x = '{"name":"John", "age":30, "city":"New York"}'

# parse x:
y = json.loads(x)

# the result is a Python dictionary:
print(y["age"])
```

### Convert From Python to JSON

```python
import json

# a Python object (dict):
x = {
    "name": "John",
    "age": 30,
    "city": "New York"
}

# convert into JSON:
y = json.dumps(x)

# the result is a JSON string:
print(y)
```

## JSON Methods

| Method | Description |
|---|---|
| `json.dumps()` | Converts a Python object into a JSON string |
| `json.loads()` | Converts a JSON string into a Python object |

```python
import json

print(json.dumps({"name": "John", "age": 30}))
print(json.dumps(["apple", "bananas"]))
print(json.dumps(("apple", "bananas")))
print(json.dumps("hello"))
print(json.dumps(42))
print(json.dumps(31.76))
print(json.dumps(True))
print(json.dumps(False))
print(json.dumps(None))
```

```python
import json

x = {
    "name": "John",
    "age": 30,
    "married": True,
    "divorced": False,
    "children": ("Ann", "Billy"),
    "pets": None,
    "cars": [
        {"model": "BMW 230", "mpg": 27.5},
        {"model": "Ford Edge", "mpg": 24.1}
    ]
}

print(json.dumps(x))
print(json.dumps(x, indent=4))
print(json.dumps(x, indent=4, sort_keys=True))
```

# Date and Time

Python has a built-in module called `datetime` to work with dates and times.

## Date and Time Methods

- `datetime.now()`
- `datetime.today()`
- `datetime.date()`
- `datetime.time()`
- `datetime.datetime()`
- `datetime.timedelta()`

```python
import datetime

x = datetime.datetime.now()
print(x)
```

## Create Date Objects

To create a date, we can use the `datetime()` class (constructor) of the `datetime` module.

```python
import datetime

x = datetime.datetime(2020, 5, 17)
print(x)
```

## The `strftime()` Method

The `strftime()` method is used to format dates.

```python
import datetime

x = datetime.datetime.now()
print(x.strftime("%B"))
```

# Iterators

An iterator is an object that contains a countable number of values. An iterator is an object that can be iterated upon, meaning that you can traverse through all the values.

## Iterator vs Iterable

Lists, tuples, dictionaries, and sets are all iterable objects. They are iterable containers from which you can get an iterator. All these objects have a `iter()` method which is used to get an iterator.

```python
mytuple = ("apple", "banana", "cherry")
myit = iter(mytuple)

print(next(myit))
print(next(myit))
print(next(myit))
```

## Looping Through an Iterator

```python
mytuple = ("apple", "banana", "cherry")

for x in mytuple:
    print(x)
```

## Create an Iterator

To create an object/class as an iterator you have to implement the methods `__iter__()` and `__next__()` to your object.

```python
class MyNumbers:
    def __iter__(self):
        self.a = 1
        return self

    def __next__(self):
        x = self.a
        self.a += 1
        return x

myclass = MyNumbers()
myiter = iter(myclass)

print(next(myiter))
print(next(myiter))
print(next(myiter))
print(next(myiter))
print(next(myiter))
```

## StopIteration

To prevent the iteration from going forever, we can use the `StopIteration` statement.

```python
class MyNumbers:
    def __iter__(self):
        self.a = 1
        return self

    def __next__(self):
        if self.a <= 20:
            x = self.a
           

 self.a += 1
            return x
        else:
            raise StopIteration

myclass = MyNumbers()
myiter = iter(myclass)

for x in myiter:
    print(x)
```

# Testing

Testing is the process of evaluating a system or its component(s) with the intent to find whether it satisfies the specified requirements or not. It is the process of executing a program with the intent of finding an error.

## Testing in Python

Python's built-in `unittest` module can be used to test your code.

```python
import unittest

def add(a, b):
    return a + b

class TestAddFunction(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(2, 3), 5)

if __name__ == '__main__':
    unittest.main()
```

## Writing Test Cases

A test case is a single unit of testing. It checks for a specific response to a particular set of inputs.

```python
import unittest

def add(a, b):
    return a + b

class TestAddFunction(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(2, 3), 5)
        self.assertEqual(add(-1, 1), 0)
        self.assertEqual(add(-1, -1), -2)

if __name__ == '__main__':
    unittest.main()
```

## Running Tests

To run the tests, you can use the command line:

```bash
python -m unittest test_file.py
```

# Conclusion

This guide covered the basics of Python programming, from simple syntax and data structures to more advanced topics like functions, classes, file handling, and testing. Understanding these concepts will give you a solid foundation to further explore and master Python programming.
