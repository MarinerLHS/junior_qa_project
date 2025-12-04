**Bug ID: BUG_API_003**
Title: PATCH /users/2 returns 400 Bad Request for invalid JSON

**Test Case ID: TC_API_FAIL_003**

Environment: Windows 10 PRO; Postman v11.74.4;

Reported By: Igor Protsenko

**Description:**
The PATCH request with broken JSON is rejected with 400 Bad Request. The test case expected 200 OK and updated fields.

**Steps to Reproduce:**

- Send PATCH request to https://reqres.in/api/users/2

- Request body (broken JSON):
```json
{
  "name": "morpheus",
  "job":
}
```

- Check the status code and response

**Expected Result:**

- Status code: 200 OK

- Response contains updated fields

**Actual Result:**

- Status code: 400 Bad Request

Severity: Low

Priority: Low

Status: Open

Comments: The test case is intentionally incorrect to demonstrate negative testing.
