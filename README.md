-- 1. Create the products table
CREATE TABLE products (
    product_id INT PRIMARY KEY,
    product_name VARCHAR(100),
    price DECIMAL(10, 2)
);

-- 2. Insert sample data into the products table
INSERT INTO products (product_id, product_name, price)
VALUES
    (1, 'Laptop', 1200.00),
    (2, 'Mouse', 25.00),
    (3, 'Keyboard', 75.00),
    (4, 'Monitor', 300.00),
    (5, 'USB Cable', 15.00),
    (6, 'Headphones', 45.00),
    (7, 'Smartphone', 600.00),
    (8, 'Tablet', 150.00);

-- 3. Query to find all products where the price is greater than $50
SELECT product_id, product_name, price
FROM products
WHERE price > 50;

