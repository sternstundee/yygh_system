# Orders

## Add Order

- **Endpoint**: `/api/orders/save`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name           | Description   | Required | Type   |
| -------------- | ------------ | -------- | ------ |
| registrationId | Registration | No       | string |
| amount         | Amount       | No       | number |
| status         | Status       | No       | int    |

### Request Example

```json
{
  "registrationId": "1",
  "amount": 100,
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

## Get Order List

- **Endpoint**: `/api/orders/list`
- **Method**: `GET`

### Response Example

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "registrationId": "1",
      "amount": 100,
      "status": 1
    }
  ]
}
``` 