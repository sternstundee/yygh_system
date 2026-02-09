# 订单管理

## 添加订单

- **接口地址**：`/api/orders/save`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称        | 说明       | 是否必须 | 类型   |
| --------------- | ---------- | -------- | ------ |
| registrationId  | 挂号ID     | 否       | string |
| amount          | 金额       | 否       | number |
| status          | 状态       | 否       | int    |

### 请求示例

```json
{
  "registrationId": "1",
  "amount": 100,
  "status": 1
}
```

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": true
}
```

---

## 获取订单列表

- **接口地址**：`/api/orders/list`
- **请求方式**：`GET`

### 响应示例

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