**Test Case ID:** TC_SQL_003

**Title:** Count the total order amount for every user 

**Preconditions:**
Database is available. Tables users, products, and orders exist and contain initial sample data.

-Steps:

1.Execute:
```sql
SELECT 
    u.first_name,
    u.last_name,
    SUM(o.total_price) AS total_spent	
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
GROUP BY u.id;
```
-**Screenshot** :

<img src="../images/JOIN/total-order-amount.png" alt="total-order-amoun-for-every" width="700">

2.Check returned data.

**Expected Result:**
Query returns 3 rows with the following columns: first_name, last_name, total_spent.
Data corresponds to existing orders.

**Actual Result:**
Query executed successfully. Returns 3 rows with correct column values.

-Priority: Medium

-Test Type: Positive

-Status: Pass
