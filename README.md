Expense Tracker
The Expense Tracker app is an Android application designed to help users manage their expenses efficiently. It allows users to add, view, and delete expenses while keeping track of their remaining budget.
Project done by: Francu Teodor Matei, Radu Matei, Munteanu Amalia Nicole

Features
Add Expense: Users can add expense details such as title, amount, and date.
Expense List: A dynamic list displaying all added expenses.
Remaining Budget: A feature to calculate and display the remaining budget.
Delete All Expenses: Clear all expenses with a single tap.
Background Services: Services to log expense data and handle alerts.
Custom Alerts: Notifications to remind users of their expense patterns.
Database Integration: Uses SQLite for data persistence.

Project Structure

Activities
MainActivity:
Displays the list of expenses.
Provides options to add a new expense or delete all expenses.

AddExpenseActivity:
Allows users to input expense details (title, amount, date).
Contains a "Save Expense" button to store the data.

Services
ExpenseForegroundService:
A foreground service that provides real-time updates related to expenses.

ExpenseLoggingService:
Logs expense-related data for tracking and debugging.

Receivers
AlertReceiver:
Handles scheduled alerts for user notifications.

ExpenseAlertReceiver:
Manages custom expense-related alerts.

Database
ExpenseDatabaseHelper:
Manages database operations like adding, retrieving, and deleting expenses.

Layouts
1. activity_main.xml
Add Expense Button: Opens the AddExpenseActivity.
Remaining Budget TextView: Displays the user's remaining budget.
Expense ListView: Shows a list of all saved expenses.
Delete All Button: Deletes all expenses.

2. activity_add_expense.xml
Input Fields:
Title
Amount
Date (e.g., "2025-01-01").
Save Expense Button: Saves the expense data.

How to Run the Project
Download the source code as a ZIP file.
Open the project in Android Studio.
Build the project to ensure there are no errors.
Run the project on an emulator or a physical device.
