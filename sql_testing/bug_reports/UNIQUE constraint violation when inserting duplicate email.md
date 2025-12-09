**Bug ID:** BUG_SQL_001

**Title:** UNIQUE constraint violation when inserting duplicate email

**Test Case ID:** TC_SQL_FAIL_001

**Environment:** PostgreSQL 18; DBeaver 25.3.0

**Reported By:** Igor Protsenko

**Description:**
Attempting to insert a user with an email that already exists in the users table results in a UNIQUE constraint violation.

**Steps to Reproduce:**

1.Execute:
```sql
INSERT INTO users (first_name, last_name, email)
VALUES ('Duplicate','User','john.new@example.com');
```

2.Check system response.

**Expected Result:**
Database returns a UNIQUE constraint violation error (intentional negative test case).

**Actual Result:**

Database returns:
`SQL Error [23505]: ERROR: duplicate key value violates unique constraint "users_email_key"`

`Detail: Key (email)=(john.new@example.com) already exists.`

Severity: High

Priority: High

Status: Open
