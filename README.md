



# Inventory Management System Database ERD

This README file provides an overview of the Entity Relationship Diagram (ERD) for the database. The ERD illustrates the relationships between different entities (tables) stored within the database.

## Entities

- **Customer**
- **Store**
- **Employee**
- **Product**
- **Supplier**
- **Order**
- **Debt**
- **Order Items**
- **Store Items**
- **Product Supplier**

## Relationships

- A **Customer** can have many **Orders**.
- An **Order** belongs to one **Customer**.
- A **Customer** can have many **Debts**.
- A **Debt** belongs to one **Customer**.
- A **Store** can have many **Orders**.
- An **Order** belongs to one **Store**.
- A **Store** can have many **Employees**.
- An **Employee** works for one **Store** (One-to-Many).
- A **Store** can have many **Products**.
- A **Product** can be supplied by many **Suppliers** (Many-to-Many).
- A **Supplier** can supply many **Products** (Many-to-Many).
- A **Product** can be part of many **Orders** (Many-to-Many).
- An **Order** can have many **Products** (Many-to-Many).
- A **Store** can have many **Store Items**.
- A **Store Item** references one **Product**.
- A **Product** can be in many **Store Items**.
- An **Order Item** references one **Order**.
- An **Order Item** references one **Store Item**.

## Entity Relationship Diagram (ERD)

![Screenshot 2024-04-03 100305](https://github.com/khaled7hasan7/-Inventory-Management-System-/assets/131875788/14ee2c09-b457-4fc3-8751-d99af7574dbf)

<!-- Replace `path_to_your_erd_image.png` with the actual path to your ERD image -->

## Additional Information

- The ERD depicts foreign keys which are used to establish relationships between tables.
- The table attributes are not shown but can be documented further.

## Running on SQL Server Management Studio

1. **Download and Install SQL Server Management Studio**: If you haven't already, download and install SQL Server Management Studio (SSMS) from [Microsoft's official website](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms).

2. **Open SSMS**: Launch SQL Server Management Studio.

3. **Connect to Your Database Server**: Connect to your SQL Server instance where you want to create the database.

4. **Execute SQL Scripts**: Run the SQL scripts provided in your repository to create the database schema and populate it with initial data.

5. **Explore the Database**: Once the database is created, you can explore the tables, relationships, and data using SQL Server Management Studio.

## Tools

Consider using a database modeling tool to create a more detailed ERD which can include data types, constraints, and table descriptions.

This is a basic structure for your README file, you can expand on it further to include:

- Assumptions made while designing the ERD.
- Future considerations for the database design.
