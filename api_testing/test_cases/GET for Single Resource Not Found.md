Test Case ID: TC_API_005

Title: Verify that requesting a non-existing resource returns correct error

Preconditions:
- API is available
- Resource with ID=23 does not exist
- Base URL: https://reqres.in/api/

Steps:
1. Send GET request to https://reqres.in/api/unknown/23
2. Check the status code
3. Validate returned JSON error message

Expected Result:
- Status code: 404
- Response body is empty or contains an error message

Actual Result:
- Response contains expected status code 404 and an empty JSON file

Priority: Medium

Test Type: Negative

Status:
- PASS
