Test Case ID: TC_API_FAIL_001

Title: Verify that user email equals peter.peterson@mail.com

**Preconditions:**

- API is available
- User with ID=2 exists
- Base URL: https://reqres.in/api/

**Steps:**

1. Send GET request to https://reqres.in/api/users/2

2. Check status code

3. Validate email

**Expected Result:**

Status code: 200

email: peter.peterson@mail.com

**Actual Result:**

email: janet.weaver@reqres.in

Priority: Medium

Test Type: Negative

Status: FAIL
