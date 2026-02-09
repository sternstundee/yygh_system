# Appointment

## Import Appointment Excel Data

- **Endpoint**: `/api/appointment/import`
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

## Get Appointment List

- **Endpoint**: `/api/appointment/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "patientId": "1",
      "doctorId": "2",
      "departmentId": "3",
      "appointmentTime": "2024-06-01T10:00:00"
    }
  ]
}
``` 