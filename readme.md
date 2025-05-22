# Practice Task M_9: SQL Database and Query Exercises

This project contains SQL scripts for creating and populating a sample database, along with a series of SQL queries to practice database operations such as joins, aggregations, subqueries, and date functions.

## Contents

- **pt_m9.sql**: Main SQL script containing:
  - User and database creation
  - Table definitions for `employees`, `departments`, and `orders`
  - Sample data insertion
  - Practice SQL queries for various tasks

## Database Structure

### Tables

- **departments**

  - `department_id` (SERIAL, Primary Key)
  - `department_name` (VARCHAR)

- **employees**

  - `employee_id` (SERIAL, Primary Key)
  - `employee_name` (VARCHAR)
  - `department_id` (INT, Foreign Key)
  - `salary` (DECIMAL)
  - `hire_date` (DATE)

- **orders**
  - `order_id` (SERIAL, Primary Key)
  - `customer_id` (INT)
  - `order_date` (DATE)
  - `total_amount` (DECIMAL)

## Tasks Covered

### Employee & Department Queries

1. **Inner Join**: Retrieve employees with salary above 70,000 and their department names.
2. **Left Join**: List all employees and their departments.
3. **Group By**: Show average salary per department.
4. **Aggregate**: Count employees in each department.
5. **Subquery**: Find employees with salary above the company average.
6. **Top Departments**: Departments with the highest average salary.
7. **Recent Hires**: Employees hired in the last year.
8. **Yearly Hires**: Count of employees hired each year.

### Order Queries

1. **Frequent Customers**: Customers with more than 2 orders and their total spend.
2. **Top Spender**: Customer who spent the most.
3. **Average Order**: Average order amount per customer.
4. **Monthly Orders**: Number of orders per month.
5. **Monthly Sales (2022)**: Total order amount per month in 2022.

## Usage

1. **Setup Database**

   - Run the script in [pt_m9.sql](pt_m9.sql) using your PostgreSQL client.
   - This will create the user, database, tables, and insert sample data.

2. **Run Queries**
   - Each task is separated by comments in the SQL file.
   - Copy and execute the queries as needed to practice or analyze results.

## Requirements

- PostgreSQL

## License

This project is for educational purposes.
