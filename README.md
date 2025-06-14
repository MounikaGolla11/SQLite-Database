# SQLite-Database
# Task 7 – Basic Sales Summary using Python and SQLite

This is a simple Python project to create a sales summary from a small SQLite database.

## Objective

- Connect to a SQLite database (`sales_data.db`)
- Run a SQL query to get total quantity sold and revenue for each product
- Show the results using `print()`
- Create a bar chart using `matplotlib`

## Tools Used

- Python
- sqlite3
- pandas
- matplotlib

## How It Works

1. Creates a database with sample sales data (if it doesn't already exist).
2. Runs this SQL query:
   ```sql
   SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue FROM sales GROUP BY product;
   ```
3. Loads the result into a pandas DataFrame.
4. Prints the summary in the terminal.
5. Plots a bar chart and saves it as `sales_chart.png`.

## Files

- `sales_summary.py` – Python code
- `sales_data.db` – SQLite database file (auto-created)
- `sales_chart.png` – Bar chart image (auto-created)

## Skills Learned

- Using SQL in Python
- Working with SQLite databases
- Simple data visualization with matplotlib
