# Project: Calculator

## Step 1: Set Up the Basic Structure

In this step, we'll create the basic structure of our calculator program. This includes defining variables and setting up the main loop to repeatedly take user input.

    # Start an infinite loop to keep the calculator running until the user chooses to exit
    while True:
        # Display options to the user
        print("Select operation:")
        print("1. Add")
        print("2. Subtract")
        print("3. Multiply")
        print("4. Divide")
        print("5. Exit")

        # Get user choice
        choice = input("Enter choice (1-5): ")
        
        # Check if the user wants to exit
        if choice == '5':
            print("Exiting the calculator. Goodbye!")
            break

## Step 2: Get User Input and Perform Addition

Now, let's implement the addition functionality. We'll take two numbers as input from the user, add them, and display the result.

    elif choice == '1':
        # Get two numbers from the user
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        
        # Add the two numbers and display the result
        result = num1 + num2
        print("Result: ", result)

## Step 3: Implement Subtraction
Extend the program to handle subtraction. Take two numbers as input, subtract them, and display the result.

    elif choice == '2':
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        result = num1 - num2
        print("Result: ", result)

## Step 4: Implement Multiplication
Add functionality for multiplication. Take two numbers as input, multiply them, and display the result.

    elif choice == '3':
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        result = num1 * num2
        print("Result: ", result)

## Step 5: Implement Division
Extend the program to handle division. Take two numbers as input, perform the division, and display the result. Also, handle division by zero.

    elif choice == '4':
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
        
        # Check for division by zero
        if num2 != 0:
            result = num1 / num2
            print("Result: ", result)
        else:
            print("Error: Division by zero.")

## Step 6: Exit the Program
If the user chooses to exit (option 5), print a goodbye message and break out of the loop to end the program.

    elif choice == '5':
        print("Exiting the calculator. Goodbye!")
        break

<br>

## Challenges

Congratulations, you now have a simple calculator application! Now, to improve your calculator further, try to modify your code so that:

1. User can decide how many numbers to perform the mathematical operations. (1HP)
2. Instead of asking the users to enter the first or second number. Use string handling skills to allow user to input the whole formulae in one input. For example: user enters "2+2", then your program will output 4.(5HP)