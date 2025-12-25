**Test Case ID:** TC_SQL_007

**Title:** Update email of a specific user

**Preconditions:**
Database is available. Table users exists. User with id = 1 exists.

-Steps:

1.Execute:
```sql
UPDATE users
SET email = 'john.new@example.com'
WHERE id = 1;
```
-**Screenshot** :

<img src="../images/UPDATE/email-change.png" alt="change-email-of-specific-user" width="700">


Verify change:
```sql
SELECT email FROM users WHERE id = 1;
```
-**Screenshot-of-result** :

<img src="../images/UPDATE/email-change-result.png" alt="change-email-of-specific-user-result" width="700">


**Expected Result:**
Email of user with id = 1 is updated to john.new@example.com

**Actual Result:**
UPDATE executes successfully. SELECT confirms new email is applied.

- Priority: Medium

- Test Type: Positive

- Status: Pass
