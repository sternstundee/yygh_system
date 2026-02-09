# 患者管理

## 导入患者Excel数据

- **接口地址**：`/api/patient/import`
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

## 获取患者列表

- **接口地址**：`/api/patient/list`
- **请求方式**：`GET`

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "name": "张三",
      "gender": "男",
      "age": 30,
      "phone": "13800000003"
    }
  ]
}
``` 