
**Test Case ID:** TC_SQL_002

**Title:** Check of quantity of orders per user

**Preconditions:** Database is available. Tables "orders" and "users" exists.

- Steps:

1. Execute: 
```sql
SELECT user_id, COUNT(*) AS order_count 
		FROM orders 
		GROUP BY user_id;
```
-**Screenshot** :

<img src="../images/SELECT/order-per-user.png" alt="quantity-orders-per-user" width="700">

    
2. Check returned data

**Expected Result:** Returns 2 rows, with columns user_id and order_count
 
**Actual Result:** Query executed successfuly. Returns two rows, with correct columns. 

- Priority: High

- Test Type: Positive

- Status: Pass
