# Patient

## Import Patient Excel Data

- **Endpoint**: `/api/patient/import`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name | Description | Required | Type |
| ---- | ----------- | -------- | ---- |
| file | Excel File  | Yes      | file |

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": ""
}
```

---

## Get Patient List

- **Endpoint**: `/api/patient/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "name": "John",
      "gender": "Male",
      "age": 30,
      "phone": "13800000003"
    }
  ]
}
``` 