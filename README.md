# Relational Databases DQL commands HW-03

## P1

```sql
SELECT * FROM products;
```

![](p1_1.png)

```sql
SELECT name, phone FROM shippers;
```

![](p1_2.png)

## P2

```sql
SELECT MIN(price) as min_price, MAX(price) as max_price, AVG(price) as avg_price FROM products;
```
![](p2_1.png)


## P3

```sql
SELECT DISTINCT category_id, price 
FROM products 
ORDER BY price DESC 
LIMIT 10;
```
![](p3_1.png)

## P4

```sql
SELECT COUNT(*) AS products_count 
FROM products 
WHERE price BETWEEN 20 AND 100;
```
![](p4_1.png)

## P5

```sql
SELECT supplier_id, COUNT(*) as products_count, AVG(price) as avg_price 
FROM products 
GROUP BY supplier_id;
```
![](p5_1.png)
