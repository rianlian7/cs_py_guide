# Number Guessing Game

## Introduction

In this guide, you will learn how to create a simple number guessing game using Python.

## Step 1: Set Up the Game

First, let's set up the game by defining the minimum and maximum values for the range of numbers to guess.

    # Define the range of numbers
    min_number = 1
    max_number = 100

## Step 2: Generate the Random Number

Next, generate a random number within the defined range for the player to guess.

    import random

    # Generate a random number
    secret_number = random.randint(min_number, max_number)

## Step 3: Prompt the User for Guesses
Prompt the user to guess the number and provide feedback on whether the guess is too high, too low, or correct.

    # Prompt the user to guess the number
    guess = int(input(f"Guess a number between {min_number} and {max_number}: "))

    # Check if the guess is correct
    if guess == secret_number:
        print("Congratulations! You guessed the number correctly!")
    elif guess < secret_number:
        print("Too low! Try again.")
    else:
        print("Too high! Try again.")


## Step 4: Repeat until correct guess

Repeat the guessing process until the user correctly guesses the secret number.

Add a *while* statement before the *if* statement. Make sure to **indent** your code below the while statement.

    # Repeat until correct guess
    while guess != secret_number:


## Final Code

    import random

    # Define the range of numbers
    min_number = 1
    max_number = 100

    # Generate a random number
    secret_number = random.randint(min_number, max_number)

    # Prompt the user to guess the number
    guess = int(input(f"Guess a number between {min_number} and {max_number}: "))


    # Repeat until correct guess
    while guess != secret_number:
        guess = int(input("Try again: "))
        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print("Congratulations! You guessed the number correctly!")


## Challenges

1. Limited Attempts: Modify the game to allow the player only a certain number of attempts to guess the number before revealing the correct answer. (2HP)

2. Difficulty Levels: Implement different difficulty levels (e.g., easy, medium, hard) where the range of numbers to guess from varies accordingly. (3HP)