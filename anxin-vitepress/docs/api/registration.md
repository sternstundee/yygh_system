# 挂号管理

## 添加挂号

- **接口地址**：`/api/registration/save`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称      | 说明     | 是否必须 | 类型   |
| ------------- | -------- | -------- | ------ |
| userId        | 用户ID   | 否       | string |
| doctorId      | 医生ID   | 否       | string |
| departmentId  | 科室ID   | 否       | string |
| registerTime  | 挂号时间 | 否       | string |
| status        | 状态     | 否       | int    |

### 请求示例

```json
{
  "userId": "1",
  "doctorId": "2",
  "departmentId": "3",
  "registerTime": "2024-06-01T09:00:00",
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

## 获取挂号列表

- **接口地址**：`/api/registration/list`
- **请求方式**：`GET`

### 响应示例

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