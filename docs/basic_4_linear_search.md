# Linear Search

## Step 1: Set up the list of names

    # Define the list of names
    names = ["Alice", "Bob", "Charlie", "David", "Eva", "Frank"]

## Step 2: Input name to find

    # Prompt the user to enter the name to find
    name_to_find = input("Enter name to find: ")

## Step 3: Initilise counter and boolean variables

Initialize Variables:

- **found** is a *boolean* variable that indicates whether the name has been found in the list.
- **counter** is an *integer* variable that keeps track of the current position in the list while searching.

        # Initialize variables
        found = False
        counter = 0


## Step 4: Perform linear search
- Start a while loop to iterate through each element of the list.
- The loop continues as long as the counter is less than the length of the list (len(names)) and found is False.

Inside the loop:

- Check if the name at the current position (names[counter]) matches the name the user wants to find (name_to_find).
- If there's a match, set found to True to indicate that the name has been found.
- If there's no match, increment counter by 1 to move to the next element in the list.

        # Perform linear search
        while counter < len(names) and not found:
            if names[counter] == name_to_find:
                found = True
            else:
                counter += 1

## Step 5: Output Result

    # Output result
    if found:
        print(name_to_find, "found")
    else:
        print(name_to_find, "not found")

## Step 6: Test code

1. Run the code.
2. In the console screen, it should show "Enter name to find:"
3. Enter the name "David".
4. Press **Enter**

The code should output, "David found". 

Then try testing the code with other names.

## Final Code

    # Define the list of names
    names = ["Alice", "Bob", "Charlie", "David", "Eva", "Frank"]

    # Prompt the user to enter the name to find
    name_to_find = input("Enter name to find: ")

    # Initialize variables
    found = False
    counter = 0

    # Perform linear search
    while counter < len(names) and not found:
        if names[counter] == name_to_find:
            found = True
        else:
            counter += 1

    # Output result
    if found:
        print(name_to_find, "found")
    else:
        print(name_to_find, "not found")
