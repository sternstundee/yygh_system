# 预约管理

## 导入预约Excel数据

- **接口地址**：`/api/appointment/import`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称 | 说明     | 是否必须 | 类型   |
| -------- | -------- | -------- | ------ |
| file     | Excel文件 | 是      | file   |

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": ""
}
```

---

## 获取预约列表

- **接口地址**：`/api/appointment/list`
- **请求方式**：`GET`

### 响应示例

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