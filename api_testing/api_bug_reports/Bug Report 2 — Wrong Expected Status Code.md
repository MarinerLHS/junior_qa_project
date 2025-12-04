**Bug ID: BUG_API_002**

Title: Create User API returns 201 Created instead of expected 200 OK

**Test Case ID: TC_API_FAIL_002**

Environment: Windows 10 PRO; Postman v11.74.4;

Reported By: Igor Protsenko

**Description:**
The POST request to create a new user returns status code 201 Created, but the test case expected 200 OK.

**Steps to Reproduce:**

- Send POST request to https://reqres.in/api/users

**Request body:**

```json
  {
      "name": "morpheus",
      "job": "leader"
  }
```


- Check the status code

**Expected Result:**

- Status code = 200

**Actual Result:**

- Status code = 201

Severity: Medium

Priority: Medium

Status: Open

Comments: API works correctly; test case expectation was intentionally incorrect to simulate FAIL.
