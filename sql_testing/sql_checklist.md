# **SQL testing Checklist** #

### **Description** : Self-studying for understanding of how SQL database works, practice with basic SQL commands. 
### **Environment** : Windows 10 PRO; PostgreSQL 18; DBeaver 25.3.0;
### **Created by** : Igor Protsenko
### **Status** : Done
### **Version** : 1.1.5

| ID | Descriptoin of SQL queries                                | Expected result | Priority | Status |
|:---|:----------------------------------------------------------|:----------------|:--------:|:------:|
|TC_SQL_001| Unique emails. | Query returns nothig, beacuse of unique emails. | High | Pass |
|TC_SQL_002| Quantity of orders per user.| Returns 2 rows, with columns user_id and order_count | High | Pass |
|TC_SQL_003| Total order amount for every user.| Query returns 3 rows with the following columns: first_name, last_name, total_spent. Data corresponds to existing orders. | Medium | Pass |
|TC_SQL_004| Finding users with no orders.| Query returns 1 row with the following columns: first_name, last_name, email. Data corresponds to existing orders. |  Medium | Pass |
|TC_SQL_005| Reducing the quantity of goods in stock.| Stock of product with id = 2 decreases from 150 to 149. | Medium | Pass |
|TC_SQL_006| Retrieving users and their orders by using JOIN statement.| Query returns 3 rows with the following columns: first_name, last_name, product_name, quantity, total_price. | High | Pass |
|TC_SQL_007| Updating email of a specific user by using UPDATE statement. | Email of user with id = 1 is updated to john.new@example.com | Medium | Pass |
|TC_SQL_008| Order status update using a UPDATE statement.| Order with id = 2 will change status to completed. | High | Pass |
|TC_SQL_009| Verifying of all users by SELECT statement. | 3 rows, fields: id, first_name, last_name, email, created_at | High | Pass |
|TC_SQL_010| Verifying users with specific ID by SELECT statement. | 1 row, for user with ID = 2, first_name, last_name, email, created at | High | Pass |
|TC_SQL_011| Verifying of valid prices for products SELECT statement. | Returns empty data. | High | Pass |

## **Negative Tests** ##

| ID | Descriptoin of SQL queries                                | Expected result | Priority | Status |
|:---|:----------------------------------------------------------|:----------------|:--------:|:------:|
|TC_SQL_FAIL_001| Invalid input sintax.| Database returns an error: System returns error of invalid input sintax. | Medium | Pass |
|TC_SQL_FAIL_002| Availability to insert a user with duplicate email.| Database returns an error: duplicate key value violates unique constraint "users_email_key" | High | Pass |
|TC_SQL_FAIL_003| Violatin of foreign key by INSERT statement with user which does not exists. | Database returns an error: Insert on table "orders" violates foreign key constraint. | High | Pass |
