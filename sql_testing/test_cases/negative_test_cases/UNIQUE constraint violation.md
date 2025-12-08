**Test Case ID:** TC_SQL_FAIL_001

**Title:** Attempt to insert a user with duplicate email (UNIQUE constraint violation)

**Preconditions:**
Database is available. Table users exists. Email john.new@example.com already exists in the table.

- Steps:

1. Execute:
```sql
INSERT INTO users (first_name, last_name, email)
VALUES ('Duplicate', 'User', 'john.new@example.com');
```

2. Observe system response.

**Expected Result:**
Database returns an error:
duplicate key value violates unique constraint "users_email_key"

**Actual Result:**
System correctly returns UNIQUE constraint violation.

- Priority: High

- Test Type: Negative

- Status: Pass
