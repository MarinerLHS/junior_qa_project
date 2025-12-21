 # **Api testing checklist Reqres.in** # 
 
### Description : Self-studying for understanding of how API requests works

### Environment : Reqres.in; Windows 10 PRO; Postman v11.74.4;

### Created by : Igor Protsenko

### Status : Done

### Version : 1.12

| ID | Descriptoin of API requests                              | Expected result | Priority | Status |
|:---|:---------------------------------------------------------|:----------------|:--------:|:------:|
|TC_API_001| GET for List of Users.           | Status code: 200, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|TC_API_002| GET for Single User.             | Status code: 200, Field types are correct, Response contains required fields: id, email, first_name, last_name, avatar | High | Pass |
|TC_API_003| GET for Single User not Found.   | Status code: 404, Response body is empty or contains an error message | Medium | Pass |
|TC_API_004| GET for Single **Resource**.     | Status code: 200, No errors | Medium | Pass |
| TC_API_005| GET for Single **Resource** Not Found. | Status code: 404, Response body is empty or contains an error message | Medium | Pass |
|TC_API_006| POST for Create.                 | Status code: 201, Response contains: id (generated), name: morpheus, job: leader, createdAt timestamp | High | Pass |
|TC_API_007| POST for Register successful.    | Status code: 200, Response contains: id, token | High | Pass |
|TC_API_008| POST for Register unsuccessful.  | Status code: 400, Response contains error: "Missing password" | Medium | Pass |
|TC_API_009| PATCH for Update.                | Status code: 200, Response contains: name: morpheus, job: zion resident, updatedAt: time | High | Pass |
|TC_API_010| DELETE for Delete.               | Status code: 204, Response body is empty | High | Pass |

 ## **Negative testing** ##  
| ID | Descriptoin of API requests                              | Expected result | Priority | Status |
|:---|:---------------------------------------------------------|:----------------|:--------:|:------:|
|TC_API_FAIL_001| GET for Wrong Expected Email.| Status code: 200, email: peter.peterson@mail.com | Medium | Fail |
|TC_API_FAIL_002| POST for Wrong expected Status Code.| Status code: 200 | Medium | Fail |
|TC_API_FAIL_003| PATCH for Invalid Json Body.| Status code: 200, API returns updated fields| Low | Fail |
