Medicine Management System

Project Overview

The Medicine Management System / Pharmacy Management System is a simple software project designed to manage medicine details, customer details, sales, quantities, and bill calculation.

This project is suitable for a 1st-year BCA student and demonstrates basic concepts of database management and system design.

Features

- Manage medicine details
- Manage customer details
- Select medicines for sale
- Enter medicine quantity
- Check available medicine stock
- Calculate item total
- Calculate total bill
- Update medicine stock after sale
- Generate bill
- Display customer and sale details

Main Entities

The system contains the following entities:

1. Medicine
2. Customer
3. Sale
4. Sale_Item
5. Bill

Entity Details

1. Medicine

Stores information about medicines.

- Medicine_ID (PK)
- Medicine_Name
- Category
- Price
- Stock_Quantity
- Expiry_Date

2. Customer

Stores customer information.

- Customer_ID (PK)
- Customer_Name
- Contact_Number
- Address

3. Sale

Stores information about each sale.

- Sale_ID (PK)
- Customer_ID (FK)
- Sale_Date

4. Sale_Item

Stores medicines included in a particular sale.

- Sale_Item_ID (PK)
- Sale_ID (FK)
- Medicine_ID (FK)
- Quantity
- Price
- Item_Total

5. Bill

Stores billing information.

- Bill_ID (PK)
- Sale_ID (FK)
- Total_Amount
- Bill_Date

Relationships

- One Customer can have many Sales — 1:N
- One Sale belongs to one Customer — N:1
- One Sale can contain many Sale_Items — 1:N
- One Medicine can appear in many Sale_Items — 1:N
- One Sale generates one Bill — 1:1

Bill Calculation

Item Total

Item Total = Medicine Price × Quantity

Total Bill

Total Bill = Sum of All Item Totals

Basic Working Process

1. Enter customer details.
2. Display available medicine details.
3. Select a medicine.
4. Enter the required quantity.
5. Check whether sufficient stock is available.
6. If stock is insufficient, display "Insufficient Stock".
7. Calculate the item total.
8. Add the item total to the total bill.
9. Ask whether the customer wants to purchase another medicine.
10. If Yes, repeat the medicine selection process.
11. If No, generate the final bill.
12. Update the medicine stock.
13. Display customer details, selected medicines, quantities, prices, and final bill.
14. Complete the sale.

Flowchart Symbols

Symbol| Purpose
Oval| Start / End
Parallelogram| Input / Output
Rectangle| Processing
Diamond| Decision

Project Objective

The main objective of this project is to develop a simple system that can manage medicines and customers, process medicine sales, maintain stock quantities, and calculate the final bill accurately.

Technologies

The project can be implemented using technologies such as:

- Programming Language: As required by the project
- Database: MySQL / SQLite
- IDE: Visual Studio Code / Eclipse / NetBeans or any suitable IDE

Project Level

1st-Year BCA Project

Conclusion

The Medicine Management System provides a simple way to manage medicine information, customer information, sales, stock quantities, and billing. It also demonstrates basic concepts of ER diagrams, relationships, database management, algorithms, flowcharts, and bill calculation.
