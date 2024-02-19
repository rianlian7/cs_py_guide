# Max Min Average

## Step 1: Set up the List of marks

- Begin by defining a list of marks for the class

        # Define the list of marks for the class
        marks = [75, 92, 98, 40, 50, 48, 92, 14, 58]

## Step 2: Initialise variables

Initialize variables for the total, maximum mark, minimum mark, and class size.

    # Initialize variables
    total = 0
    max_mark = marks[0]  # Accessing the first element in the list marks
    min_mark = marks[0]  # Accessing the first element in the list marks
    class_size = len(marks)  # Getting the number of elements in the list marks

- Accessing the Array (**marks[0]**):

    - marks[0] accesses the first element in the list marks.
    - In Python, list index start from 0, so marks[0] refers to the first element.

- Using the **len()** Function:
    - len(marks) returns the number of elements in the list marks.
    - The len() function is a built-in Python function used to get the length or number of items in a sequence like lists, tuples, strings, etc.

## Step 3: Find maximum and minimum marks

- Iterate through the list of marks to find the maximum and minimum marks.

        # Find maximum and minimum marks
        for mark in marks:
            if mark > max_mark:
                max_mark = mark
            if mark < min_mark:
                min_mark = mark

## Step 4: Calculate Total

- Calculate the total of all marks in teh class.

        # Calculate total
        for mark in marks:
            total += mark

## Step 5: Calculate Average

- Calculate the average mark of the class.

        # Calculate average
        average = total / class_size


## Step 6: Display results

- Display the maximum, minimum, and average marks.

        print("Maximum Mark:", max_mark)
        print("Minimum Mark:", min_mark)
        print("Average Mark:", average)


## Final Code

        # Define the list of marks for the class
        marks = [75, 92, 98, 40, 50, 48, 92, 14, 58]

        # Initialize variables
        total = 0
        max_mark = 0
        min_mark = 100
        class_size = len(marks)

        # Find maximum and minimum marks
        for mark in marks:
            if mark > max_mark:
                max_mark = mark
            if mark < min_mark:
                min_mark = mark

        # Calculate total
        for mark in marks:
            total += mark

        # Calculate average
        average = total / class_size

        # Display results
        print("Maximum Mark:", max_mark)
        print("Minimum Mark:", min_mark)
        print("Average Mark:", average)
