import math
import cmath
# Basic Arithmetic Operations
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
        return "Error! Division by zero."

# Exponentiation
def exponentiate(x, y):
    return x ** y

# Square Root (real and complex support)
def sqrt(x):
    if x >= 0:
        return math.sqrt(x)
    else:
        return cmath.sqrt(x)

# Factorial (only non-negative integers)
def factorial(x):
    if x >= 0 and x == int(x):
        return math.factorial(int(x))
    else:
        return "Error! Factorial is only defined for non-negative integers."

# Logarithms
def log_base_10(x):
    if x > 0:
        return math.log10(x)
    else:
        return "Error! Logarithm is defined for positive numbers."

def natural_log(x):
    if x > 0:
        return math.log(x)
    else:
        return "Error! Natural logarithm is defined for positive numbers."

# Trigonometric functions (input in radians)
def sin_func(x):
    return math.sin(x)

def cos_func(x):
    return math.cos(x)

def tan_func(x):
    try:
        return math.tan(x)
    except:
        return "Error! Undefined value for tan."

# Convert degrees to radians for user convenience
def degrees_to_radians(deg):
    return math.radians(deg)

# Operations with complex numbers
def complex_add(x, y):
    return x + y

def complex_subtract(x, y):
    return x - y

def complex_multiply(x, y):
    return x * y

def complex_divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error! Division by zero."

def display_menu():
    print("\nSelect operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exponentiation")
    print("6. Square Root")
    print("7. Factorial")
    print("8. Logarithm (base 10)")
    print("9. Natural Logarithm")
    print("10. Sin")
    print("11. Cos")
    print("12. Tan")
    print("13. Complex Addition")
    print("14. Complex Subtraction")
    print("15. Complex Multiplication")
    print("16. Complex Division")

# Main loop to handle user input and calculate results
def calculator():
    while True:
        display_menu()
        
        choice = input("\nEnter choice (1-16), or 'q' to quit: ")

        if choice == 'q':
            print("Exiting Calculator. Goodbye!")
            break

        # Basic arithmetic operations
        if choice in ['1', '2', '3', '4', '5']:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            if choice == '1':
                print(f"Result: {add(num1, num2)}")
            elif choice == '2':
                print(f"Result: {subtract(num1, num2)}")
            elif choice == '3':
                print(f"Result: {multiply(num1, num2)}")
            elif choice == '4':
                print(f"Result: {divide(num1, num2)}")
            elif choice == '5':
                print(f"Result: {exponentiate(num1, num2)}")

        # Square root
        elif choice == '6':
            num = float(input("Enter a number: "))
            print(f"Square Root: {sqrt(num)}")

        # Factorial
        elif choice == '7':
            num = int(input("Enter a non-negative integer: "))
            print(f"Factorial: {factorial(num)}")

        # Logarithms
        elif choice == '8':
            num = float(input("Enter a positive number: "))
            print(f"Log10: {log_base_10(num)}")
        elif choice == '9':
            num = float(input("Enter a positive number: "))
            print(f"Natural Log: {natural_log(num)}")

        # Trigonometric operations
        elif choice in ['10', '11', '12']:
            deg = float(input("Enter angle in degrees: "))
            rad = degrees_to_radians(deg)
            if choice == '10':
                print(f"sin({deg}) = {sin_func(rad)}")
            elif choice == '11':
                print(f"cos({deg}) = {cos_func(rad)}")
            elif choice == '12':
                print(f"tan({deg}) = {tan_func(rad)}")

        # Complex number operations
        elif choice in ['13', '14', '15', '16']:
            real1 = float(input("Enter real part of first complex number: "))
            imag1 = float(input("Enter imaginary part of first complex number: "))
            real2 = float(input("Enter real part of second complex number: "))
            imag2 = float(input("Enter imaginary part of second complex number: "))
            num1 = complex(real1, imag1)
            num2 = complex(real2, imag2)
            if choice == '13':
                print(f"Result: {complex_add(num1, num2)}")
            elif choice == '14':
                print(f"Result: {complex_subtract(num1, num2)}")
            elif choice == '15':
                print(f"Result: {complex_multiply(num1, num2)}")
            elif choice == '16':
                print(f"Result: {complex_divide(num1, num2)}")

        else:
            print("Invalid input! Please choose a valid option.")

if __name__ == "__main__":
    calculator()
