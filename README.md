# ViLearnX-Task-2
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

    def main():
        print("Welcome")
    
    
    try:
        a = float(input("Enter the first number: "))
        b = float(input("Enter the second number: "))
    except ValueError:
        print("Invalid input.")
        return

    
    print("\nSelect operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    choice = input("Enter choice (1/2/3/4): ")

    # Operation Execution and Result Display
    if choice == '1':
        result = add(a, b)
        operation = "addition"
    elif choice == '2':
        result = subtract(a, b)
        operation = "subtraction"
    elif choice == '3':
        result = multiply(a, b)
        operation = "multiplication"
    elif choice == '4':
        result = divide(a, b)
        operation = "division"
    else:
        print("Invalid choice! Please select a valid operation.")
        return
    
    # Display Result
    print(f"\nThe result of {operation} between {a} and {b} is: {result}")

    if __name__ == "__main__":
        main()
