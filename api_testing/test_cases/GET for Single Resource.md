Steps:
1. Send GET request to https://api.reqres.in/api/unknown/2
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
   ```json {
    "data": {
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
