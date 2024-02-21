# Project: Parcel Checking

The Parcel project is a Python program that:

- Prompts users to input the weight of a parcel.
- Displays a menu of delivery options.
- Calculates the cost of shipping based on the chosen delivery option.
- Outputs the calculated cost to the user.

## Step 1: Check Parcel Weight

Prompt the user to enter the weight of the parcel.

    # Check parcel weight
    weight = float(input("Enter the weight of the parcel (in kg): "))

    if weight >= 0.5 and weight <= 5.0:
        # Display delivery options

## Step 2: Display Delivery Options

Display a menu of delivery options for the user to choose from.

    print("Select a delivery option:")
    print("1. Guaranteed next day delivery before noon")
    print("2. Guaranteed next day delivery")
    print("3. 24-hour delivery")
    print("4. 48-hour delivery")
    print("5. 3-5 days delivery")


## Step 3: Get the user's choice of delivery option.

Get the user's choice of delivery option.

    # Get user choice
    choice = int(input("Enter choice (1-5): "))

## Step 4: Calculate the cost

Based on the user's choice of delivery option, calculate the cost of delivery.
    cost = 0
    # Calculate cost based on delivery option
    if choice == 1:
        cost = weight * 10 + 1
    elif choice == 2:
        cost = weight * 10
    elif choice == 3:
        cost = 5
    elif choice == 4:
        cost = 4
    elif choice == 5:
        cost = 3
    else:
        print("Invalid choice. Please select a valid delivery option.")

## Step 5: Output the cost

    # Display cost
    print("The cost of delivery is: $", cost)

After completing all the steps, the code will function as a parcel checking program, allowing users to input the weight of a parcel and select a delivery option to calculate the cost.


## Final code

    # Check parcel weight
    weight = float(input("Enter the weight of the parcel (in kg): "))

    if weight >= 0.5 and weight <= 5.0:
        # Display delivery options
        print("Select a delivery option:")
        print("1. Guaranteed next day delivery before noon")
        print("2. Guaranteed next day delivery")
        print("3. 24-hour delivery")
        print("4. 48-hour delivery")
        print("5. 3-5 days delivery")

        # Get user choice
        choice = int(input("Enter choice (1-5): "))
        
        cost = 0
        # Calculate cost based on delivery option
        if choice == 1:
            cost = weight * 10 + 1
        elif choice == 2:
            cost = weight * 10
        elif choice == 3:
            cost = 5
        elif choice == 4:
            cost = 4
        elif choice == 5:
            cost = 3
        else:
            print("Invalid choice. Please select a valid delivery option.")

        # Display cost
        print("The cost of delivery is: $", cost)
    else:
        print("Parcel is rejected")



## Challenges

1. **Loop**: After the program ends, ask the user if they want to do another parcel check. (1HP)

1. **Add additional delivery options**: Expand the program to include more delivery options, such as international shipping or express delivery. (1HP)

1. **Discounts**: Introduce discount codes or loyalty rewards that can be applied to reduce the cost of delivery. (2HP)

