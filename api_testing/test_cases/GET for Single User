Test Case ID: TC_API_002
Title: Verify that a single user with ID=2 can be retrieved successfully

Preconditions:
- API is available
- User with ID=2 exists
- Base URL: https://api.reqres.in/api/

Steps:
1. Send GET request to https://api.reqres.in/api/users/2
2. Check the status code
3. Validate returned JSON structure and values

Expected Result:
- Status code: 200
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
Code: 200 
```json
"data": {
        "id": 2,
        "email": "janet.weaver@reqres.in",
        "first_name": "Janet",
        "last_name": "Weaver",
        "avatar": "https://reqres.in/img/faces/2-image.jpg"
    }
```


Priority: High
Test Type: Positive

Status:
- Pass 
