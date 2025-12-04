Test Case ID: TC_API_FAIL_003

Title: Verify that update user returns 200 with invalid JSON

**Steps:**

Send PATCH request to https://reqres.in/api/users/2

**Body (broken JSON):**
```json
{
    "name": "morpheus",
    "job":
}
```


**Expected Result:**

- Status code: 200

- API returns updated fields

**Actual Result:**

- Status code: 400 Bad Request

Priority: Low

Test Type: Negative

Status: FAIL
