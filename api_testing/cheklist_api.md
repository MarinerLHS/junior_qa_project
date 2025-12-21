 # **Api testing checklist Reqres.in** #                                          


| ID | Descriptoin of API requests                              | Expected result | Priority | Status |
|:---|:---------------------------------------------------------|:----------------|:--------:|:------:|
|TC_API_001| GET for List of Users.           | Status code: 200, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|TC_API_002| GET for Single User.             | Status code: 200, Field types are correct, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|TC_API_003| GET for Single User not Found.   | Status code: 404, Response body is empty or contains an error message | Medium | Pass |
|TC_API_004| GET for Single **Resource**.     | Status code: 200, No errors | Medium | Pass |
| TC_API_005| GET for Single **Resource** Not Found. | Status code: 404, Response body is empty or contains an error message | Medium | Pass |
|TC_API_006| POST for Create.                 | Status code: 201, Response contains:
- id (generated)
- name: morpheus
- job: leader
- createdAt timestamp | High | Pass |
|TC_API_007| POST for Register successful.    | Status code: 200, Response contains:
- id
- token | High | Pass |
|  8.| POST for Register unsuccessful.        |
| 9. | PATCH for Update.                      |
| 10.| DELETE for Delete.                     |
| 11.| GET for Wrong Expected Email.          |
| 12.| POST for Wrong expected Status Code.   |
| 13.| PATCH for Invalid Json Body.           |
