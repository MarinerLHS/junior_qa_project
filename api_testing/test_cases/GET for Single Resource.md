Test Case ID: TC_API_004

Title: Verify that a single resource can be retrieved successfully

Preconditions:
- API is available
- Resource with ID=2 exists
- Base URL: https://reqres.in/api/

Steps:
1. Send GET request to https://reqres.in/api/unknown/2
2. Check the status code
3. Validate returned JSON structure and resource details

Expected Result:
- Status code: 200
- Response contains:
```json
 {
    "data": {
        "id": 2,
        "name": "fuchsia rose",
        "year": 2001,
        "color": "#C74375",
        "pantone_value": "17-2031"
    }
}
```
- No errors

Actual Result:
- Response contains expected data: 
  - Code: 200
   ```json 
   { "data": {
        "id": 2,
        "name": "fuchsia rose",
        "year": 2001,
        "color": "#C74375",
        "pantone_value": "17-2031"
    }
   }
   ```

- No any errors

Priority: Medium

Test Type: Positive

Status:
- PASS
