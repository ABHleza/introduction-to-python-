# introduction-to-python-
Python
# Define a function for each mathematical operation
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error! Division by zero is not allowed."
    else:
        return x / y

# Take user input for numbers and operation
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
operation = input("Enter operation (+, -, *, /): ")

# Perform operation based on user input
if operation == "+":
    result = add(num1, num2)
    print(f"{num1} + {num2} = {result}")
elif operation == "-":
    result = subtract(num1, num2)
    print(f"{num1} - {num2} = {result}")
elif operation == "*":
    result = multiply(num1, num2)
    print(f"{num1} * {num2} = {result}")
elif operation == "/":
    result = divide(num1, num2)
    if isinstance(result, str):
        print(result)
    else:
        print(f"{num1} / {num2} = {result}")
else:
    print("Invalid operation! Please try again.")
