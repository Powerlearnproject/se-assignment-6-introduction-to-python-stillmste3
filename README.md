[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15314581&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a high-level, object-oriented, and interpreted programming language. Python is easy to lean, free and open source, has a remarkable standard library, which includes an extensive selection of modules and packages like itertools, functools, and operator. These pre-built tools are indispensable for developers and significantly decrease the time and effort required to implement projects.
   Real-world Python Use Cases: Amazon is heavily driven by machine learning and data science, and Python is the dominant language for creating machine learning models. Amazon has a recommendation engine under the hood that takes in data about your purchases and surfaces products similar to ones you have purchased before. 

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   To install Python on Windows, follow these steps:
- Visit the official Python website and navigate to the download page.
- Select the appropriate version of Python based on your Windows operating system.
- Click the Download button and wait for downloading python for windows.
- Once downloaded, run the Python installer by double-clicking on the downloaded file.
- Follow the prompts to complete the installation process.
- Once you have installed Python on your Windows system, you can check windows python version by opening a command prompt and typing python --version.
To create a virtualenv use the following command:
- python -m venv ./venv
Then change the directory to venv\Scripts:
- cd venv\Scripts
After changing the directory type the below command to activate the virtual environment:
- $ Source venv_name\Scripts> activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")
- print() is a built-in Python function used to display output on the console.
- "Hello, World!" is a string literal in Python.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   - Integer (int): Represents whole numbers without a fractional part.
   - Floating Point (float): Represents numbers with a fractional part. 
   - String (str): Represents sequences of characters.
   - Boolean (bool): Represents truth values.
   Script:
   age = 19
print("Integer:", age)

height = 5.9
print("Float:", height)

name = "Tumelo"
print("String:", name)

is_student = True
print("Boolean:", is_student)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements in Python allow you to execute different blocks of code based on certain conditions and loops allow you to execute a block of code multiple times.
   Example: Python if…else Statement :
    number = 10

if number > 0:
    print('Positive number')

else:
    print('Negative number')

print('This statement always executes')

Example of a for Loop:
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions are blocks of code that can take parameters, return values, and have different types of arguments.
   Functions are useful in Python because:
- They allow you to write a block of code once and use it multiple times, saving you lots of time in the future.
- They make your code easier to maintain because, if you need to update your function at some point, you only need to edit it in one place.
- They are reusable pieces of code that can be called using a function's name.
- They allow the same piece of code to run multiple times.
- They break long programs up into smaller components.

Function example:
def sum_two_numbers(a, b):
    return a + b
Calling the function:
result = sum_two_numbers(10, 16)
print("Sum:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists and Dictionaries in Python are inbuilt data structures that are used to store data. Lists are linear in nature whereas the dictionaries stored the data in key-value pair.
   # Creating a list of numbers
numbers = [1, 2, 3, 4, 5]

# Creating a dictionary
person = {
    'name': 'Tumelo',
    'age': 19,
    'city': 'Krugersdorp',
    'is_student': True
}

# Print the initial list and dictionary
print("Initial list of numbers:", numbers)
print("Initial dictionary:", person)
print()

# Accessing elements in the list
print("First element of the list:", numbers[0])
print("Last element of the list:", numbers[-1])
print()

# Accessing elements in the dictionary
print("Name of the person:", person['name'])
print("Age of the person:", person['age'])
print()

# Modifying elements in the list
numbers[0] = 10
print("Updated list of numbers after modification:", numbers)
print()

# Modifying elements in the dictionary
person['city'] = 'Johannesbug'
print("Updated dictionary after modification:", person)
print()

# Adding elements to the list
numbers.append(6)
print("List of numbers after adding an element:", numbers)
print()

# Adding elements to the dictionary
person['gender'] = 'female'
print("Dictionary after adding a key-value pair:", person)
print()

# Removing elements from the list
removed_element = numbers.pop(1)
print("List after removing element at index 1:", numbers)
print("Removed element from list:", removed_element)
print()

# Removing elements from the dictionary
del person['is_student']
print("Dictionary after removing 'is_student' key:", person)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling is the way python handles exceptions to execute code without frequent handling.
   def divide_numbers(a, b):
    try:
        result = a / b
    except ZeroDivisionError:
        print("Error: Division by zero!")
    else:
        print(f"The result of {a} divided by {b} is: {result}")
    finally:
        print("Executing finally block.")

divide_numbers(10, 2)

divide_numbers(5, 0)


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Python modules and Python packages, two mechanisms that facilitate modular programming. Modular programming refers to the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or modules.
   You can import a module by using the import statement.
   Example:
   import math

Estimated Reading Time: 9 mins


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    Python provides built-in functions for creating, writing, and reading files. Two types of files can be handled in Python, normal text files and binary files (written in binary language, 0s, and 1s).
    # Reading from a file and printing its content to console

file_path = 'sample.txt'

try:
    # Open the file in read mode
    with open(file_path, 'r') as file:
        # Read all lines from the file
        content = file.read()
        
        # Print the content
        print("Content of the file:")
        print(content)

except FileNotFoundError:
    print(f"Error: The file '{file_path}' does not exist.")
except IOError:
    print(f"Error: Failed to read the file '{file_path}'.")

    # Writing a list of strings to a file

lines_to_write = [
    "This is line 1.",
    "This is line 2.",
    "This is line 3."
]

output_file_path = 'output.txt'

try:
    # Open the file in write mode
    with open(output_file_path, 'w') as file:
        # Write each line from the list to the file
        for line in lines_to_write:
            file.write(line + "\n")

    print(f"Successfully wrote {len(lines_to_write)} lines '{output_file_path}'.")

except IOError:
    print(f"Error: Failed to write to the file '{output_file_path}'.")

    references:
    geeksforgeeks: https://www.geeksforgeeks.org/getting-started-with-python-programming/?ref=shm



# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


