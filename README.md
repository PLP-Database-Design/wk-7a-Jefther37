📚 Database Design and Normalization Assignment
🎯 Learning Objectives
Understand principles of good database design.

Apply normalization techniques (1NF and 2NF).

Eliminate redundancy and optimize data structure.

🛠️ Requirements
A computer with internet access

A code editor (e.g., Visual Studio Code)

A SQL database environment (e.g., MySQL Workbench)

📋 Assignment Tasks
Question 1: Achieving 1NF (First Normal Form)
Problem:
The ProductDetail table had multiple values in a single column (Products), violating 1NF.

Solution:

Created a new table ProductDetail_1NF where each product for an order is represented in its own row.

Ensured atomicity by separating multi-valued fields.

Question 2: Achieving 2NF (Second Normal Form)
Problem:
The OrderDetails table had a partial dependency — CustomerName depended only on OrderID, not on the whole composite key.

Solution:

Created a Customers table to store OrderID and CustomerName.

Created a new OrderDetails_2NF table to store OrderID, Product, and Quantity.

Added foreign key constraints to maintain referential integrity.

📂 Files Included
answers.sql — Contains all SQL queries for transforming the tables into 1NF and 2NF.

📝 Instructions
Open MySQL Workbench (or your preferred SQL environment).

Execute the queries in answers.sql step-by-step.

Ensure tables are created and populated correctly.

Review structure to confirm normalization is achieved.

✅ Outcome
Data is now atomic (1NF achieved).

Partial dependencies have been removed (2NF achieved).

Database structure is efficient, scalable, and easier to maintain.