Test Case ID: TC_API_006

Title: Verify that a new user can be created successfully

Preconditions:
- API is available
- Base URL: https://reqres.in/api/

Steps:
1. Send POST request to https://reqres.in/api/users
2. Include JSON body:
```json
   {
       "name": "morpheus",
       "job": "leader"
   }
```
3. Check the status code
4. Validate returned JSON contains created user data

Expected Result:
- Status code: 201
- Response contains:
  - id (generated)
  - name: morpheus
  - job: leader
  - createdAt timestamp

Actual Result:
- Response contain expected data, file JSON
```json 
{
    "name": "morpheus",
    "job": "leader",
    "id": "330",
    "createdAt": "2025-12-04T18:14:48.111Z"
}
```
- Fields are correct
- Status code: 201
- No any errors

Priority: High

Test Type: Positive

Status:
- PASS
