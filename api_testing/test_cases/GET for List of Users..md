Test Case ID: TC_API_001

Title: Verify that the list of users can be retrieved successfully

Preconditions:
- API is available
- Base URL: https://reqres.in/api/

Steps:
1. Send GET request to https://reqres.in/api/users?page=1
2. Check the status code
3. Validate returned JSON structure and user list

Expected Result:
- Status code: 200
- Response contains required fields:
id, email, first_name, last_name, avatar
- Field types are correct
- Response contains a list of users with fields:
```json
{
  "page": 2,
  "per_page": 6,
  "total": 12,
  "total_pages": 2,
  "data": [
    {
      "id": 7,
      "email": "michael.lawson@reqres.in",
      "first_name": "Michael",
      "last_name": "Lawson",
      "avatar": "https://reqres.in/img/faces/7-image.jpg"
    }
  ]
}
```
- No errors

Actual Result:
- Status code: 200
- Response contains a list of users
- Fields and type of fields are correct
- No errors

Priority: High

Test Type: Positive

Status:
- PASS
