# Message

## Add Message

- **Endpoint**: `/api/message/save`
- **Method**: `POST`
- **Request Type**: `application/x-www-form-urlencoded, application/json`
- **Response Type**: `*/*`

### Request Parameters

| Name    | Description | Required | Type   |
| ------- | ----------- | -------- | ------ |
| userId  | User ID    | No       | string |
| content | Content    | No       | string |
| type    | Type       | No       | string |
| status  | Status     | No       | int    |

### Request Example

```json
{
  "userId": "1",
  "content": "Your appointment is successful!",
  "type": "Notification",
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

## Get Message List

- **Endpoint**: `/api/message/list`
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
      "content": "Your appointment is successful!",
      "type": "Notification",
      "status": 1
    }
  ]
}
``` 