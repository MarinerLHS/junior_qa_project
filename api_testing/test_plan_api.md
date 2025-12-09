# Test Plan – Reqres.in API

**Objective:** 
To test the functionality of the REST API (GET, POST, DELETE), identify bugs, and ensure that the API returns correct responses for requests.

**Test Object:** 
Public REST API: [https://reqres.in/]

**Tools:**
- Postman (for sending requests)
- GitHub (for storing artifacts)
- Google sheets/Notepad (for writing test cases and reports)

**Types of Testing:**
- Functional testing (checking the correctness of all endpoints)
- Positive testing (valid requests)
- Negative testing (invalid requests, empty fields, non-existing resources)
- HTTP status verification (200, 201, 204, 400, 404)

**Test Start Criteria:**
- All endpoints and scenarios are defined
- Checklists and test cases are created

**Test Completion Criteria:**
- All test cases are executed
- All bugs are logged and documented

**Test Objects:**
- List of users (GET /users)
- Single user (GET /users/{id})
- Create user (POST /users)
- Update user (PUT /users/{id})
- Delete user (DELETE /users/{id})
- Field validation checks

