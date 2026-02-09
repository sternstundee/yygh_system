# 用户管理

## 添加用户

- **接口地址**：`/api/user/add`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称   | 说明     | 是否必须 | 类型   |
| ---------- | -------- | -------- | ------ |
| username   | 用户名   | 否       | string |
| password   | 密码     | 否       | string |
| realName   | 真实姓名 | 否       | string |
| phone      | 手机号   | 否       | string |
| email      | 邮箱     | 否       | string |
| roleId     | 角色ID   | 否       | string |
| status     | 状态     | 否       | int    |

### 请求示例

```json
{
  "username": "user1",
  "password": "123456",
  "realName": "王五",
  "phone": "13800000002",
  "email": "user1@example.com",
  "roleId": "admin",
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

## 获取用户列表

- **接口地址**：`/api/user/list`
- **请求方式**：`GET`

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": "1",
      "username": "user1",
      "realName": "王五",
      "phone": "13800000002",
      "email": "user1@example.com",
      "roleId": "admin",
      "status": 1
    }
  ]
}
``` 