# 消息管理

## 添加消息

- **接口地址**：`/api/message/save`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称 | 说明   | 是否必须 | 类型   |
| -------- | ------ | -------- | ------ |
| userId   | 用户ID | 否       | string |
| content  | 内容   | 否       | string |
| type     | 类型   | 否       | string |
| status   | 状态   | 否       | int    |

### 请求示例

```json
{
  "userId": "1",
  "content": "您的预约已成功！",
  "type": "通知",
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

## 获取消息列表

- **接口地址**：`/api/message/list`
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
      "content": "您的预约已成功！",
      "type": "通知",
      "status": 1
    }
  ]
}
``` 