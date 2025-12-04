Test Case ID: TC_API_008

Title: Verify unsuccessful user registration without password

Preconditions:
- API is available
- Base URL: https://reqres.in/api/

Steps:
1. Send POST request to https://reqres.in/api/register
2. Include JSON body:
```json
   {
       "email": "sydney@fife"
   }
```
3. Check the status code
4. Validate returned JSON error message

Expected Result:
- Status code: 400
- Response contains error: "Missing password"

Actual Result:
- Response contains JSON 
```json
{
    "error": "Missing password"
}
```
- Status kod: 400

Priority: Medium

Test Type: Negative

Status:
- PASS
