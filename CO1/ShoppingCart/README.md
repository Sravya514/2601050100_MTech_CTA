
# Shopping Cart

## Description

This project contains a Python program that implements a simple **Shopping Cart** system. It allows users to add products to a cart, manage the items, and calculate the total price.

## Algorithm

The script manages the cart using basic data structures (like lists or dictionaries). The step-by-step algorithm is as follows:

1. **Initialize:** Create an empty list or dictionary to represent the shopping cart.
2. **Add Items:** When a user adds an item, capture the item's name, price, and quantity. Append this data as a record to the cart structure.
3. **View Cart:** Iterate through the cart data structure and display each item's name, price, quantity, and subtotal.
4. **Calculate Total:** 
   * Initialize a `total_cost` variable to 0.
   * Loop through each item currently in the cart.
   * Multiply the item's price by its quantity and add it to `total_cost`.
5. **Output:** Return or print the final `total_cost` and a summary of the cart.
### Input


Enter product: Apple

Enter quantity: 2


### Output


Product added to cart.

Total: 100

