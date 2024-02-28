# Shakespeare Insult Generator

This project involves creating a program that generates random insults inspired by the language of Shakespeare.

## Step 1: Set Up the Basic Structure

The first step is to import necessary modules and define lists of words for generating insults with a Shakespearean twist.

    import random

    adjectives = ['base-court', 'villainous', 'bootless', 'fusty']
    nouns = ['swag-bellied', 'flap-mouthed', 'hedge-born', 'milk-livered', 'canker-blossom']

## Step 2: Generate Insult Function

A **function** is a reusable block of code that performs a specific task. 

It always starts with the keyword **def** followed by the function name. 

For example: 
**def generate_insult():**

Where **def** is the keyword to create function and **generate_insult()** is the function name.

The indented code below it is the block of code that will run when we call the function in the next step. We can run this block of code anytime by calling the function

Create a function to generate insults by randomly selecting adjectives and nouns from the lists.

    def generate_insult():
        adjective = random.choice(adjectives)
        noun = random.choice(nouns)
        return f"Thou {adjective} {noun}!"


## Step 3: Get User Input

Allow the user to input the number of insults they want to generate.

    num_insults = int(input("Enter the number of insults to generate: "))

## Step 4: Generate Insults

Generate the specified number of insults and display them to the user.

    for _ in range(num_insults):
        print(generate_insult())


## Final Code

    import random

    adjectives = ['base-court', 'villainous', 'bootless', 'fusty']
    nouns = ['swag-bellied', 'flap-mouthed', 'hedge-born', 'milk-livered', 'canker-blossom']

    def generate_insult():
        adjective = random.choice(adjectives)
        noun = random.choice(nouns)
        return f"Thou {adjective} {noun}!"

    num_insults = int(input("Enter the number of insults to generate: "))

    for _ in range(num_insults):
        print(generate_insult())

## Challenges

1. Search for more adjectives and nouns to expand your list. (1HP)
1. Change the adjectives and nouns to other style of insults such as Irish or Elizabethan-era. (1HP)