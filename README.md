Cafe Management System

Overview

This is a simple Python-based application designed to help small cafe owners manage their day-to-day sales. It automates the process of displaying the menu, taking orders, and calculating the final bill with tax. I built this project to practice using Python modules, functions, and data structures like lists and dictionaries.

Features

Digital Menu: Shows a clean list of items and prices.

Easy Ordering: You can add multiple items to your cart one by one.

Automatic Billing: Calculates the total cost automatically so there are no math errors.

Tax Calculation: Automatically adds a 5% GST to the final bill.

Smart Input: It understands if you type "coffee" or "Coffee", so it's easy to use.

Technologies Used

Language: Python 3

Concepts:

Modular Programming (Code split into multiple files)

Dictionaries & Lists

Functions & Control Flow (Loops/Conditions)

Project Structure

My code is organized into three files to keep it clean:

main.py: The entry point where the user interacts with the program.

cafe_menu.py: Stores the menu items and prices.

billing.py: Contains the logic for calculating totals and printing the receipt.

How to Run the Project

Make sure you have Python installed on your computer.

Download or Clone this repository.

Open your terminal or command prompt.

Navigate to the CafeProject folder.

Run the following command:

python main.py


How to Test

Run the program.

When asked for an order, type Coffee.

Then type Pizza.

Type Done to finish.

Check the final receipt; it should show the total of Coffee + Pizza plus 5% tax.
