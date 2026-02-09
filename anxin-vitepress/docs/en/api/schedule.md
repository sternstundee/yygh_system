# Schedule

## Add Schedule

- **Endpoint**: `/api/schedule/add`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name           | Description    | Required | Type   |
| -------------- | ------------- | -------- | ------ |
| doctorId       | Doctor ID     | No       | string |
| date           | Date          | No       | string |
| timeSlot       | Time Slot     | No       | string |
| price          | Price         | No       | number |
| availableCount | Available     | No       | int    |
| bookedCount    | Booked        | No       | int    |
| status         | Status        | No       | string |

### Request Example

```json
{
  "doctorId": "1",
  "date": "2024-06-01",
  "timeSlot": "Morning",
  "price": 50,
  "availableCount": 10,
  "bookedCount": 0,
  "status": "Available"
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

## Update Schedule

- **Endpoint**: `/api/schedule/update`
- **Method**: `PUT`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

Parameters are the same as above.

---

## Get Doctor's Schedules

- **Endpoint**: `/api/schedule/doctor/{doctorId}`
- **Method**: `GET`

### Path Parameters

| Name     | Description | Required | Type   |
| -------- | ----------- | -------- | ------ |
| doctorId | Doctor ID   | Yes      | string |

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "doctorId": "1",
      "date": "2024-06-01",
      "timeSlot": "Morning",
      "price": 50,
      "availableCount": 10,
      "bookedCount": 0,
      "status": "Available"
    }
  ]
}
``` 