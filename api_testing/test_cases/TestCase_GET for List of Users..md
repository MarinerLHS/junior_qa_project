Test Case ID: TC_API_001
Title: Verify that user with ID=2 can be retrieved successfully

Preconditions:
- API is available
- Base URL: https://api.reqres.in/api/

Steps:
1. Send GET request to /users/2
2. Check the status code
3. Validate returned JSON structure

Expected Result:
- Status code: 200
- Response contains:
  - id: 2
  - email: janet.weaver@reqres.in
  - first_name: Janet
  - last_name: Weaver
  - avatar: valid URL

Actual Result:
- (You will fill this after running Postman)

Status:
- (PASS/FAIL)
