# 科室管理

## 添加科室

- **接口地址**：`/api/department/save`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称        | 说明         | 是否必须 | 类型   |
| --------------- | ------------ | -------- | ------ |
| departmentName  | 科室名称     | 否       | string |
| departmentCode  | 科室编码     | 否       | string |
| parentId        | 上级科室ID   | 否       | string |
| leader          | 负责人       | 否       | string |
| phone           | 电话         | 否       | string |
| address         | 地址         | 否       | string |
| status          | 状态         | 否       | int    |

### 请求示例

```json
{
  "departmentName": "内科",
  "departmentCode": "NK001",
  "parentId": "0",
  "leader": "李主任",
  "phone": "13800000004",
  "address": "一楼东区",
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

## 获取科室列表

- **接口地址**：`/api/department/list`
- **请求方式**：`GET`

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "departmentName": "内科",
      "departmentCode": "NK001",
      "parentId": "0",
      "leader": "李主任",
      "phone": "13800000004",
      "address": "一楼东区",
      "status": 1
    }
  ]
}
``` 