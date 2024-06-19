[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15299552&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

Python is a high-level programming language known for its simplicity and readability. Key features include a clear syntax, extensive standard library, platform independence, support for multiple paradigms, and a rich ecosystem of third-party libraries. It's popular for web development (Django, Flask), data science (NumPy, Pandas), automation, prototyping, and education due to its ease of use and versatility.



   



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.


 Installing Python on Windows

Download Python:
   - Go to [python.org](https://www.python.org/downloads/) and download the latest Python installer for Windows.

Run the Installer:
   - Double-click the downloaded installer (`python-3.x.x.exe`).
   - Check the box "Add Python x.x to PATH".
   - Click "Install Now".

Verify Installation:
   - Open Command Prompt (`cmd`).
   - Type `python --version` and press Enter.
   - This command should display the installed Python version.

Install `virtualenv`:
   - Open your terminal.
   - Install `virtualenv` using pip:
     
     pip install virtualenv


   -Activate the virtual environment using this command
      source "vevnv name"/Scripts/activate








3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")

-print() function: Outputs text or variables to the console.
-"Hello, World!": String literal enclosed in double quotes, representing the text to be printed.








4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

 The basic data types in Python include:

-Integer (int): Whole numbers without decimals.
-Float (float): Numbers with decimal points.
-String (str): Text enclosed in single, double, or triple quotes.
-Boolean (bool): Represents True or False.
-List (list): Ordered collection of items, enclosed in square brackets.
-Tuple (tuple): Ordered, immutable collection of items, enclosed in parentheses.
-Dictionary (dict): Key-value pairs, enclosed in curly braces.
-Set (set): Unordered collection of unique items, enclosed in curly braces

# Integer
age = 25
print(age) 

# Float
height = 5.9
print(height) 

# String
name = "Alice"
print(name) 

# Boolean
is_student = True
print(is_student) 

# List
fruits = ["apple", "banana", "cherry"]
print(fruits)  

# Tuple
coordinates = (10.0, 20.0)
print(coordinates) 

# Dictionary
person = {"name": "Alice", "age": 25}
print(person)  # Output: 

# Set
colors = {"red", "blue", "green"}
print(colors) 










5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.



Conditional statements and loops are fundamental control structures in Python that allow you to control the flow of execution based on conditions and repeat code blocks multiple times.

### Conditional Statements (if-else)

Conditional statements in Python allow you to execute certain blocks of code based on whether a condition is true or false. The basic syntax includes `if`, `else`, and optionally `elif` (short for "else if") for multiple conditions.

Example of an `if-else` statement:


number = 10

if number > 0:
    print(f"{number} is positive.")
elif number < 0:
    print(f"{number} is negative.")
else:
    print(f"{number} is zero.")

Explanation:
- The `if` statement checks if `number > 0`.
- If true, it prints that the number is positive.
- The `elif` statement (else if) checks if `number < 0`.
- If true, it prints that the number is negative.
- If both conditions (`number > 0` and `number < 0`) are false, the `else` block executes, printing that the number is zero.

FOR LOOP
Loops in Python allow you to execute a block of code repeatedly. The for loop iterates over a sequence (such as lists, tuples, dictionaries, or ranges) or any iterable object.

Example:
numbers = [1, 2, 3, 4, 5]

for num in numbers:
    print(num)

Explanation:

-numbers is a list containing integers [1, 2, 3, 4, 5].
-The for loop iterates through each element (num) in the numbers list.
-In each iteration, it prints the value of num.










6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.


Functions in Python are blocks of organized, reusable code that perform a specific task. They allow you to break down a program into smaller, modular pieces, making the code more organized, readable, and easier to maintain. Functions in Python are defined using the def keyword.

Example:
def add_numbers(a, b):
    """Function to add two numbers."""
    return a + b

To call the above function;

result = add_numbers(3, 5)
print(result)









7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Differences Between Lists and Dictionaries in Python:


Lists (list):

-Ordered collection of items.
-Elements are accessed by index (integer position starting from 0).
-Mutable: Elements can be changed, added, or removed.
-Elements can be of different data types (e.g., integers, strings, other lists).


Dictionaries (dict):

-Unordered collection of key-value pairs.
-Elements are accessed by keys (unique identifier).
-Mutable: Values can be changed, added, or removed; keys are immutable (cannot be changed once set).
-Keys are typically strings or numbers; values can be of any data type (e.g., integers, strings, lists).



EXAMPLE
# Create a list of numbers
numbers = [1, 2, 3, 4, 5]

# Create a dictionary with some key-value pairs
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York",
    "email": "alice@example.com"
}

# Print the list and dictionary
print("List of numbers:", numbers)
print("Dictionary of a person:", person)

# Accessing elements:
print("\nAccessing elements:")
print("Third number in the list:", numbers[2])  # Accessing by index
print("Name of the person:", person["name"])    # Accessing by key

# Updating elements:
print("\nUpdating elements:")
numbers[0] = 10            # Update list element
person["age"] = 31         # Update dictionary value
print("Updated list of numbers:", numbers)
print("Updated dictionary of a person:", person)

# Adding elements:
print("\nAdding elements:")
numbers.append(6)          # Add new element to list
person["phone"] = "123-456-7890"  # Add new key-value pair to dictionary
print("List after adding a number:", numbers)
print("Dictionary after adding phone number:", person)

# Removing elements:
print("\nRemoving elements:")
removed_number = numbers.pop(2)  # Remove and return element by index
removed_email = person.pop("email")  # Remove and return element by key
print("Removed number from list:", removed_number)
print("Removed email from dictionary:", removed_email)
print("List after removing element:", numbers)
print("Dictionary after removing email:", person)

# Length of list and dictionary:
print("\nLength of list and dictionary:")
print("Length of numbers list:", len(numbers))
print("Length of person dictionary:", len(person))

source:
Generative Pre-trained Transformer









8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.


Exception handling in Python allows you to gracefully manage and respond to errors that occur during program execution. It prevents your program from crashing abruptly when encountering unexpected situations, such as division by zero, accessing a non-existent file, or invalid input.

Example in python:

def divide_numbers(a, b):
    try:
        result = a / b
        print(f"{a} divided by {b} is {result}")
    except ZeroDivisionError:
        print("Error: Division by zero is not allowed!")
    finally:
        print("Execution of divide_numbers function completed.")

# Example usage:
divide_numbers(10, 2)   
divide_numbers(5, 0)    







9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.


Modules and Packages in Python
MODULES:
A module is a file containing Python definitions (functions, variables, classes).
Example: my_module.py

PACKAGE:
A package is a directory of modules.

Example:
import math

radius = 5
area = math.pi * radius ** 2
print(f"Area of circle with radius {radius} is {area:.2f}")  # Output: Area of circle with radius 5 is 78.54







10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


To read from a file in Python, we use `open('filename.txt', 'r').read()`; to write to a file, use `open('output.txt', 'w').writelines(["Line 1\n", "Line 2\n", "Line 3\n"])`.



SCRIPT TO READ

file_path = "example.txt"
with open(file_path, 'r') as file:
    # Read and print the content
    file_content = file.read()
    print(file_content)

SCRIPT TO WRITE

# List of strings to write
lines_to_write = [
    "Hello,",
    "Welcome to Python file handling.",
    "This is a new line.",
    "Goodbye!"
]

# Specify the file path
file_path = "output.txt"

# Open the file in write mode
with open(file_path, 'w') as file:
    # Write each string in the list to the file
    for line in lines_to_write:
        file.write(line + "\n")









# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


