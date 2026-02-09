# Doctor

## Add Doctor

- **Endpoint**: `/api/doctor/add`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name       | Description   | Required | Type   |
| ---------- | ------------ | -------- | ------ |
| name       | Name         | No       | string |
| title      | Title        | No       | string |
| specialty  | Specialty    | No       | string |
| age        | Age          | No       | int    |
| phone      | Phone        | No       | string |
| gender     | Gender       | No       | string |
| status     | Status       | No       | int    |
| category   | Category     | No       | string |
| department | Department   | No       | string |
| schedules  | Schedules    | No       | array  |

### Request Example

```json
{
  "name": "Dr. Lee",
  "title": "Chief Physician",
  "specialty": "Internal Medicine",
  "age": 40,
  "phone": "13800000001",
  "gender": "Male",
  "status": 1,
  "category": "Full-time",
  "department": "Internal Medicine"
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

## Get Doctor List

- **Endpoint**: `/api/doctor/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "name": "Dr. Lee",
      "title": "Chief Physician",
      "specialty": "Internal Medicine",
      "age": 40,
      "phone": "13800000001",
      "gender": "Male",
      "status": 1,
      "category": "Full-time",
      "department": "Internal Medicine"
    }
  ]
}
``` 