# Bubble Sort

## Step 1: Set up the list of numeric data.

- Begin by defining a list of numeric data to be sorted.

        # Define the list of numeric data
        data = [8, 5, 2, 9, 3, 6, 1, 4, 7]

## Step 2: Implement Bubble Sort

    # Set the first index of the data list
    first = 0

    # Set the last index of the data list
    last = len(data)

    # Start the bubble sort loop
    while True:
        # Initialize a variable to track whether a swap has occurred
        swap = False
        
        # Iterate through the data list
        for index in range(first, last - 1):
            # Compare adjacent elements and swap them if necessary
            if data[index] > data[index + 1]:
                temp = data[index]       # Store the value of the current element in a temporary variable
                data[index] = data[index + 1]  # Replace the current element with the next element
                data[index + 1] = temp   # Replace the next element with the stored value
                swap = True             # Set swap flag to indicate that a swap occurred
        
        # Move the last index one step to the left
        last -= 1
        
        # Check if a swap has occurred or if the last index has reached the first index
        if not swap or last == 1:
            break   # Exit the loop if no swap occurred or if the last index is equal to the first index


## Step 3: Display sorted data

- Display the sorted data after applying the Bubble Sort algorithm.

        # Display sorted data
        print("Sorted Data:", data)


## Step 4: Test the code

- Run the code, it should return a list of number in ascending order.

## Final Code

    # Define the list of numeric data
    data = [8, 5, 2, 9, 3, 6, 1, 4, 7]

    # Implement Bubble Sort
    first = 0
    last = len(data)
    while True:
        swap = False
        for index in range(first, last - 1):
            if data[index] > data[index + 1]:
                temp = data[index]
                data[index] = data[index + 1]
                data[index + 1] = temp
                swap = True
        last -= 1
        if not swap or last == 1:
            break

    # Display sorted data
    print("Sorted Data:", data)
