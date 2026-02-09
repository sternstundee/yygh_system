# 排班管理

## 添加排班

- **接口地址**：`/api/schedule/add`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称        | 说明       | 是否必须 | 类型   |
| --------------- | ---------- | -------- | ------ |
| doctorId        | 医生ID     | 否       | string |
| date            | 日期       | 否       | string |
| timeSlot        | 时间段     | 否       | string |
| price           | 价格       | 否       | number |
| availableCount  | 可预约数   | 否       | int    |
| bookedCount     | 已预约数   | 否       | int    |
| status          | 状态       | 否       | string |

### 请求示例

```json
{
  "doctorId": "1",
  "date": "2024-06-01",
  "timeSlot": "上午",
  "price": 50,
  "availableCount": 10,
  "bookedCount": 0,
  "status": "可用"
}
```

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```

---

## 更新排班

- **接口地址**：`/api/schedule/update`
- **请求方式**：`PUT`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

参数同上。

---

## 获取医生的排班列表

- **接口地址**：`/api/schedule/doctor/{doctorId}`
- **请求方式**：`GET`

### 路径参数

| 参数名称 | 说明   | 是否必须 | 类型   |
| -------- | ------ | -------- | ------ |
| doctorId | 医生ID | 是       | string |

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "doctorId": "1",
      "date": "2024-06-01",
      "timeSlot": "上午",
      "price": 50,
      "availableCount": 10,
      "bookedCount": 0,
      "status": "可用"
    }
  ]
}
``` 