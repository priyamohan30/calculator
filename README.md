# calculator
This is my first repository.
<br>
Author = Priyanka
# Simple Calculator in Python

# This function adds two numbers
def add(x, y):
    return x + y

# This function subtracts two numbers
def subtract(x, y):
    return x - y

# This function multiplies two numbers
def multiply(x, y):
    return x * y

# This function divides two numbers
def divide(x, y):
    # Check if denominator is zero
    if y == 0:
        return "Error! Division by zero."
    else:
        return x / y

# This function is for floor division
def floordivision(x,y):
    # Check if denominator is zero
    if y == 0:
        return "Error! Division by zero."
    else:
        return x // y

# Display menu for user input
print("Select operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")
print("5.Floor division")

# Take input from the user
choice = input("Enter choice (1/2/3/4/5): ")

# Ask for numbers
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Perform calculation based on user choice
if choice == '1':
    print("Result:", add(num1, num2))
elif choice == '2':
    print("Result:", subtract(num1, num2))
elif choice == '3':
    print("Result:", multiply(num1, num2))
elif choice == '4':
    print("Result:", divide(num1, num2))
elif choice == '5':
    print("Result:",floordivision(num1,num2))
else:
    print("Invalid input")
