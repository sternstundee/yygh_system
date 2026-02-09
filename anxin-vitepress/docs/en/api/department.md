# Department

## Add Department

- **Endpoint**: `/api/department/save`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name           | Description      | Required | Type   |
| -------------- | --------------- | -------- | ------ |
| departmentName | Department Name | No       | string |
| departmentCode | Department Code | No       | string |
| parentId       | Parent ID       | No       | string |
| leader         | Leader          | No       | string |
| phone          | Phone           | No       | string |
| address        | Address         | No       | string |
| status         | Status          | No       | int    |

### Request Example

```json
{
  "departmentName": "Internal Medicine",
  "departmentCode": "NK001",
  "parentId": "0",
  "leader": "Dr. Li",
  "phone": "13800000004",
  "address": "East Area, 1st Floor",
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

## Get Department List

- **Endpoint**: `/api/department/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "departmentName": "Internal Medicine",
      "departmentCode": "NK001",
      "parentId": "0",
      "leader": "Dr. Li",
      "phone": "13800000004",
      "address": "East Area, 1st Floor",
      "status": 1
    }
  ]
}
``` 