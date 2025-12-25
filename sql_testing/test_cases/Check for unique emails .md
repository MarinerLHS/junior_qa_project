**Test Case ID:** TC_SQL_001

**Title:** Check for unique emails 

**Preconditions:** Database is available, table with users exists, field email with emails exists for all users.

- Steps:

1. Execute: 
```sql
SELECT email, COUNT(*) 
		FROM users 
		GROUP BY email 
		HAVING COUNT(*) > 1;
```

-**Screenshot** :

<img src="../images/SELECT/unique-emails.png" alt="check-for-unique-emails" width="700">

2. Check returned data

**Expected Result:** Query returns nothig, beacuse of unique emails.
 
**Actual Result:** Query executed sucessfuly. There are no duplicate emails.

- Priority: High

- Test Type: Positive

- Status: Pass
