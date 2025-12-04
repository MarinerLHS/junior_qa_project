Test Case ID: TC_API_007

Title: Verify successful user registration

Preconditions:
- API is available
- User email and password are valid
- Base URL: https://reqres.in/api/

Steps:
1. Send POST request to https://reqres.in/api/register
2. Include JSON body:
   {
       "email": "eve.holt@reqres.in",
       "password": "pistol"
   }
3. Check the status code
4. Validate returned JSON contains id and token

Expected Result:
- Status code: 200
- Response contains:
  - id
  - token

Actual Result:
- Response contains expected status code 200 and JSON file 
```json
{
    "id": 4,
    "token": "QpwL5tke4Pnpja7X4"
}
```
- No any errors

Priority: High

Test Type: Positive

Status:
- PASS
