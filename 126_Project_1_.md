#this function is to add two numbers
def addition(a, b):
    return a + b
#this function is to subtract two numbers
def subtraction(a, b):
    return a - b
#this function is to multiply two numbers
def multiplication(a, b):
    return a * b
#this function is to divide two numbers
def division(a, b):
    return a / b

#this is what the user will see in the start of the application
print("Please select an operation.")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")

#this is where we take the user input in the application
while True:
#checks if user's choice is one of the four operations 
    user_choice = input("Pick an operation(1, 2, 3, 4): ")
    if user_choice in ('1', '2', '3', '4'):
        number_1 = float(input("Please enter the first number: "))
        number_2 = float(input("Please enter the second number: "))
#print accordingly based on user's input of numbers and desired operation
        if user_choice == '1':
            print(number_1, "+", number_2, "=", addition(number_1, number_2))

        elif user_choice == '2':
            print(number_1, "-", number_2, "=", subtraction(number_1, number_2))

        elif user_choice == '3':
            print(number_1, "*", number_2, "=", multiplication(number_1, number_2))

        elif user_choice == '4':
            print(number_1, "/", number_2, "=", division(number_1, number_2))
        break
    else:
        print("Input Error, Please try a different operation. ")


