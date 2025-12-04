Test Case ID: TC_API_FAIL_002

Title: Verify that user creation returns 200 OK

**Steps:**

Send POST request to https://reqres.in/api/users

**Body:**
```json
{
    "name": "morpheus",
    "job": "leader"
}
```


**Expected Result:**

- Status code: 200

**Actual Result:**

- Status code: 201

Priority: Medium

Test Type: Negative

Status: FAIL
