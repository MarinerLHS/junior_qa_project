Test Case ID: TC_API_009

Title: Verify that an existing user can be updated partially

Preconditions:
- API is available
- User with ID=2 exists
- Base URL: https://reqres.in/api/

Steps:
1. Send PATCH request to https://reqres.in/api/users/2
2. Include JSON body:
   {
       "name": "morpheus",
       "job": "zion resident"
   }
3. Check the status code
4. Validate returned JSON contains updated data and updatedAt timestamp

Expected Result:
- Status code: 200
- Response contains:
  - name: morpheus
  - job: zion resident
  - updatedAt: time

Actual Result:
- Response contains expected JSON file 
```json 
{
    "name": "morpheus",
    "job": "zion resident",
    "updatedAt": "2025-12-04T18:38:52.031Z"
}
```
- Status code: 200
- No any Errors

Priority: High

Test Type: Positive

Status:
- PASS
