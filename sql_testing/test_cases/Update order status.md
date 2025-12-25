**Test Case ID:** TC_SQL_008

**Title:** Update order status 

**Preconditions:**
Database is available. Table orders exists. Order with id = 2 exists.

-Steps:

1.Execute:
```sql
UPDATE orders
SET status = 'completed'
WHERE id = 2;
```
-**Screenshot** :

<img src="../images/UPDATE/update-order-status.png" alt="update-order-status" width="700">


Verify change:
```sql
SELECT status FROM orders WHERE id = 2;
```
-**Screenshot-of-result** :

<img src="../images/UPDATE/order-status-result.png" alt="order-status-result" width="700">


**Expected Result:**
Order with id = 2 will change status to completed.

**Actual Result:**
UPDATE executes successfully. SELECT confirms new status is applied.

- Priority: High

- Test Type: Positive

- Status: Pass
