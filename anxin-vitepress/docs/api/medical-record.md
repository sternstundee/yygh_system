# 病历管理

## 创建病历记录

- **接口地址**：`/api/medical-record`
- **请求方式**：`POST`
- **请求数据类型**：`application/x-www-form-urlencoded, application/json`
- **响应数据类型**：`*/*`

### 请求参数

| 参数名称              | 说明         | 是否必须 | 类型   |
| --------------------- | ------------ | -------- | ------ |
| patientId             | 患者ID       | 否       | string |
| doctorId              | 医生ID       | 否       | string |
| departmentId          | 科室ID       | 否       | string |
| appointmentId         | 预约ID       | 否       | string |
| visitDate             | 就诊日期     | 否       | string |
| chiefComplaint        | 主诉         | 否       | string |
| presentIllness        | 现病史       | 否       | string |
| pastHistory           | 既往史       | 否       | string |
| physicalExamination   | 体格检查     | 否       | string |
| auxiliaryExamination  | 辅助检查     | 否       | string |
| diagnosis             | 诊断         | 否       | string |
| treatmentPlan         | 治疗方案     | 否       | string |
| followUpPlan          | 随访计划     | 否       | string |

### 请求示例

```json
{
  "patientId": "1",
  "doctorId": "2",
  "departmentId": "3",
  "appointmentId": "4",
  "visitDate": "2024-06-01",
  "chiefComplaint": "头痛",
  "presentIllness": "持续2天",
  "pastHistory": "无",
  "physicalExamination": "正常",
  "auxiliaryExamination": "CT正常",
  "diagnosis": "感冒",
  "treatmentPlan": "多喝水",
  "followUpPlan": "一周后复查"
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

## 获取病历记录详情

- **接口地址**：`/api/medical-record/{id}`
- **请求方式**：`GET`

### 路径参数

| 参数名称 | 说明   | 是否必须 | 类型   |
| -------- | ------ | -------- | ------ |
| id       | 病历ID | 是       | string |

### 响应示例

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "id": "1",
    "patientId": "1",
    "doctorId": "2",
    "departmentId": "3",
    "appointmentId": "4",
    "visitDate": "2024-06-01",
    "chiefComplaint": "头痛",
    "presentIllness": "持续2天",
    "pastHistory": "无",
    "physicalExamination": "正常",
    "auxiliaryExamination": "CT正常",
    "diagnosis": "感冒",
    "treatmentPlan": "多喝水",
    "followUpPlan": "一周后复查"
  }
}
``` 