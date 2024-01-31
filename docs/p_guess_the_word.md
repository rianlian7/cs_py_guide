# Project: Guess the word

## Step 1: Set up the basic structure

In this step, we're getting ready to play a game called "Guess the Word." 

We're selecting a word randomly from a list of words related to computer science and printing it out. 

This is the word that the player will try to guess. 

We also create an empty list to keep track of the letters the player has guessed.

    from random import randint

    print("Welcome to Guess the Word!")
    words = ["cat", "dog", "cow", "chicken", "pig", "piglet", "hamster"]
    randomWord = wordList[randint(0, len(wordList)-1)]
    print(f"Word to guess: {word_to_guess}")


## Step 2: Display underscores for each letter in the word

Now, we want to show the player how many letters are in the word they need to guess. We use underscores "_" to represent each letter in the word. This step helps the player understand how long the word is, but we haven't revealed any actual letters yet.

    display = ""
    for letter in word_to_guess:
        if letter in guessed_letters:
            display += letter
        else:
            display += "_"

    print(display)

## Step 3: Take user input for guessing a letter

It's time for the player to make a guess! We ask the player to type in a letter, and whatever letter they type, we add it to the list of guessed letters. This is their attempt to figure out the secret word.

    guess = input("Guess a letter: ")
    guessed_letters.append(guess)

## Step 4: Check if the guessed letter is in the word

Now, we check if the letter the player guessed is actually in the secret word. If it is, we tell them it's a "Good guess!" If not, we encourage them to "Try again!" This step helps the player understand if they are moving closer to guessing the word.

    if guess in word_to_guess:
        print("Good guess!")
    else:
        print("Try again!")


![type:video](https://www.youtube.com/embed/LXb3EKWsInQ)
