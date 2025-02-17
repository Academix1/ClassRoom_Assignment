# Hackathon Assignment: Inventory and Shopping Cart System

## Introduction

The Inventory and Shopping Cart System is a simple e-commerce application that allows users to manage a shopping cart, view available products, add products to the cart, and complete the checkout process. The system supports basic inventory management, user management, and transaction tracking. It also provides features for clearing the cart and removing items, offering a flexible shopping experience.

## Features

1. **View Products**:
   - Users can view a list of available products with details such as product name, price, quantity available, and discount.

2. **Add to Cart**:
   - Users can add products to their shopping cart, specifying the quantity they wish to purchase.
   - The system ensures that the requested quantity is available in stock.

3. **Checkout**:
   - Users can proceed to checkout where the system calculates the total cost including an additional GST of 18%.
   - If the user’s balance is insufficient to complete the transaction, the system prevents the checkout and notifies the user.
   - A successful checkout updates the user’s balance and records the transaction.
   - Upon successful payment, the shopping cart is cleared.

4. **Clear Cart**:
   - Users can view the products currently in their cart and remove some or all of the products.
   - The cart updates in real-time, and users are asked to specify the quantity of items to remove.
   - If a user decides to remove a product entirely, it will be completely removed from the cart.

5. **User Management**:
   - Users are registered with an initial balance and can have multiple transactions recorded in their history.
   - The user’s shopping cart and transaction history are stored and updated throughout the shopping process.

## Functionality Flow

### 1. User Initialization
- When a user first logs into the system, their data is initialized (including balance, cart, and transaction history).
- If the user does not exist in the system, they are automatically added with default settings.

### 2. Inventory Management
- The inventory is stored in a JSON file and includes information such as the product name, price, available quantity, and discount.
- Users can view the current inventory, and the system will check stock availability when items are added to the cart.

### 3. Shopping Cart Management
- Users can add items to their cart, which is stored in the system under the user’s profile.
- The system ensures that users cannot exceed the available stock when adding items.
- Cart items can be removed, and the quantity can be adjusted using the "Clear Cart" feature.

### 4. Checkout Process
- Users are prompted to checkout when they wish to complete their purchase.
- The system calculates the total cost, including an additional GST of 18% and checks whether the user has enough balance to complete the purchase.
- After the checkout, if the transaction is successful, the user’s cart is cleared, and a transaction record is added to their history.

### 5. Error Handling
- The system checks for invalid inputs, such as entering non-numeric values for quantity or attempting to remove more products than are in the cart.
- It provides feedback if an attempt is made to checkout with insufficient balance.

## Data Storage

- **Inventory Data**: Products, prices, available quantities, and discounts are stored in `inventory.json`.
- **User Data**: User details such as balance, cart, and transaction history are stored in `users.json`.

## Data Structures

1. **Inventory**: 
   The inventory is stored as a dictionary with product names as keys. Each product has an associated dictionary containing its price, quantity, and discount.

   ```json
   {
     "Laptop": {"price": 50000, "quantity": 10, "discount": 10},
     "Keyboard": {"price": 1000, "quantity": 50, "discount": 5},
     "Mouse": {"price": 500, "quantity": 100, "discount": 2},
     "Monitor": {"price": 15000, "quantity": 20, "discount": 8}
   }
   ```

2. **User Data**:
   The user data is stored as a dictionary, where the key is the username, and the value is a dictionary containing:
   - `balance`: The user's account balance.
   - `cart`: The products in the user’s shopping cart, with quantities.
   - `transactions`: A history of the user’s transactions.

   Example:
   ```json
   {
     "john_doe": {
       "balance": 100000,
       "cart": {
         "Laptop": {"quantity": 4, "price": 50000},
         "Mouse": {"quantity": 6, "price": 500}
       },
       "transactions": []
     }
   }
   ```

## User Interface

The user interface is text-based and is presented through a command-line interface (CLI). The user can interact with the system by selecting options via the menu, which includes:

1. View available products.
2. Add products to the shopping cart.
3. Proceed to checkout.
4. Clear the cart by removing products.
5. Exit the system (only allowed if the cart is empty or checkout is completed).

## Example Usage

1. **Viewing Products**:
   - Users can view a list of available products with details such as product name, price, quantity available, and discount percentage.

2. **Adding Items to Cart**:
   - A user can select a product, specify the quantity, and add it to their cart.

3. **Proceeding to Checkout**:
   - Once the user is ready, they can proceed to checkout where the system calculates the total cost and checks if the user has sufficient balance.
   
4. **Clearing Cart**:
   - Users can choose to clear the cart by removing selected quantities of products.

## Requirements

- Python 3.6 or higher
- Basic understanding of file I/O in Python
- JSON for data storage
