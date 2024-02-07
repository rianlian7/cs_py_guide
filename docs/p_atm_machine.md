# Project: ATM Machine

Always read and try out your code each step.

## Step 1: Set Up the Basic Structure

The first step of the ATM machine is to display the options for users to choose. Write the following code below.

    # Initialize balance
    balance = 0

    # Function to display options
    def display_options():
        print("Select an option:")
        print("1. Check Balance")
        print("2. Deposit")
        print("3. Withdraw")
        print("4. Exit")

## Step 2: Getting the user input

Now, let's add the code to get input from the user within an infinite loop.

    # Start an infinite loop to keep the ATM running until the user chooses to exit
    while True:
        # Display options to the user
        display_options()

        # Get user choice
        choice = input("Enter choice (1-4): ")

## Step 3: Output the balance

When the user selects the option to check balance, we need to output the current balance.

    # Check user's choice
    if choice == '1':
        print("Your balance is: $", balance)

## Step 4: Deposit

If the user chooses to deposit money, we need to prompt for the deposit amount and update the balance.

    elif choice == '2':
        deposit_amount = float(input("Enter deposit amount: $"))
        balance += deposit_amount
        print("Deposit successful.")

## Step 5: Withdraw

For withdrawal, prompt for the withdrawal amount and update the balance, checking for sufficient funds.

    elif choice == '3':
        withdraw_amount = float(input("Enter withdrawal amount: $"))
        if withdraw_amount <= balance:
            balance -= withdraw_amount
            print("Withdrawal successful.")
        else:
            print("Insufficient funds.")


## Step 6: Error Checking

Finally, we need to handle invalid user input by displaying an error message.

    else:
        print("Invalid choice. Please enter a number between 1 and 4.")


## Challenges

1. Add a PIN system. Before the options are displayed to the user, get the user to enter their pin. You may create a variable to store the PIN number (1HP).
1. Add an option for converting different currency type (2HP).
1. Add an algorithm to record down every transaction into an array(list) and add an option for user to pick to show their transaction history. (3HP)


Send your full code to my chat for me to check and claim your house point.