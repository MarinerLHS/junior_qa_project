Test Case ID: TC_API_003

Title: Verify that requesting a non-existing user returns correct error

Preconditions:
- API is available
- User with ID=23 does not exist
- Base URL: https://reqres.in/api/

Steps:
1. Send GET request to https://reqres.in/api/users/23
2. Check the status code
3. Validate returned JSON error message

Expected Result:
- Status code: 404
- Response body is empty or contains an error message

Actual Result:
- Status code: 404
- Respponse body with empty file JSON {}

Priority: Medium

Test Type: Negative

Status:
- PASS
