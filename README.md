# Leet-code-solutions-SQL
This repository guides you through the 50 most important SQL Leet Code problems which serves as a perfect bucket to prepare you for SQL interviews or tasks in your daily job. Have Fun and comment me out if you face any issues while running the codes. 

Problem 1  Table: Products

+-------------+---------+
| Column Name | Type    |
+-------------+---------+
| product_id  | int     |
| low_fats    | enum    |
| recyclable  | enum    |
+-------------+---------+
product_id is the primary key (column with unique values) for this table.
low_fats is an ENUM (category) of type ('Y', 'N') where 'Y' means this product is low fat and 'N' means it is not.
recyclable is an ENUM (category) of types ('Y', 'N') where 'Y' means this product is recyclable and 'N' means it is not.
 

Write a solution to find the ids of products that are both low fat and recyclable.

Return the result table in any order.

Solution 1 : 

SELECT product_id FROM Products
WHERE low_fats = 'Y'
AND recyclable = 'Y';
