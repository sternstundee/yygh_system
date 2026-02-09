# Registration

## Add Registration

- **Endpoint**: `/api/registration/save`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name         | Description     | Required | Type   |
| ------------ | -------------- | -------- | ------ |
| userId       | User ID        | No       | string |
| doctorId     | Doctor ID      | No       | string |
| departmentId | Department ID  | No       | string |
| registerTime | Register Time  | No       | string |
| status       | Status         | No       | int    |

### Request Example

```json
{
  "userId": "1",
  "doctorId": "2",
  "departmentId": "3",
  "registerTime": "2024-06-01T09:00:00",
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

## Get Registration List

- **Endpoint**: `/api/registration/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "userId": "1",
      "doctorId": "2",
      "departmentId": "3",
      "registerTime": "2024-06-01T09:00:00",
      "status": 1
    }
  ]
}
``` 