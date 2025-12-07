
**Test Case ID:** TC_SQL_005

**Title:** Check of quantity of orders per user

**Preconditions:** Database is available. Tables "orders" and "users" exists.

- Steps:

1. Execute: `SELECT user_id, COUNT(*) AS order_count 
		FROM orders 
		GROUP BY user_id;`
    
2. Check returned data

**Expected Result:** Returns 2 rows, with columns user_id and order_count
 
**Actual Result:** Query executed successfuly. Returns two rows, with correct columns. 

- Priority: High

- Test Type: Positive

- Status: Pass
