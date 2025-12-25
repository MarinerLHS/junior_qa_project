**Test Case ID:** TC_SQL_004

**Title:** Find users with no orders 

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

<img src="../images/JOIN/no-orders.png" alt="users-with-no-orders" width="700">


2.Check returned data.

**Expected Result:**
Query returns 1 row with the following columns: first_name, last_name, email.
Data corresponds to existing orders.

**Actual Result:**
Query executed successfully. Returns 1 row with correct columns.

-Priority: Medium

-Test Type: Positive

-Status: Pass
