Test Case ID: TC_API_002

Title: Verify that a single user with ID=2 can be retrieved successfully

Preconditions:
- API is available
- User with ID=2 exists
- Base URL: https://reqres.in/api/

Steps:
1. Send GET request to https://reqres.in/api/users/2
2. Check the status code
3. Validate returned JSON structure and values

Expected Result:
- Status code: 200
- Response contains required fields:
id, email, first_name, last_name, avatar
- Field types are correct
- Response contains:
 ```json 
{
    "data": {
        "id": 2,
        "email": "janet.weaver@reqres.in",
        "first_name": "Janet",
        "last_name": "Weaver",
        "avatar": "https://reqres.in/img/faces/2-image.jpg"
    },
    "support": {
        "url": "<a href=https://reqres.in/#support-heading>https://reqres.in/#support-heading</a>",
        "text": "To keep ReqRes free, contributions are appreciated!"
    }
}
```
- No errors

Actual Result:

- Code: 200 

- Response contains an actual user with ID=2:
```json
"data": {
        "id": 2,
        "email": "janet.weaver@reqres.in",
        "first_name": "Janet",
        "last_name": "Weaver",
        "avatar": "https://reqres.in/img/faces/2-image.jpg"
    }
```
- Field types are correct
- No errors.

Priority: High

Test Type: Positive

Status:
- Pass 
