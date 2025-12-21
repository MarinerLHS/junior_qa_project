 # **Api testing checklist Reqres.in** #                                          


| ID | Descriptoin of API requests                                          | Expected result | Priority | Status |
|:---|:---------------------------------------------------------|:----------------|:--------:|:------:|
|TC_API_001| GET for List of Users.           | Status code: 200, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|TC_API_002| GET for Single User.             | Status code: 200, Field types are correct, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|  3.| GET for Single User not Found.         |
|  4.| GET for Single **Resource**.           |
|  5.| GET for Single **Resource** Not Found. |
|  6.| POST for Create.                       |
|  7.| POST for Register successful.          |
|  8.| POST for Register unsuccessful.        |
| 9. | PATCH for Update.                      |
| 10.| DELETE for Delete.                     |
| 11.| GET for Wrong Expected Email.          |
| 12.| POST for Wrong expected Status Code.   |
| 13.| PATCH for Invalid Json Body.           |
