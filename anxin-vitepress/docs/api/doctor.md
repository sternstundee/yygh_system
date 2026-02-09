# 医生管理

## 添加医生

- **接口地址**：`/api/doctor/add`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称   | 说明     | 是否必须 | 类型   |
| ---------- | -------- | -------- | ------ |
| name       | 姓名     | 否       | string |
| title      | 职称     | 否       | string |
| specialty  | 专业     | 否       | string |
| age        | 年龄     | 否       | int    |
| phone      | 电话     | 否       | string |
| gender     | 性别     | 否       | string |
| status     | 状态     | 否       | int    |
| category   | 类别     | 否       | string |
| department | 科室     | 否       | string |
| schedules  | 排班信息 | 否       | array  |

### 请求示例

```json
{
  "name": "李医生",
  "title": "主任医师",
  "specialty": "内科",
  "age": 40,
  "phone": "13800000001",
  "gender": "男",
  "status": 1,
  "category": "全职",
  "department": "内科"
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

## 获取医生列表

- **接口地址**：`/api/doctor/list`
- **请求方式**：`GET`

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "name": "李医生",
      "title": "主任医师",
      "specialty": "内科",
      "age": 40,
      "phone": "13800000001",
      "gender": "男",
      "status": 1,
      "category": "全职",
      "department": "内科"
    }
  ]
}
``` 