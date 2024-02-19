# Totalling

## Step 1: Set Up the Basic Structure
- Initialize a variable total_price to keep track of the total price of all the items purchased.
- Use the assignment operator = to assign the value 0 to the variable total_price.

        # Set up basic structure
        total_price = 0

## Step 2: List of item prices

- We are provided with a list of item prices.

        # List of item prices
        item_prices = [10.99, 5.75, 8.50, 12.25, 6.99]

## Step 3: Iterate through the loop
-  We use a **for loop** to iterate through each item price in the list and add it to the *total_price* variable.

        # Iterate through each item price in the list
        for price in item_prices:
            total_price += price

## Step 4: Display the total price
- Display the calculated total price to the user using the print() function.

        # Display the total price
        print("Total price: $", total_price)

## Final Code

    # Set up basic structure
    total_price = 0

    # List of item prices
    item_prices = [10.99, 5.75, 8.50, 12.25, 6.99]

    # Iterate through each item price in the list
    for price in item_prices:
        total_price += price

    # Display the total price
    print("Total price: $", total_price)

