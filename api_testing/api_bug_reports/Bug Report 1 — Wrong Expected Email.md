**Bug ID: BUG_API_001**

Title: Single User API returns correct email, but test expected wrong email


**Test Case ID: TC_API_FAIL_001**

Environment: Windows 10 PRO; Postman v11.74.4; 

Reported By: Igor Protsenko

**Description:**
The GET request for user ID=2 returns the correct email from API (janet.weaver@reqres.in), but the test case expected peter.peterson@mail.com.

**Steps to Reproduce:**

1.Send GET request to https://api.reqres.in/api/users/2

2.Check the email field in the response

**Expected Result:**
- Status code: 200
- Email = peter.peterson@mail.com

**Actual Result:**
- Status code: 200
- Email = janet.weaver@reqres.in

Severity: Medium

Priority: Medium

Status: Open

Comments: Test case intentionally set the wrong expected email to simulate a FAIL.
