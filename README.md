# MYSQL-Comprehensive-Assessment-

his document outlines a MySQL Comprehensive Assessment for building a Library Management System. The project focuses on tracking book information, costs, status, and availability through a structured database.
## Database Schema
The project requires the creation of a database named library containing the following six tables:
* Branch: Contains Branch_no (Primary Key), Manager_Id, Branch_address, and Contact_no.
* Employee: Contains Emp_Id (Primary Key), Emp_name, Position, Salary, and Branch_no (Foreign Key referencing Branch).
* Books: Contains ISBN (Primary Key), Book_title, Category, Rental_Price, Status (yes/no for availability), Author, and Publisher.
* Customer: Contains Customer_Id (Primary Key), Customer_name, Customer_address, and Reg_date.
* IssueStatus: Contains Issue_Id (Primary Key), Issued_cust (Foreign Key referencing Customer), Issue_date, and Isbn_book (Foreign Key referencing Books).
* ReturnStatus: Contains Return_Id (Primary Key), Return_cust, Return_book_name, Return_date, and Isbn_book2 (Foreign Key referencing Books).
## Assessment Queries
The document lists 12 specific SQL queries to perform on the database, including:
* Retrieving available book titles, categories, and rental prices.
* Listing employee names and salaries in descending order.
* Displaying total book counts per category.
* Identifying customers who registered before 2022-01-01 but haven't issued books.
* Retrieving branch information for locations with more than 5 employees.
