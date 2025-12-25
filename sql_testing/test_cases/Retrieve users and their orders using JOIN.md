**Test Case ID:** TC_SQL_006

**Title:** Retrieve users and their orders using JOIN

**Preconditions:**
Database is available. Tables users, products, and orders exist and contain initial sample data.

-Steps:

1.Execute:

```sql
SELECT 
    u.first_name,
    u.last_name,
    u.email
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
WHERE o.id IS NULL;
```
-**Screenshot** :

<img src="../images/JOIN/name and products.png" alt="user-and-their-orders" width="700">

2.Check returned data.

**Expected Result:**
Query returns 3 rows with the following columns: first_name, last_name, product_name, quantity, total_price.
Data corresponds to existing orders.

**Actual Result:**
Query executed successfully. Returns 3 rows with correct column values.

-Priority: High

-Test Type: Positive

-Status: Pass
