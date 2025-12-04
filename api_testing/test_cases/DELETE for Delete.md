Test Case ID: TC_API_010

Title: Verify that an existing user can be deleted

Preconditions:
- API is available
- User with ID=2 exists
- Base URL: https://reqres.in/api/

Steps:
1. Send DELETE request to https://reqres.in/api/users/2
2. Check the status code

Expected Result:
- Status code: 204
- Response body is empty

Actual Result:
- There is expected empty response, with status code 204 **No content**

Priority: High

Test Type: Positive

Status:
- PASS
