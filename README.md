# CODETECH-Task1

def add(x, y):
    return x + y


def subtract(x, y):
    return x - y


def multiply(x, y):
    return x * y


def divide(x, y):
    return x / y

print("Welcome to Mini Calcys world!")

while True:
   
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))

    
    print("\nOperations:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    
    choice = input("\nEnter your choice (1/2/3/4): ")

   
    if choice == '1':
        print(f"\n{num1} + {num2} = {add(num1, num2)}")
    elif choice == '2':
        print(f"\n{num1} - {num2} = {subtract(num1, num2)}")
    elif choice == '3':
        print(f"\n{num1} * {num2} = {multiply(num1, num2)}")
    elif choice == '4':
        
        if num2 != 0:
            print(f"\n{num1} / {num2} = {divide(num1, num2)}")
        else:
            print("\nError: Division by zero")
    else:
        print("\nInvalid input")

    
    restart = input("\nDo you want to perform another calculation? (1/0): ").lower()
    if restart != '1':
        break
    print("--------------------------------------------------------------")

print("\nThank you for using Mini Calcy!")
