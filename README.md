# Handle user data from file with API request practice using TypeScript and Express Js (Documentation Practice)
Practice of TypeScript and Express Js to handle api request

# Get user with user id

Request :

`GET /users/userid`

`User id example : 15f7c260-d48d-11ee-a985-b16c6c8af41a`

Response:

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| userID  | string  | User id. |
| firstName  | string  | User first name. |
| lastName  | string  | User last name. |
| age  | number  | User age. |

# Get user with user name

Request : 

`GET /users?name=username`

*User name can be first name or last name, letter case sensitivity.*

Response:

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| userID  | string  | User id. |
| firstName  | string  | User first name. |
| lastName  | string  | User last name. |
| age  | number  | User age. |

# Create new user

Request :

`POST /users/`

> Authentication token is needed

Body : 

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| firstName  | string  | User first name. `Minimum 2 characters`|
| lastName  | string  | User last name. `Minimum 2 characters`|
| age  | number  | User age. `Minimum age 0`|

Response :

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| userID  | string  | User id. |
| firstName  | string  | User first name. |
| lastName  | string  | User last name. |
| age  | number  | User age. |

# Delete a user

Request : 

`DELETE /user/userID`

`User id example : 15f7c260-d48d-11ee-a985-b16c6c8af41a`

> Authentication token is needed

Response : 

`"User Deleted"`

# Update a user

Request : 

`PUT /users/userID`

`User id example : 15f7c260-d48d-11ee-a985-b16c6c8af41a`

Body : 

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| firstName  | string  | User first name. `Minimum 2 characters`|
| lastName  | string  | User last name. `Minimum 2 characters`|
| age  | number  | User age. `Minimum age 0`|

Response :

| **Key** | **Type** | **Desciption** |
| ------------- | ------------- | ------------- |
| userID  | string  | User id. |
| firstName  | string  | User first name. |
| lastName  | string  | User last name. |
| age  | number  | User age. |

