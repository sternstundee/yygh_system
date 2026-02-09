# Auth

## User Registration

- **Endpoint**: `/api/auth/register`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name        | Description   | Required | Type   |
| ----------- | ------------ | -------- | ------ |
| username    | Username     | Yes      | string |
| password    | Password     | Yes      | string |
| realName    | Real Name    | Yes      | string |
| phone       | Phone        | No       | string |
| email       | Email        | No       | string |
| role        | Role         | Yes      | string |
| departmentId| DepartmentId | No       | string |

### Request Example

```json
{
  "username": "test",
  "password": "123456",
  "realName": "John Doe",
  "phone": "13800000000",
  "email": "test@example.com",
  "role": "doctor",
  "departmentId": "1"
}
```

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```

---

## User Login

- **Endpoint**: `/api/auth/login`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name     | Description | Required | Type   |
| -------- | ----------- | -------- | ------ |
| username | Username   | Yes      | string |
| password | Password   | Yes      | string |

### Request Example

```json
{
  "username": "test",
  "password": "123456"
}
```

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": ""
}
```

---

## User Logout

- **Endpoint**: `/api/auth/logout`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded`
- **Response Type**: `*/*`

### Request Parameters

None

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
``` 