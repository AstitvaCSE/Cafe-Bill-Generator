Project Report: Cafe Management System

1. Introduction
The Cafe Management System is a console-based Python application designed to assist small cafe owners in managing their day-to-day billing operations. It automates the process of displaying the menu, taking customer orders, and generating a finalized bill including tax calculations. This project aims to replace manual billing with a digital, error-free solution.

2. Problem Statement
Manual billing in cafes is prone to calculation errors and can be time-consuming during peak hours. Keeping track of item prices and manually calculating taxes (GST) slows down service. There is a need for a simple, lightweight software solution that can run on basic hardware to streamline the ordering and billing process.

3. Project Objectives
To create a user-friendly interface for viewing the menu and placing orders.
To automate mathematical calculations for totals and taxes to ensure accuracy.
To demonstrate modular programming by separating data, logic, and interface.

5. Functional Requirements
Menu Display: The system must accurately display a list of available items and their prices in a readable format.
Order Taking: The system must allow users to input multiple items continuously until they decide to stop. It should validate whether an item exists in the menu.
Billing & Taxation: The system must calculate the subtotal of all items, apply a 5% GST (Goods and Services Tax), and print a final formatted receipt.

5. Non-Functional Requirements
Usability: The application uses simple text prompts, making it easy for non-technical staff to use.
Maintainability: The code is modular (split into three files), making it easy to update menu prices or tax rates without breaking the entire program.
Error Handling: The system handles case sensitivity (e.g., "coffee" vs "Coffee") and invalid inputs (items not on the menu).

6. Technical Implementation
This project utilizes core Python concepts covered in the syllabus:
Modules (Module 10): The project is split into three distinct files (main.py, cafe_menu.py, billing.py) to ensure clean code structure.

Data Structures (Module 7):
Dictionaries: Used to store the Menu ({"Item": Price}), allowing for O(1) time complexity when looking up prices.
Lists: Used to store the user's current order (my_order = []).
Control Flow (Module 8):
While True Loop: Keeps the ordering process active until the user finishes.
If/Else: Validates user input against the menu.
Functions (Module 9): Encapsulates logic for calculating totals and printing receipts to ensure code reusability.
Operators (Module 3): Handles arithmetic operations for summing up prices and calculating percentages for tax.

7. Workflow / Logic
Start: The program initializes and imports the menu data.
Display: The menu is shown to the customer.
Input Loop:
Prompt user for item name.
Check if item exists in menu_items.
If yes -> Add to my_order list.
If no -> Show error message.
If "Done" -> Break loop.

Processing: Pass the my_order list to the billing module.
Output: Calculate Subtotal + Tax and print the final Receipt.

8. Future Enhancements
Add a feature to remove items from the cart before billing.
Implement file handling to save daily sales reports to a text file.
Add an "Admin Mode" to update menu prices directly from the program.
