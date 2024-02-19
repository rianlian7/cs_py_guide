# Counting

## Problem Statement
We are building an algorithm to counts the number of players whose score is over 50.

## Step 1: Set Up the List of Player Scores

- Begin by defining a list of player scores.

        player_scores = [53, 23, 60, 45, 80, 100, 40, 38, 54]


## Step 2: Count players score over 50

- Initialize a counter variable to keep track of the number of player scores over 50. 
- Then, iterate through the list of player scores and increment the counter for each score over 50.

        # Initialize counter for player scores over 50
        count_over_50 = 0

        # Count player scores over 50
        for score in player_scores:
            if score > 50:
                count_over_50 += 1

## Step 3: Display the Count of Player Scores Over 50

- Display the count of player scores over 50.

        # Display count of player scores over 50
        print("Number of player scores over 50:", count_over_50)


## Final Code

    # Define the list of player scores
    player_scores = [75, 92, 83, 88, 97, 85]

    # Initialize counter for player scores over 50
    count_over_50 = 0

    # Count player scores over 50
    for score in player_scores:
        if score > 50:
            count_over_50 += 1

    # Display count of player scores over 50
    print("Number of player scores over 50:", count_over_50)

