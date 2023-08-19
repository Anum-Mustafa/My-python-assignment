# My-python-assignment
# 1. Write a Python program to print the following string in a specific format (see the
# output).

# Twinkle, twinkle, little star,
# How I wonder what you are!
# Up above the world so high,
# Like a diamond in the sky.

# Twinkle, twinkle, little star,
# How I wonder what you are

print("Twinkle, twinkle, little star,")
print("How I wonder what you are!")
print("Up above the world so high,")
print("Like a diamond in the sky.")
print()
print("Twinkle, twinkle, little star,")
print("How I wonder what you are")


# 2. Write a Python program to get the Python version you are using

import sys

print("Python version:")
print(sys.version)
print("Version info:")
print(sys.version_info)


# 3. Write a Python program to display the current date and time.

import datetime

now = datetime.datetime.now()
print("Current date and time:")
print(now)


# 4. Write a Python program which accepts the radius of a circle from the user and compute
# the area.

import math

radius = float(input("Enter the radius of the circle: "))
area = math.pi * (radius ** 2)
print("The area of the circle is:", area)

# 5. Write a Python program which accepts the user's first and last name and print them in
# reverse order with a space between them.

first_name = input("Enter your first name: ")
last_name = input("Enter your last name: ")

reversed_name = last_name + " " + first_name
print("Reversed name:", reversed_name)

# 6. Write a python program which takes two inputs from user and print them addition

num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
sum_nums = num1 + num2
print("Sum:", sum_nums)

# 7. Write a program which takes 5 inputs from user for different subject’s marks, total it
# and generate mark sheet using grades ?

subject_marks = []
for i in range(5):
    marks = int(input(f"Enter marks for subject {i + 1}: "))
    subject_marks.append(marks)

total_marks = sum(subject_marks)
average_marks = total_marks / len(subject_marks)

if average_marks >= 90:
    grade = "A"
elif average_marks >= 80:
    grade = "B"
elif average_marks >= 70:
    grade = "C"
elif average_marks >= 60:
    grade = "D"
else:
    grade = "F"

print("Total Marks:", total_marks)
print("Average Marks:", average_marks)
print("Grade:", grade)


# 8. Write a program which take input from user and identify that the given number is even
# or odd?

number = int(input("Enter a number: "))
if number % 2 == 0:
    print("Even")
else:
    print("Odd")


# 9. Write a program which print the length of the list?

my_list = [1, 2, 3, 4, 5]
length = len(my_list)
print("Length of the list:", length)

# 10.Write a Python program to sum all the numeric items in a list?

num_list = [1, 2, 3, 4, 5]
total_sum = sum(num_list)
print("Sum of numeric items in the list:", total_sum)

# 11.Write a Python program to get the largest number from a numeric list.
num_list = [10, 24, 6, 45, 78, 5, 90]
largest_num = max(num_list)
print("Largest number:", largest_num)

# 12. Take a list, say for example this one:
# a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
# Write a program that prints out all the elements of the list that are less than 5.

a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
for num in a:
    if num < 5:
        print(num)


# ASSIGNMENT NO 04
# 1. Make a calculator using Python with addition , subtraction ,
# multiplication ,division and power.

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Cannot divide by zero"

def power(x, y):
    return x ** y

print("Select operation:")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")
print("5. Power")

choice = input("Enter choice (1/2/3/4/5): ")

num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

if choice == '1':
    print("Result:", add(num1, num2))
elif choice == '2':
    print("Result:", subtract(num1, num2))
elif choice == '3':
    print("Result:", multiply(num1, num2))
elif choice == '4':
    print("Result:", divide(num1, num2))
elif choice == '5':
    print("Result:", power(num1, num2))
else:
    print("Invalid input")


# 2. Write a program to check if there is any numeric value in list using for
# loop.

my_list = [1, 'a', 3.14, 'hello', 5]

for item in my_list:
    if isinstance(item, (int, float)):
        print(f"{item} is a numeric value")


# 3. Write a Python script to add a key to a dictionary.

my_dict = {'a': 1, 'b': 2, 'c': 3}

key = input("Enter key: ")
value = input("Enter value: ")

my_dict[key] = value

print("Updated dictionary:", my_dict)



# 4. Write a Python program to sum all the numeric items in a dictionary.

my_dict = {'a': 10, 'b': 20, 'c': 'hello', 'd': 30}

total_sum = 0
for key, value in my_dict.items():
    if isinstance(value, (int, float)):
        total_sum += value

print("Sum of numeric items in the dictionary:", total_sum)


# 5. Write a program to identify duplicate values from list.

my_list = [1, 2, 3, 2, 4, 5, 3, 6, 7, 8, 4]

unique_items = set()
duplicate_items = set()

for item in my_list:
    if item in unique_items:
        duplicate_items.add(item)
    else:
        unique_items.add(item)

print("Duplicate values:", duplicate_items)


# 6. Write a Python script to check if a given key already exists in a
# dictionary

my_dict = {'a': 1, 'b': 2, 'c': 3}

key = input("Enter key to check: ")

if key in my_dict:
    print(f"The key '{key}' exists in the dictionary.")
else:
    print(f"The key '{key}' does not exist in the dictionary.")

