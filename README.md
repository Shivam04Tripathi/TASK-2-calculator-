# TASK-2-calculator-
def simple_calculator():
    print("Simple Calculator")
    print("Choose an operation:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")

    try:
    
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        
    
        operation = input("Enter the operation (+, -, *, /): ")

    
        if operation == '+':
            result = num1 + num2
            print(f"Result: {num1} + {num2} = {result}")
        elif operation == '-':
            result = num1 - num2
            print(f"Result: {num1} - {num2} = {result}")
        elif operation == '*':
            result = num1 * num2
            print(f"Result: {num1} * {num2} = {result}")
        elif operation == '/':
            if num2 != 0:
                result = num1 / num2
                print(f"Result: {num1} / {num2} = {result}")
            else:
                print("Error: Cannot divide by zero.")
        else:
            print("Invalid operation. Please enter one of +, -, *, or /.")

    except ValueError:
        print("Invalid input. Please enter numeric values for numbers.")

simple_calculator()






OUTPUT 


Enter the first number: 10
Enter the second number: 5
Enter the operation : +
Result: 10.0 + 5.0 = 15.0




