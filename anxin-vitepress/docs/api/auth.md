# 认证管理

## 用户注册

- **接口地址**：`/api/auth/register`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称      | 说明       | 是否必须 | 类型   |
| ------------- | ---------- | -------- | ------ |
| username      | 用户名     | 是       | string |
| password      | 密码       | 是       | string |
| realName      | 真实姓名   | 是       | string |
| phone         | 手机号     | 否       | string |
| email         | 邮箱       | 否       | string |
| role          | 角色       | 是       | string |
| departmentId  | 科室ID     | 否       | string |

### 请求示例

```json
{
  "username": "test",
  "password": "123456",
  "realName": "张三",
  "phone": "13800000000",
  "email": "test@example.com",
  "role": "doctor",
  "departmentId": "1"
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

## 用户登录

- **接口地址**：`/api/auth/login`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称 | 说明   | 是否必须 | 类型   |
| -------- | ------ | -------- | ------ |
| username | 用户名 | 是       | string |
| password | 密码   | 是       | string |

### 请求示例

```json
{
  "username": "test",
  "password": "123456"
}
```

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": ""
}
```

---

## 用户登出

- **接口地址**：`/api/auth/logout`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded`
- **响应数据类型**：`*/*`

### 请求参数

无

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
``` 