# Coffee Machine Project

This Python program simulates a simple coffee machine that allows users to order various types of coffee drinks. The program manages resources (water, milk, coffee), processes payments, and dispenses the selected drink if the transaction is successful.

![Logo](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)

## Features

- **Drink Options:** The machine offers three types of drinks:
  - Espresso
  - Latte
  - Cappuccino

- **Resource Management:** The machine checks if there are enough resources (water, milk, coffee) to make the selected drink.

- **Payment Processing:** Users can insert coins (quarters, dimes, nickels, pennies) to pay for their drinks. The machine calculates the total amount inserted and checks if it's sufficient to cover the cost of the drink.

- **Transaction Handling:** If the user inserts more money than required, the machine returns the change. If the user inserts less money, the transaction is canceled, and the money is refunded.

- **Resource Report:** Users can view the current status of the machine's resources and the total profit by typing `report`.

- **Turn Off:** The machine can be turned off by typing `off`.

## How to Use

1. **Run the Program:** Start the program by running the Python script.
2. **Choose a Drink:** When prompted, type the name of the drink you want (espresso, latte, cappuccino).
3. **Insert Coins:** Follow the prompts to insert coins. The machine will calculate the total amount and determine if the payment is sufficient.
4. **Enjoy Your Drink:** If the transaction is successful, the machine will dispense your drink.
5. **View Resource Report:** Type `report` to see the current resources and profit.
6. **Turn Off the Machine:** Type `off` to stop the program.

## Code Overview

The main components of the code are:

- **MENU:** A dictionary containing the drink options, their ingredients, and costs.
- **Resources:** A dictionary that tracks the available quantities of water, milk, and coffee.
- **Functions:**
  - `is_resource_sufficient(order_ingredients)`: Checks if there are enough resources to make the selected drink.
  - `process_coin()`: Handles coin input and calculates the total amount of money inserted.
  - `is_transaction_sucessful(money_received, drink_cost)`: Verifies if the inserted money is sufficient for the drink.
  - `make_coffee(drink_name, order_ingredients)`: Deducts the required ingredients from the resources and serves the drink.

## Requirements

- Python 3.x

## Running the Project

1. Clone or download the project to your local machine.
2. Open a terminal or command prompt and navigate to the project directory.
3. Run the script using Python:

   ```bash
   python coffee_machine.py
