**Test Case ID:** TC_SQL_FAIL_003

**Title:** Violatin of foreign key, user_id not exists. 

**Preconditions:**

Database is available. Table users, products and orders exists. User with id = 999 does not exists.
- Steps:

1. Execute:

```sql
INSERT INTO orders (user_id, product_id, quantity, total_price, status)
VALUES (999, 1, 1, 1200.00, 'pending');
```

2. Observe system response.

-**Screenshot** :

<img src="../../images/NEGATIVE/user-id-not-exists.png" alt="error-user-id-not-exists" width="700">

**Expected Result:**
- Database returns an error:

Insert on table "orders" violates foreign key constraint.

**Actual Result:**
System correctly return error.
SQL Error [23503]: ERROR: insert or update on table "orders" violates foreign key constraint "orders_user_id_fkey"
- Detail: Key (user_id)=(999) is not present in table "users".

- Priority: High

- Test Type: Negative

- Status: Pass
