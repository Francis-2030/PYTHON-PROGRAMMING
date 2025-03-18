def add(x, y):
    return x + y
def subtract(x, y):
    return x - y
def multiply(x, y):
    return x * y
def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    else:
        return x / y
def calculator():
    try:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        operation = input("Enter the operation (+, -, *, /): ")
        
        if operation == '+':
            addition = num1 + num2
            print(f"The result of addition is: {addition}")
        elif operation == '-':
            sub = num1 - num2
            print(f"The result of subtraction is: {sub}")
        elif operation == '*':
            mult = num1 * num2
            print(f"The result of multiplication is: {mult}")
        elif operation == '/':
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
            else:
                div = num1 / num2
                print(f"The result of division is: {div}")
        else:
            print("Invalid operation. Please enter +, -, *, or /.")
    except ValueError:
        print("Invalid input. Please enter numerical values.")

calculator()
