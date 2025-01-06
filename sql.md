### SQL Query questions
**Say we have two tables, Orders and Products** 
orders table has:
   1. id
   2. product_id (foreign key to product table)
   3. price
   4. date (not relevant to the question)

product table has:
   1. id (pk)
   2. name

Write the SQL query to find the 3 topmost selling product and the total sales made (product_name, total_sales)


solve above and explain in detail steps involved
SELECT p.name AS product_name,
       SUM(o.price) AS total_sales
FROM orders o
JOIN products p ON o.product_id = p.id
GROUP BY p.name
ORDER BY total_sales DESC
LIMIT 3;



-----------------------------------------------------------------------------
