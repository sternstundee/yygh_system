# User

## Add User

- **Endpoint**: `/api/user/add`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name     | Description | Required | Type   |
| -------- | ----------- | -------- | ------ |
| username | Username   | No       | string |
| password | Password   | No       | string |
| realName | Real Name  | No       | string |
| phone    | Phone      | No       | string |
| email    | Email      | No       | string |
| roleId   | Role ID    | No       | string |
| status   | Status     | No       | int    |

### Request Example

```json
{
  "username": "user1",
  "password": "123456",
  "realName": "Tom",
  "phone": "13800000002",
  "email": "user1@example.com",
  "roleId": "admin",
  "status": 1
}
```

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": true
}
```

---

## Get User List

- **Endpoint**: `/api/user/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "username": "user1",
      "realName": "Tom",
      "phone": "13800000002",
      "email": "user1@example.com",
      "roleId": "admin",
      "status": 1
    }
  ]
}
``` 